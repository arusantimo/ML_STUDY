# ML_STUDY
머신러닝에 대한 공부와 계념 정리

# 머신러닝이란. (개인적인 공부에 의한 정리)

프로그래밍을 하지 않아도 컴퓨터가 학습하여 해결하는 기술

머신러닝의 가장큰 오해는 기계는 이해 할수 없고 데이타를 통해 예측하고 평가하는 것만 가능하다.


# 머신러닝에서 출발

수집한 데이타가 있다는 전재.

데이터 마이닝이 첫번째 단계이다. 데이터 마이닝이란 수집한 데이타안에서 가치있는 정보를 찾아내는 방법이다.

 - 예측 =>
 예측이란 데이타에서 어떤 규칙이나 특징들을 바탕으로 현재 시점에서의 미래를 예측하는 것이다.

 - 분류 =>
 데이타들을 분류하는 작업을 말한다. 강아지 사진과 고양이 사진을 분류하는 작업등을 생각할 수 있다.
 선택 항목이 2가지 경우인 경우는 2클래스 분류, 여러가지의 경우 다중 클래스 분류

## 지도학습기법

지도학습기법을 이용하기 위해서는 유의미한 결과들이 있어야한다는 전재가 있다.
예를 들어 가뭄이 3달 이상 지속되었다면 그해의 과일이 당도가 줋어 든다는 결과 지향적인 데이타가 존재해야지 지도학습기법을 이용할 수 있다.

지도학습이란 유의미한 결과에 의해서 예측이 가능하고 결과을 분류 할수 있다.
가령 예를 들면 알파고의 경우 이겼던 결과패턴과 졌던 결과패턴을 분류하게 되고 그렇다면 그 학습을 통해서 예측이 가능해 진다. 그런 (분류와 예측작업) 지도학습기법을 통해서 기계(컵퓨터)는 이기는 패턴으로 게임을 진행 할 수 있다.

쉬어가는 이야기. 무서운 이야기 일수 있지만 인공지능에 인간을 죽일 수 없다는 결과는 쉽게 넣을 수 없다는 것이 된다. 왜냐면 컴퓨터는 지도학습기법(경험)을 통해서만 선택을 하게 되어 있어 원하는 결과를 얻기위해 지도학습을 하는 것은 쉽지 않은 작업이 될수 있다. 인간을 죽일 수는 없다는 결과를 얻을 수 있는 데이타가 그렇게 많지 않다는 것이기 때문이기도 하다.

### 지도학습기법 일반적인 순서

1. 데이타 수집과 학습에 사용할 데이타를 정한다. (데이타 마이닝)

   연관성 분석: 연관성 규칙을 추출하는 방법 (예: 빵을 사는 사람은 우유도 같이 산다.)

   회귀 분석: 두자기 의상의 변수사이의 경향성 의존성을 수학적으로 분석 (예: 여름이 더워진다면.. 수박에 판매량이 증가한것이다.)

   클래스 분류: 비슷한 특성의 변수들을 점진적으로 분할하며 그룹화 하는 것이다.


2. 입력의 특징을 어떻게 표현할지 결정한다.

   (일반적으로는 백터 형태로 표현한다.) 백터형태는 x, y가 기본적으로 존재하는 그래프의 형태라고.. 생각하는게 편하다.

3. 학습 알고리즘을 결정한다.
4. 만들어진 모델의 정확도를 평가 (다른 테스트 알고리즘등을 이용해서 평가.)
5. 결과는 보통 내가 원하는 결과을 얻기 위한 현재의 선택을 얻는것이 일반적이다.

### 알고리즘의 종류와 특징

1. 일반화 선형 모델(GLM) :
선형회귀의 발전된 형태로 다양한 가능성 분산과 연결함수를 지원해서 분석자가 더 효고적인 데이타를 모델링 한다.

2. 의사결정 트리(Decision Tree) :
모 집단을 대상변수에 대해 동질적인 더 작은 로직으로 점진적으로 분할 하는 규직 집합을 학습하는 비지도 학습 방법.

3. 랜덤 포레스트(Random forest) :
널리  사용되는 총체적 학습 방법으로 여러 개의 의사결정 트리를 학습한 다음. 트리 전반에 걸친 평균을 구해 예측을 산출한다.

4. 딥러닝(deep learning) :
데이타의 고수준 패턴을 복합적인 다계층 네트워크로 모델링하는 방법.
문제를 모델링하는 가장 일반적인 방법이며 ML의 가장 어려운 문제를 해결할 잠재력이 있다.


## 비지도학습기법

유의미한 결과 데이타가 없다면 일반적인 분류작업은 할 수 있지만 학습작업(결과에 대한 분류 예측 작업)을 할수는 없다. 그렇지만 그런 데이타에서 유의미한 지식을 얻고자 할때 비지도 학습기법을 이용한다.

1. 클러스트링

개체를 다수의 매트릭스에서 상호 유사한 세그먼트 또는 클러스터로 그룹화하는 기법
고객의 세분화 그룹이 한가지 예다. 클러스트링의 알고리즘의 가장 일반적인 알고리즘이 k-means

2. 비정상 탐지

예상치 못한 이벤트 또는 결과를 식별하는 기법

## 비지도학습기법

유의미한 결과 데이타가 없다면 일반적인 분류작업은 할 수 있지만 학습작업(결과에 대한 분류 예측 작업)을 할수는 없다. 그렇지만 그런 데이타에서 유의미한 지식을 얻고자 할때 비지도 학습기법을 이용한다.

1. 클러스트링

개체를 다수의 매트릭스에서 상호 유사한 세그먼트 또는 클러스터로 그룹화하는 기법
고객의 세분화 그룹이 한가지 예다. 클러스트링의 알고리즘의 가장 일반적인 알고리즘이 k-means

2. 비정상 탐지

예상치 못한 이벤트 또는 결과를 식별하는 기법


## 텐서플로우 (구글 머신러닝 라이브러리)

<a href="https://gist.github.com/haje01/202ac276bace4b25dd3f" target="_blank">텐서플로우시작하기</a>

구글에서 딥러닝 머신러닝을 라이브러리 간단히 설명하면 일종의 데이타의 흐름을 포현해 주는 툴이라고 하면 된다.

### 텐서 tensor (다중벡터)
일종의 다차원 배열이라고 할수 있다. (0차원 => 스칼라, 1차원 => 벡터, 다차원 => 텐서)
### 플로우 flow
계속되는 공급, 흐름이라고 할 수 있다.
