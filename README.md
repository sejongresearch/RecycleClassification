# Recycle
2019 AI Term Project-Team Recycle

### 진행상황
* 데이터 수집 ([구체적 진행상황](https://github.com/SEEUNL/Recycle/issues/13))


* 간결한 학습 모델 구축 ([구체적 진행상황](https://github.com/SEEUNL/Recycle/issues/14)), [학습코드](https://github.com/SEEUNL/Recycle/blob/master/Untitled24_ipynb%EC%9D%98_%EC%82%AC%EB%B3%B8.ipynb)


* 데이터셋 분할 (train, test(직접 촬영한 데이터셋 포함), validation) (진행중)

### 계획 대비 진행 상황
* 비닐을 포함한 6개의 클래스로 분류할 예정이었지만 비닐 데이터셋이 적고 학습에 어려움이 있어 제외하기로 함. 


* 복잡한 모델을 사용하기에 앞서 학습과 평가에 이르는 골격을 짜기 위해 퀴즈때 구현한 VGGNet 모델과 유사한 간단한 모델을 사용.


* 데이터 셋을 나눌 때 코드를 이용하여 분류 시 train_test_split함수를 이용한 방법(데이터가 작은 경우 overfitting이 발생할 수 있음) 또는 계층적 샘플링을 사용할 예정이고 수동으로 폴더를 생성하여 나누는 방법과 고민 중.

* 라즈베리 파이는 사용하지 않기로 했음. openCV부분에서 실시간으로 카메라에 인식시키기로 했으나, 실제적 구현이 힘들 것 같아 구글 드라이브를 이용하기로 함.

### 앞으로의 계획
* OpenCV를 이용하여 데이터 이진화

* 모델 평가, 선정(VGGNet, Resnet, Inception, GoogleNet 등 여러가지 분류모델중 성능이 좋은 모델 선정)
  * 평가 지표: accuracy, precision, recall, F-measure 
  * 모델 성능 비교 시 데이터에 분포 차이가 있는 경우가 많으므로 F-measure 많이 사용
  * precision과 recall중 무엇을 중시할지 결정.
  * "precision이 0.9 미만인 모델은 채용X" 같은 최소조건을 정하고 이 조건을 만족하면서 F-measure, accuracy가 높은 모델 선택
  
   
* 모델 성능 개선
  * Data Augmentation 을 통한 데이터 증강(keras 내장 함수 이용)
  * 데이터셋 추가 
  * Batch Nomarlization
  * Hyperparameter Tuning(랜덤 서치)
  * 성능이 좋은 2가지 모델을 병렬로 구성하여 앙상블 모델 생성 

  
### 회의록
* [5월 28일 모임](https://github.com/SEEUNL/Recycle/issues/15)


* [5월 13일](https://github.com/SEEUNL/Recycle/issues/10)


* [5월 8일](https://github.com/SEEUNL/Recycle/issues/5)


* [4월 18일](https://github.com/SEEUNL/Recycle/issues/1)

### 보고서
https://github.com/sejongresearch/Recycle/blob/master/%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%20%EB%B3%B4%EA%B3%A0%EC%84%9C%20.pdf

### 발표 PPt
https://github.com/SEEUNL/Recycle/blob/master/ppt.pptx
