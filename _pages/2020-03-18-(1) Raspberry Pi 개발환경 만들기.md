---
title: "Raspberry Pi 개발환경 만들기"
categories: IT
tags:
  - Raspberry Pi
toc: true
toc_sticky: true
published: true
---

참고 서적 : [빠르게 활용하는 파이썬 3.6 프로그래밍](https://wikibook.co.kr/python-36-programming/)

## 운영체제 다운로드 하기

먼저 Micro SD Card를 준비하자.
라즈베리파이 [공식 홈페이지](https://www.raspberrypi.org/downloads/)에서 Raspberry Pi 운영체제를 다운로드 받자.

홈페이지에서는 각 사용환경(윈도우, MacOS, Ubuntu)에 맞게 라즈페리파이 이미지를 SD Card에 구워주는 **Imager**를 제공하고 있다.

> **Raspbian** is our official operating system for **all** models of the Raspberry Pi.  Use **Raspberry Pi Imager** for an easy way to install Raspbian and other operating systems to an SD card ready to use with your Raspberry Pi:


**[Raspberry Pi Imager](https://www.raspberrypi.com/software/)**를 다운로드 받아 설치해서 실행하자. 이미지로 옮길 Raspberry Pi 는 (recommended) OS를 고르고, 설치할 SD Card의 위치를 선택해 **Write** 하자. 여기서는 2022-09-22 release 버전의 Raspberry pi OS (32-bit)를 설치했다.
(시간이 좀 많이 걸린다.)


![image](https://user-images.githubusercontent.com/61964210/76919358-f7bae980-690b-11ea-8dc5-d1ad60dd5975.png)


## 운영체제 실행하기
이미지가 설치된 SD Card를 Raspberry Pi에 넣고, 기본 설정을 위해 키보드, 마우스, 모니터를 연결하자. 안쓰던 유선 키보드, 마우스를 다시 꺼내야 한다.

micro-5pin 충전기를 꽂아 전원을 연결하면 자동으로 켜진다.

## WiFi 및 초기 설정하기

운영체제가 설치되면 자동으로 설정화면이 뜨는데, 여기서 와이파이를 잡아주자. 이전에는 지역을 KOR로 설정하는 경우 와이파이가 잡히지 않는 문제를 경험한적 있었는데, 적어도 이번 설치 과정에서는 같은 문제를 확인할 수 없었다.

지역설정, 시간, 키보드, SSID, 사용자 계정 및 비밀번호를 설정하고 나면, 설정한 WiFi로 소프트웨어 업데이트를 시작한다. 


5 GHz WiFi SSID 나, Hidden SSID는 라즈베리파이에서 찾지도 못하고 접속도 못하니 유의하자. 
{: .notice--warning}

터미널에서는 `/etc/wpa_supplicant/wpa_supplicant.conf` 파일을 통해 설정값을 입력할 수 있다.

``` bash
network = {
	ssid = "my-ap-ssid"
	psk = "my password"
	key_mgnt = 
```

골동품 키보드/마우스를 빨리 치우고 싶으니, 어서 SSH 통신을 활성화 시켜 원격접속 터미널로 접속하자.

SSH 통신 활성화는 `메뉴` > `Preference` > `Raspberry Pi Configuration` > `Configure Raspberry Pi system` > `Interface` 에서 설정 가능하다.

추가로, 이후 작업을 위해 `SSH` 뿐 아니라, `I2C`와 `Serial Port`도 같이 활성화 시킨다.

### 고정 IP 할당
DHCP로 IP를 받는 경우, Raspberry Pi 의 IP 주소가 재부팅할 때마다 바뀔 수 있다. 고정 IP를 할당하려면, `/etc/dhcpcd.conf`파일에 다음 예시를 참고하여 내용을 수정하자.
``` bash
# Example static IP configuration:
interface eth0
static ip_address=192.168.0.10/24
static ip6_address=fd51:42f8:caae:d92e::ff/64
static routers=192.168.0.1
static domain_name_servers=192.168.0.1 8.8.8.8 fd51:42f8:caae:d92e::1
```

네트워크 인퍼테이스를 `wlan0`로, `ip_address`를 원하는 주소로 설정하고, `routers`와 `domain_name_servers` 정도만 사용하는 AP 주소로 바꿔줘도 충분하다.

라즈베리파이에서 네트워크 서비스 재시작 명령어는 `service networking restart`이지만, 여기서는 그냥 화면 오른쪽 위 WiFi 아이콘을 이용해 `Turn Off/On`로 고정IP 설정이 잘 되었는지, 인터넷 접속은 잘 되는지 확인할 수 있다.

이제, putty나 터미널로 `ssh`를 사용해 원격으로 작업할 수 있다.

``` bash
$ ssh pi@192.168.xxx.xxx
```

## SMB 설치

Raspberry Pi와 작업용 PC, 맥, 리눅스 등 장치와의 원할한 파일 공유를 위해 samba를 설치하자.

``` bash
$ sudo apt-get install samba
```

혹시 DHCP 설정 및 관련 패키지 설치를 물으면, **NO**를 선택한다.
![image](https://user-images.githubusercontent.com/61964210/76933970-af162700-6931-11ea-96ca-760df3ed19da.png)


사용자 pi의 패스워드를 설정하자.
``` bash
$ sudo smbpasswd -a pi
```

`mkdir`로 작업할 폴더 `/home/pi/work`를 만들고, `/etc/samba/smb.conf` 설정파일에 아래와 같이 작업 폴더를 공유 폴더로 추가하자.
``` bash
[pi]
   comment = 'rpi samba'
   path = /home/pi/work
   valid user = pi
   writable = yes
   browseable = yes
```

그리고 백그라운드에서 실행되고 있는 smb 프로세스를 재시작하자.
``` bash
 $ sudo service smbd restart
```

Raspberry Pi가 시작할 때 samba가 자동실행 되도록 시작프로그램에 등록하자.
``` bash
$ sudo update-rc.d smbd defaults
```

## 파일 공유 

윈도우에서 Raspberry Pi 공유 폴더로 접근하려면, `Windows Key` + `R` 로 실행창을 띄운 후, `\\IP Address`를 입력하면 된다.
 ![image](https://user-images.githubusercontent.com/61964210/76934134-e5ec3d00-6931-11ea-8dd5-61012aeaf9a5.png)

맥에서 해당 공유 폴더로 접근하기 위해서는, `Finder`에서 `이동` > `서버에 연결` 을 누른후, IP 주소를 입력하면 접근 가능하다. [참고 링크](https://kimsungjin.tistory.com/235)
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F9925F93E5A7326F623)


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc0ODExNDc2OF19
-->
