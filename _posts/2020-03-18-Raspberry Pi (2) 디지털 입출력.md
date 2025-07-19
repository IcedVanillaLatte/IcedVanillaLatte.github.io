---
title: "(2) 디지털 입출력"
categories: [Raspberry Pi]
tags: [GPIO, LED, Raspberry Pi]
toc: false
toc_sticky: false
published: true
---

- 참고 서적 : [빠르게 활용하는 파이썬 3.6 프로그래밍](https://wikibook.co.kr/python-36-programming/)

라즈베리파이에서 실행시킨 명령들이 원하는 동작을 수행하였는지 콘솔이 아닌 외부에서 확인하기 위해, LED 불빛을 반짝일 수 있는 함수들을 만들었다.

``` python
#!/usr/bin/python
# -*- coding: utf-8 -*-
import RPi.GPIO as GPIO
import time

# LED Control Pin Number
BlueLedPin = 5
RedLedPin = 6

def GPIO_set():

    GPIO.setmode(GPIO.BCM)
    GPIO.setup(BlueLedPin, GPIO.OUT)
    GPIO.setup(RedLedPin, GPIO.OUT)

def GPIO_end():
    GPIO.cleanup()

def Blink_blue(times):
    for i in range(times):
        GPIO.output(BlueLedPin, True)
        time.sleep(0.1)
        GPIO.output(BlueLedPin, False)
        time.sleep(0.1)

def Blink_red(times):
    for i in range(times):
        GPIO.output(RedLedPin, True)
        time.sleep(0.1)
        GPIO.output(RedLedPin, False)
        time.sleep(0.1)

if __name__ == "__main__":
    GPIO_set()

    Blink_blue(3)
    Blink_red(3)

    GPIO_end()

```

라즈베리파이의 GPIO 포트는 3.3V 및 20mA를 출력한다. 그리고, LED에는 임계전압이 있어 너무 많은 전류량이 흐르면 LED가 바로 타버린다. 그래서 반드시 저항이 사용되어야 한다. [참고](https://opentutorials.org/module/779/7087)

![image](https://user-images.githubusercontent.com/61964210/203698459-9a18c4a6-7eff-4f8d-9242-7f416964537c.png)

옴의 법칙에 따라 $V=IR$ 이므로, 붉은색 LED는 $R=\displaystyle \frac{3.3-1.5}{0.02}=89.999...$ 로, 최소 90 $\Omega$ 이상의 저항이 필요하다. 여기서 저항값이 커지면 커질수록 LED 불빛은 점점 약해지게 된다.

LED는 다이오드의 종류 중 하나인 발광 다이오드로, **계측기를 통해 LED의 발광에 필요한 전압을 측정**할 수도 있다.
> 다이오드(diode)는 저마늄(영어: germanium 또는 게르마늄(독일어: germanium), Ge)이나 규소(Si)로 만들어지고, 주로 한쪽 방향으로 전류가 흐르도록 제어하는 반도체 소자를 말한다. 정류, 발광 등의 특성을 지니는 반도체 소자이다. (출처: [위키피디아](https://ko.wikipedia.org/wiki/%EB%8B%A4%EC%9D%B4%EC%98%A4%EB%93%9C))

또한, LED 다리가 긴 쪽이 양극(+), 짧은 쪽이 음극(-)을 의미한다. 저항은 극성이 없으므로 LED의 양극(+) 및 음극(-)어디에 연결해도 문제가 없다. 어떤 사람들은 전류는 양극(+)에서 음극(-)으로 흐르므로, 저항도 양극 방향에 붙여줘야 된다고 말하기도 한다. (다만, 직렬로 연결된 회로이기 때문에 전체 회로에 흐르는 전류량은 일정하고, 전압은 LED와 저항의 저항값에 비례한다.)

위에서는 GPIO 5번 및 6번 핀을 LED 한 쪽 끝(양극, +, 긴 다리)과 연결하고, 다른 한 쪽 끝(은극, -, 짧은 다리)은 220 $\Omega$ 저항을 통해 GND에 연결되도록 구성했다.

여기서 핀 번호는 아래 그림의 **BCM**에 적혀있는 번호를 의미한다.


![image](https://user-images.githubusercontent.com/61964210/203694700-b47e8230-a1a2-4ffd-bf75-8501af233db3.png)


