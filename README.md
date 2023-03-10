# 영상처리 및 센서 퓨전 기반 실내 자율 주행 이동체 개발

###### 
  
  
## 개요
> 무인이동체를 활용한 인공지능 자율주행(K-Digital) 프로젝트  
> > 진행기간 : 2022년 12월 05일 ~ 2023년 1월 11일  
> > 프로젝트제목 : 인공지능과 사물인터넷의 융합  
> > rc카와 stella N2를 이용하여 차선을 감지하고 객체를 학습시켜 자율 주행 이동체를 개발하는 프로젝트 입니다.  

</br>

## 개발환경 및 사용기술
#### `언어`
- python
- c
- OpenCV
- Teachable Machine
- ARDUINO
- TensorFlow
- Keras

#### `환경`
- ROS(Noetic Ninjemys)
- Linux(Ubuntu_18.04)
- ubuntu MATE

#### `프로젝트 관리 도구`
- git, github
- jandi
- Visual Studio Code


</br>

## 하드웨어
- Arduino Uno R3
- ESP32-cam
- Logitech C920
- DC Motor 5V
- L298N
- L9110
- HW-432(XL6009E1)
- Ceramic Capacitor
- HC-05
- HC-06
- Mini Bread Board
- Arduino protosheild
- Arduino uno USB B cable
- 9V Battery
- Lithium-ion Battery 3.7V
- 18650 Battery holder
- Ni-Cd 1.2V AA * 4
- Jumper Wire
- JST 2pin connector
- Multi tester

</br>

## 영상처리 
stella는 세밀한 각도 조절이 가능하고, rc카는 세밀한 각도 조절이 어려워 영상처리 코드를 다르게 구현하였습니다.
- [stella](./stella_cv_func.py)
- [rc카](./CVlib.py)

</br>

## stella
- 모터동작과 회전 및 조향을 하는 코드 작성
- [stella](./stella_line_tracking.py)


</br>

## 인공지능
- [딥러닝](./LSB_deeplearning/)

- 보다 정밀한 사물인식을 구현하기위해 keras와 Tensorflow를 사용

![kerasAndTensor](https://user-images.githubusercontent.com/109050683/212276444-2e87fabc-161f-472c-9538-c7ae0dab96ba.png)

- 인공지능을 통하여 stella와 rc_car의 움직임을 제어하고 싶었고, 아두이노를 통하여 서보모터를 제어하는 코드로 선행을 진행하였습니다.

![servo_webc_2](https://user-images.githubusercontent.com/109050683/212274960-7ffd2371-5db8-4960-8de7-2c93b289a07d.gif)

</br>

## 미구현 및 개선사항
- 영상처리 적용, 학습 모델 적용, 하드웨어 제어 이 세가지를 합치는 과정에서 물리적/기술적 제약으로 인한 한계를 느꼈습니다.
- 예외처리 코드와 고민하던 코드를 적용시키지 못했던 부분이 아쉬웠습니다.


</br>

#### [발표 ppt](https://www.canva.com/design/DAFXLS8lMWA/PR6ZuXmCWh_rvvsVbPWt3A/view?utm_content=DAFXLS8lMWA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
