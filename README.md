# 🎉 2022-HBNU-Capstone-Design 🎉

<br>

## 적대적 공격 (Adversarial Attack) 💥
- 적대적 패턴: 적대적 패턴이란 공격자가 AI에 검출이 되지 않기 위해 인위적으로 만든 패턴
- 적대적 공격: 이 패턴이 포함된 물체는 검출이 되지 않게 하는 것

<br>

## 시나리오 🎞
  - 불법 주정차 차량을 탐지하기 위해 개별 센서를 통해 차량 데이터를 수집하고, 학습을 위해 이를 중앙의 서버로 전송
  - 무선 네트워크 상에서 데이터 전송이 이루어지는 중, 악의적 공격에 의한 데이터 손상(ex. 가우시안 노이즈 등)
  - 중앙 서버에 존재하는 AI 시스템은 불법 주정차 차량을 탐지할 수 없게 됨
  
  ![image](https://user-images.githubusercontent.com/68288862/206190023-f2dd07b6-5906-4a94-8006-0cf3d35e1ec8.png)

<br>

## 실험 #1: 차량의 특징적인 부분 제거하기
  - 3가지 test case: 바퀴 / 바퀴 + 헤드라이트 / 바퀴 + 헤드라이트 + 사이드미러
  ![image](https://user-images.githubusercontent.com/68288862/206190874-92326510-72df-4dd0-b75c-ad58a3542498.png)

<br>

## 실험 #2: 차량 이미지 전체에 가우시안 노이즈 생성
  - 표준편차(std) 값이 커질수록 노이즈 커짐
  
  ![image](https://user-images.githubusercontent.com/68288862/206190194-ec1de97d-1bb8-41b4-85ea-90658bc7ca2b.png)
  
<br>

## 결과 📌
  - 노이즈 레벨에 따른 탐지 정확도
  ![image](https://user-images.githubusercontent.com/68288862/206191670-7f8085c6-1d34-485f-b73d-72fb3e5ebc8b.png)
