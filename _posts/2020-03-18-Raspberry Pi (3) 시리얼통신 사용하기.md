---
title: "(3) I2C 시리얼 통신 사용하기"
categories: [Raspberry Pi]
tags: [Raspberry Pi, bme280, I2C]
toc: true
toc_sticky: true
published: true
---

- 참고 사이트 및 서적 
	- <https://learn.adafruit.com/adafruit-bme280-humidity-barometric-pressure-temperature-sensor-breakout/python-circuitpython-test>
	- <https://wikibook.co.kr/python-36-programming/>

## BME280 Sensor

시리얼 통신은 한 번에 하나의 비트를 보내는 데이터 전송 과정을 말한다.

Raspberry Pi에서 지원하는 시리얼 통신은 다음과 같다.
	- I2C (Inter-Integrated Circuit Interface)
	- SPI (Serial Peripheral Interface)
	- UART (Universal Asynchronous Receiver Transmitter)

**I2C 시리얼 통신**을 이용해 온도, 습도, 대기압을 측정해보자. 내가 구한 센서는 [**adafruit BME280**](https://cdn-learn.adafruit.com/downloads/pdf/adafruit-bme280-humidity-barometric-pressure-temperature-sensor-breakout.pdf)으로 다음 6개 단자를 지원한다.
- VIN, 3V, GND, SCK, SDO, SDI, CS

본 센서의 출력 값은 **온도**는 섭씨(ºC), **습도**는 상대습도(%RH), **대기압**은 hPa 단위로 계산되어 보여준다[[datasheet](https://cdn-shop.adafruit.com/datasheets/BST-BME280_DS001-10.pdf)].

## Cabling

이 센서를 Raspberry Pi와 아래와 같이 연결했다.

|Pi|Sensor|Line Color
|:---:|:---:|:---:|
|3V3|VIN|(blue)|
|GND|GND|(green)|
|SCL|SCK|(orange)|
|SDA|SDI|(yellow)|


## Enabling I2C Interface

그리고 Raspberry Pi에서 I2C 인터페이스를 활성화하자.

``` bash
 $ sudo raspi-config
 ```

![image](https://user-images.githubusercontent.com/61964210/77288244-b6b34280-6d1a-11ea-96e5-45ab4a639b1f.png)

I2C가 활성화 되었다면, `ls -l /dev/i2c*` 명령어를 통해 어떤 디바이스에 있는지 확인할 수 있다.

``` bash
pi@raspberrypi:~/work $ ls -l /dev/i2c*
crw-rw---- 1 root i2c 89, 1 Mar 23 15:26 /dev/i2c-1
```
1번 디바이스에 붙은 BME280 센서 주소를 `i2cdetect -y 1` 명령어로 확인하면 다음과 같다.

![image](https://user-images.githubusercontent.com/61964210/77288832-06463e00-6d1c-11ea-928e-67cf4d5b6945.png)

즉, Raspberry Pi는 BME280 센서 장치를 0x77 주소로 인식하고 있다. 아무 숫자가 보이지 않는다면, 접촉 불량이거나 센서 연결을 잘못한 것이다.

## Source Code

이제 Raspberry Pi에서 사용할 python을 취향에 따라 소스코드를 가져와 사용하자.
- 1번 : [[링크](https://bitbucket.org/MattHawkinsUK/rpispy-misc/src/master/python/bme280.py)]
- 2번 : [[링크](https://github.com/adafruit/Adafruit_CircuitPython_BME280/blob/master/examples/bme280_simpletest.py)]

위 원본 파일을 아래와 같이 수정하였다.
- 1번 : [[링크](https://github.com/IcedVanillaLatte/Raspberry_Pi/blob/master/bme280.py)]
	- 디바이스 주소 수정 등
- 2번 : [[링크](https://github.com/IcedVanillaLatte/Raspberry_Pi/blob/master/py3_bme280.py)]
	- 온도, 습도, 기압 각 센서 값 측정 후 `time.sleep(0.3)`으로 delay 부여 등



python 3.x에서 adafruit에서 제공하는 소스코드로 센서를 동작시키려면, 필요한 모듈을 사전에 설치해줘야 한다.

``` bash
 $ sudo pip3 install adafruit-circuitpython-bme280
 ```
> If your default Python is version 3 you may need to run 'pip' instead. Just make sure you aren't trying to use CircuitPython on Python 2.x, it isn't supported!


<!--stackedit_data:
eyJoaXN0b3J5IjpbNzI1NDM4NjgwXX0=
-->
