---
title: "Raspberry Pi UART 시리얼 통신 사용하기"
categories: IT
tags:
  - Raspberry Pi
  - CO2
  - MH-Z19B
  - UART
toc: true
toc_sticky: true
published: true
---

- 참고 사이트 및 서적
	- <https://pypi.org/project/mh-z19/>
	- 	<https://wikibook.co.kr/python-36-programming/>

## MH-Z19B Sensor

이전에는 I2C를 이용한 시리얼 통신을 했으니, 이번에는 UART를 이용한 시리얼 통신에 도전해보자.

참고 서적에 따르면, UART는 비동시식 시리얼 통신으로, 2개의 핀(TX, RX)만을 사용하여 데이터를 주고 받으며 일대일 통신만 가능하다. 이를 테스트 해 볼 수 있는 센서가 CO2 를 측정하는 [**MH-Z19B**](https://www.winsen-sensor.com/d/files/infrared-gas-sensor/mh-z19b-co2-ver1_0.pdf) 이다.

본 센서는 자체 온도 측정 값으로 보정한 **CO2 농도**를 ppm 단위로 계산하여 보여준다.


|![image](https://user-images.githubusercontent.com/61964210/77311453-774d1c00-6d43-11ea-9106-aeddf38b0722.png)|
|:---:|
|*MH-Z19B Specification*|

## Enabling UART

먼저 UART를 활성화하기 위해, 다시 설정화면으로 들어가 시리얼 통신을 Enable 하자. [[참고 링크](https://github.com/UedaTakeyuki/mh-z19/wiki/How-to-Enable-Serial-Port-hardware-on-the-Raspberry-Pi)]

``` bash
$ sudo raspi-config
```
![image](https://github.com/UedaTakeyuki/mh-z19/raw/master/pic/ss.2018-11-20.10.49.28.png?raw=true)

본 설정을 마치고 나면, Raspberry Pi가 재부팅된다.

참고로 시리얼  사용 해, python 명령어 실행시, **관리자 권한**이 필요하다.
{: .notice--warning}

>  -   **By raspi-config command**: The serial ports are opened with permission  `crw-rw-rw- 1 root dialout`
>-   **By editing /boot/config.txt file**: The serial ports are opened with permission  `crw--w---- 1 root tty`
>
>So, if you would use it without  **root**  permission, the former might be comfortable.



UART 장치가 추가되었는지 여부는 다음과 같이 확인 가능하다.

``` bash
pi@raspberrypi:~ $ ls -al /dev/serial*
lrwxrwxrwx 1 root root  5 Mar 23 16:45 /dev/serial0 -> ttyS0 # UART
lrwxrwxrwx 1 root root  7 Mar 23 16:45 /dev/serial1 -> ttyAMA0 # Bluetooth
```

## Cabling

이제, Raspberry Pi와 mh-z19를 다음과 같이 연결하자.

|Pi|Sensor|Line Color
|:---:|:---:|:---:|
|5.0V|Vin|gray|
|GND|GND|green|
|TxD|RxD|blue|
|RxD|TxD|purple|

## Source Code

그리고 mh-z19에서 제공하는 모듈을 설치한다.
``` bash
$ sudo pip install mh-z19
```

그리고 다음과 같이 실행할 수 있다.
``` bash
pi@raspberrypi:~/mh-z19/pypi $ sudo python -m mh_z19
{'co2': 500}
```
또는 파이썬에서 아래와 같이 직접 입력하여 테스트해 볼 수 있다.
``` python
pi@raspberrypi:~/work $ sudo python
Python 2.7.16 (default, Oct 10 2019, 22:02:15)
[GCC 8.3.0] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import mh_z19
>>> mh_z19.read()
{'co2': 410}
```
[mh-z19의 Data Sheet](https://www.winsen-sensor.com/d/files/infrared-gas-sensor/mh-z19b-co2-ver1_0.pdf)에 따르면, preheat time이 3분이라고 되어 있어, 연결이 불안정하다면 정확한 값이 나오지 않을 수 있다.

아래는 [스크립트 파일](https://github.com/IcedVanillaLatte/Raspberry_Pi/blob/master/mh_z19b.py)의 예시이다.
``` python
#!/usr/bin/python
# -*- coding:utf-8 -*-

import mh_z19
print  "CO2 Value Only: ", mh_z19.read()
print  "All Values: ", mh_z19.read_all()
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIxNDM1MzM0MjBdfQ==
-->