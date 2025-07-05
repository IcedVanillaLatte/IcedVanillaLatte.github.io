---
title: "Raspberry Pi 디지털 입출력"
categories: IT
tags:
  - GPIO
  - LED
  - Raspberry Pi
toc: true
toc_sticky: true
published: true
---

- 참고 서적 : [빠르게 활용하는 파이썬 3.6 프로그래밍](https://wikibook.co.kr/python-36-programming/)


GPIO 5번 핀을 LED 한 쪽 끝과 연결하고, 다른 한 쪽 끝은 220$\Omega$ 저항을 통해 GND에 연결되도록 구성한다.

``` python
#!/usr/bin/python
# -*- coding: utf-8 -*-
import RPi.GPIO as GPIO  # GPIO 임포트
import time
 
pinNum = 5
GPIO.setmode(GPIO.BCM) #GPIO num으로 사용
GPIO.setup(pinNum, GPIO.OUT) #GPIO 5번 핀을 출력용으로 선언
 
cnt = 10
flag = True
while cnt > 0 :
    if flag :
        print ("LED is ON")
    else :
        print ("LED is OFF")
    GPIO.output(pinNum, flag) # flag가 True이면 LED가 켜지고 False이면 LED가 꺼진다
    cnt-=1
    flag = not flag
    time.sleep(0.5) # 0.5초 동안 sleep
GPIO.cleanup() #GPIO를 초기화

```



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM0NDk0NTk0LDcyODU5NTMxNl19
-->