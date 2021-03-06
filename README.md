# Study_MachineLearning

1. 머신러닝이란
    프로그래밍 없이 컴퓨터가 학습하는 것

2. 머신러닝 동작원리
    기존에 룰을 만드는 프로그래밍 영역을 머신러닝 알고리즘이 대체한다.
    개발 workflow       : DATA -> Feature Extraction -> A Set Of Rules -> What is this Entitiy? -> Dog
    머신러닝 workflow : DATA -> Feature Extraction -> A Machine Learning Model -> What is this Entitiy? -> Dog

3. 머신러닝 기술 종류
    - Regression / Estimation : 집 값을 집계내어 다음 상승 하락을 예측한다.
    - Classification : 해당 케이스가 암인지 아닌지 구분한다.
    - Clustering : 비슷한 유형의 환자들을 묶는다.
    - Associations : 한 제품을 샀을때 연관되어서 사는 아이템들을 연관짓는다.
    - Anomaly detection : 금융 사기등의 이상 패턴들을 감지한다.
    - Sequence Mining : 홈쇼핑 고객의 다음 이벤트를 추론한다.
    - Dimension Reduction : 데이터의 사이즈를 줄인다.
    - Recommandation System : 새로운 아이템, 구입한 제품과 연관있는 아이템, 비슷한 아이템 등을 추천한다. 

4. 툴
    - Numpy
    - Scipy
    - marplotlib
    - pandas
    - scikit

5. 지도학습 vs 비지도학습
- 머신러닝을 어떻게 지도하는가 : 트레이닝 모델(레이블링 된 데이터셋)을 가지고 트레이닝 한다.
- supervised : classification(분류), regression(다음값 예측)ㅌ
- unsupervised : clustering, dimension reduction, density estimation, market based analysis

6. Regression (회기)
    1. 요인
    dependent variable : 의존요인으로 판단에 영향을 미치는 여러 요인
    independent variable : 독립요인으로 판단 결과가 되는 지표
    * 변수들은 연속적인 숫자형 이어야한다.
    2. Regression 종류
        Simple Regression : 독립 요인이 1개
        Multiple Regression : 독립 요인이 2개 이상
    3. 단순형 선형 회귀
        선형 회귀는 관계를 설명하는 데 사용되는 선형 모형의 근사값입니다.
        선형 회귀 분석의 핵심은 종속 값이 연속적이어야한다는 것입니다
        선형 회귀를 사용하면 데이터를 통해 선을 맞출 수 있습니다.
        예를 들어, EngineSize가 증가함에 따라 배출량도 증가합니다.
        선형 회귀를 사용하면 이러한 변수의 관계를 모델링 할 수 있습니다.
        오차는 데이터 점에서 적합 회귀선까지의 거리라고 말할 수 있습니다.
        모든 오차의 평균은 선이 전체 데이터 세트에 얼마나 적합하지 않은지를 보여줍니다.
        목표는 이러한 모든 오류의 평균이 최소화되는 라인을 찾는 것
    4. 복수형 선형 회기
        독립 변수가 여러 개인 경우 이 과정을 "다중 선형 회귀"라고합니다
    5. 모델 평가
        알려지지 않은 샘플을 예측하기 위해이 모델을 얼마나 신뢰할 수 있는지
        훈련 정확도는 모형을 사용할 때 올바른 예측의 백분율입니다.
        그러나 높은 훈련 정확도가 반드시 좋은 것은 아닙니다.
        훈련 정확도가 높으면 데이터가 '과적 합'될 수 있습니다.
        즉, 모델이 데이터 집합에 대해 과도하게 훈련되어 노이즈 및 일반화되지 않은 모델을 생성하는 것을 말합니다.
        1. Train/Test Split : 테스트 세트의 예측 값이 실제 값과 비교됩니다.
        2. K- 폴드 교차 검증
        3. training accuracy” and “out-of-sample accuracy
    6. 비 선형 회귀
    데이터가 선형이 아닌 경우 다항식 회귀(Polynomial regression)가 사용된다.
