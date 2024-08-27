
전체적으로 1~2장
1. 1장)단답형 서술형 
2.  1장 단답형 서술형
3.  1장 단답형 서술형
4. 2장 단잡형 서술형
5. 2장 단답형 서술형
6. 1장 단답형 서술형
7.  프로그램 작성 코드 작성 2장 //2장중 실습한곳  빈칸 채워넣기
8. 계산 //전류는 아님 
9. 저항 색띠
10. 계산 전류
11. 2장 단답형 서술형
12.   프로그램 작성 코드 작성 2장 //2장중 실습한곳
13. 2장 객관식
14. 2장 서술형
15. 2장 객관식
16. 서술형
17. 2장 객
18. 1장 서술형

핀번호x
풀네임 문제 x
모터 계산 문제x
총 18문제 


### 1장 나올만한것

1)  라즈베리파이 4 핀 레퍼런스 보드 1개
2)  ls 명령은 현재 디렉터리의 내용을 보는 명령입니다.
3)  mkdir 명령은 디렉터리를 생성하는 명령
4)  cd 명령은 디렉터리를 이동하는 명령
5)  핀맵 : 보드상의 칩을 만든 브로드컴사에서 정한 핀 이름으로<font color="#ffc000"> BCM GPIO </font>핀 번호
6)  <font color="#ffc000">wget</font> 명령은 명령행 기반으로 원격 파일을 가져오는 명령어입니다.
7)  dpkg 명령은 데비안 패키지 설치 프로그램으로
8)  putty는 SSH 원격 접속 프로그램입니다.
9)  ifconfig wlan0 명령을 주어 ❷ IP 주소를 확인합니다.  ifconfig 명령은 네트워크 인터페이스(랜카드, wifi 등) 설정 명령이고,
10)  wconfig wlan0 명령을 주어 ❹ AP를 확인합니다. iwconfig는 무선 네트워크 인터페이스(wifi 등) 설정 명령입니다.
11)  라즈베리파이에 삼바 서버를 설치하여 윈도우에서 라즈베리파이의 파일 시스템을 접근할 수 있도록 합니다. 리눅스와 윈도우간에 파일 및 프린터를 공유할 수 있게 해 주는 프로 그램입니다.
12) <font color="#ffc000"> apt</font> 명령은 라즈비안 리눅스의 기반이 되는 데비안 계열의 리눅스의 프로그램 설치 관리 프로그램입니다.
13)  <font color="#ffc000">sudo</font>는 pi 사용자에게 관리자 권한을 부 여하여 명령을 수행하게 합니다.
14) <font color="#ffc000"> netstat</font> 명령은 네트워크 연결 상태를 보는 명령입니다. <font color="#ffc000">-a</font>는 all의 약자로 모든 네트워크 상태를 보는 옵션
15)   pwd 명령은 present working directory의 약자로 현재 작업 디렉터리를 보는 명령입니다.
16)  <font color="#ffc000">xrdp</font> 원격 컴퓨터에 접속할 수 있는 그래픽 로그인 기능을 제공합니다.


### 2장 나올만한 것

1)  print
2)  while
3)  <font color="#ffc000">try~except</font>
4)   정수, 실수 출력하기
5)  $ <font color="#ffc000">gcc</font> _05_print_6.c –o _05_print_6
6)  저항
7)  GPIO(General Purpose Input Output)
8)  LED 켜고 끄기
9)  <font color="#ffc000">쓰레드</font> 프로그램은 하나의 프로그램에서 여러 가지 입력을 받아 처리해야하는 경우에 필 요합니다.
10)  메시지 큐 통신 : 
11)  <font color="#ffc000">브레드 보드</font> :  납땜을 하지 않고, 시험용 회 로를 구성할 수 있습니다.

01 ： import RPi.GPIO as GPIO 
02 ： 
03 ： led_pin =18 04 ：
05 ： GPIO.setmode(GPIO.BCM) 
06 ： 
07 ： GPIO.setup(led_pin, GPIO.OUT) 
08 ： 
09 ： pwm = GPIO.PWM(led_pin, 1.0) # 1.0Hz 
10 ： pwm.start(50.0) # 0.0~100.0 
11 ： 
12 ： try: 
13 ： while True:
14 ： pass 
15 ： except KeyboardInterrupt: 
16 ： pass 
17 ： 
18 ： pwm.stop() 
19 ： GPIO.cleanup()