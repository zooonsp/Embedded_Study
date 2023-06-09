### Bring up ###

간단하게 말하면, 컴퓨터가 성공적으로 부팅이 되게 끔 무한 디버깅을 통해 켜지도록 하는 것을 의미한다.   

부트로더 동작확인 및 펌웨어 및 OS 로드 등 다양한 작업을 수행한다. 

---
### SoC ###

System-on-a-Chip 의 줄임말이다. 여러 개의 컴퓨터 구성 요소를 한 개의 집적 회로 칩에 결합한 것을 말한다. 즉, 여러 페리퍼럴들이 한 칩에 모여있는 것을 의미한다.

---
### 유선통신 종류 ###

| 종류 | 내용 |
|:--:|:--:|
|UART|- 1:1 단순 통신<br> - Asynchronous<br>-CMOS 회로 사용|
|I2C|- 2개의 선으로 통신<br>- Open-Drain 회로 사용|
|SPI|- 4개의 선으로 통신<br> - I2C보다 빠름|
|CAN||
|Ethernet||
---
### 모터(스텝모터, 기어드 모터) ###
|모터 종류|내용|
|:--:|:--:|
|DC 모터|- 일반적인 모터|
|서브 모터(DC + 센서)|- DC모터 + 제어기 + 기어 세트<br>- DC 보다 더 강한 힘과, 정확한 각도 조절 가능|
|스테핑 모터|- DC와는 다른 원리로 동작되며, 로봇 팔에 주로 사용된다.|
<br>

DC 모터의 단점 극복
1. 각도 제어의 어려움
-> 엔코더 사용
2. 파워 약함
-> 회전수를 낮추고 힘을 높임(기어드 DC 모터)
3. 브러시 고갈로 인한 수명 단축
-> 브러시리스 모터 사용
---
### 페리페럴 ###

cpu, 메모리를 제외한 모든 건 페리페럴이다.

---
### ICU ###

르네사스의 Interrupt Controller를 지칭하는 말이다.
외부의 다양한 인터럽트 신호를 처리하기 위한 모듈인데, 인터럽트가 어디서 발생했는지 감지한다. 그리고 어떤 인터럽트부터 처리할지 제어하는데 인터럽트의 우선수위 번호를 발급해서 처리한다.


---
### HAL 라이브러리 ###

---
### 클럭설정 ###
클럭이 서로 다름, 맞출 때 어떤 로직을 통해서 클럭을 변경하는 가

---
### rising/falling edge ###

---
### call back에서 systick이 멈추는 이유 ###

---
### BSP ###
임베디드 Board를 Bring Up 시키기 위한 모든 S/W 모음집을 BSP(Board Support Package)라고 한다.

BSP 예시는 다음과 같다.
1. HW 개발 외주업체에서 전달받은 SW
2. 보드 완성품을 구매한 후, 전달받은 SW

BSP에는 아래와 같은 내용이 필수적으로 들어간다.
1. 부트로더
2. 운영체제
3. 주변장치들을 제어하는 SW - Device Driver

그리고 필수적이진 않지만 대부분 들어가는 것은 다음과 같다.
1. Example Code
2. Application Node - App 개발 안내 가이드

르네사스에서 제공하는 BSP(S/W)는 FSP(Flexible Software Package)라고 부른다.

---
### 각 보드 관해서 ###

1. Nucleo - F103RB / STM32-F103RB / ARM -Cortex M3
2. fpb - RA1E6 / RA1E6 /  ARM Cortex-M33
3. 라즈베리파이/ bcm2711 (Broadcom,  4코어)/ ARM - Cortex A72

---
### PWM ###

---
### 가속도 / 자이로센서 차이

|가속도 센서|자이로 센서|
|:-:|:-:|
|가속도를 측정하는 것으로 기울렸는지를 감지할 때 사용한다.|초당 각도의 변화량을 측정해서 각 속도를 알 수 있다.|
---
### Rpi4 ###
