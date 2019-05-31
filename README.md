# Recycle
2019 AI Term Project-Team Recycle

### 진행상황
* 데이터 수집 ([구체적 진행상황](https://github.com/SEEUNL/Recycle/issues/13))


* 간결한 학습 모델 구축 ([구체적 진행상황](https://github.com/SEEUNL/Recycle/issues/14)), [학습코드](https://github.com/SEEUNL/Recycle/blob/master/Untitled24_ipynb%EC%9D%98_%EC%82%AC%EB%B3%B8.ipynb)


* 데이터셋 분할 (train, test, validation) (진행중)

### 계획 대비 진행 상황
* 비닐을 포함한 6개의 클래스로 분류할 예정이었지만 비닐 데이터셋이 적고 학습에 어려움이 있어 제외하기로 함. 


* 학습 모델 구축에 차질이 있어 아직 기초적인 모델임.


* 데이터 셋을 나눌 때 cross validation을 사용할 계획이었으나 코드를 이용하여 분류 시 train_test_split함수를 이용한 방법을 사용할 예정이고 수동으로 폴더를 생성하여 나누는 방법과 고민 중. (데이터가 작은 경우 overfitting이 발생할 수 있기 때문)

* 라즈베리 파이는 사용하지 않기로 했음. openCV부분에서 실시간으로 카메라에 인식시키기로 했으나, 실제적 구현이 힘들 것 같아 구글 드라이브를 이용하기로 함.

* keras의 ImageDataGenerator의 데이터 크기, 기울기 조절 등의 기능을 이용하여 데이터 셋을 늘렸음.

### 앞으로의 계획
* OpenCV를 이용하여 데이터 이진화


* 학습 모델 평가와 이에 따른 수정


### 회의록
* [5월 28일 모임](https://github.com/SEEUNL/Recycle/issues/15)


* [5월 13일](https://github.com/SEEUNL/Recycle/issues/10)


* [5월 8일](https://github.com/SEEUNL/Recycle/issues/5)


* [4월 18일](https://github.com/SEEUNL/Recycle/issues/1)

