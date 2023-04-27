# CS_Project 딥러닝기반 의류분류모델
- 패션은 단추, 문양이 하나만 바뀌어도 다른 옷이 된다. 이런 사소한 디테일 하나에 옷의 구매여부가 결정되기 때문에 다양한 특징을 잘 추출해서 좋은 옷을 추천해줄 수 있는 모델을 만들고자 한다.
- 패션 데이터들이 일단 크기가 방대하여 현재 기기로는 현실적으로 시도가 불가능했다. 일단 시도부터 해보자는 마음으로 fashion-mnist데이터로 분류모델을 만들었다.


### 가설
- 딥러닝모델을 이용해 의류분류모델을 만들 수 있다.

### 데이터 소개
**Fashion mnist**
- 다양한 기계 학습 시스템을 교육하고 테스트하는 데 일반적으로 사용되는 패션 이미지의 대규모 무료 데이터베이스입니다.

**각 라벨 별 아이템**
- 0 :티셔츠/탑
- 1 :바지
- 2 :풀오버
- 3 :드레스
- 4 :코트
- 5 :샌들
- 6 :셔츠
- 7 :스니커즈
- 8 :가방
- 9 :앵클 부츠

### 데이터 모델링
**CNN 모델을 이용한 분류모델**
- epochs = 10
- batch_size = 64
<p align = "center">
<img src="https://user-images.githubusercontent.com/110000734/225844255-3fba6152-09a9-47ac-84e2-3264809aab20.JPG" width=400>


**검증데이터의 accuracy : 0.9**
<p align = "center">
<img src="https://user-images.githubusercontent.com/110000734/225843689-a6c37957-dcb8-44c6-883b-cc4684535d0e.png" width=500>

**모델 학습 오차율, 정확도 그래프**
<p align = "center">
<img src="https://user-images.githubusercontent.com/110000734/225843566-0ee9aa3f-309e-43e5-bb12-623d5d9f2d08.png" width=500>


**일부 데이터 검증**
- 예측가능하도록 흑백데이터로 변경 후 예측 진행
- 일부 데이터 검증에서는 어느정도 예측이 가능했다.
<p align = "center">
<img src="https://user-images.githubusercontent.com/110000734/225834055-d40516bf-d87a-4926-ba15-f49451c3f10f.JPG" width=500>

**하지만 검증결과와 다르게 예측력이 좋지는 않았다.**
  
<p align = "center">
<img src="https://user-images.githubusercontent.com/110000734/225845640-b24016a0-24c7-47f4-9db9-34c6e8d60524.png" width=400>
<img src="https://user-images.githubusercontent.com/110000734/225846621-e85e1dd5-cdfd-4e26-a8ca-c929b11fa2f0.png" width=100>
<img src="https://user-images.githubusercontent.com/110000734/225843447-b8cd0e84-1b33-47b3-8b3b-2e6bb781957e.png" width=320>


### **프로젝트 결과 및 회고**
- 의류분류 정확도가 90%가 넘는 모델을 만들었다.
- 처음에 3개의 데이터를 가지고 판별했을 때는 적중률이 나쁘지 않았지만 실제 샘플 데이터에 대한 예측률은 많이 떨어졌다.
- 성능을 개선하려고 노력해봤지만 실패했고 기본제공 데이터의 한계를 실감했다.
