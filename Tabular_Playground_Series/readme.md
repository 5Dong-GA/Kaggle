# Tabular PlayGround Series 
![TPS](https://user-images.githubusercontent.com/69240893/133883210-e851c757-e7bf-43b4-8dbe-e404237945f6.PNG)

# Description
- train.csv : 119개의 Ambigious Columns, 1개의 Target Column인 'Claim', 1개의 Index Column인 'id'
- test.csv : 119개의 Ambigious Columns
- sample_submission.csv : train.csv로 학습시킨 모델을 test.csv에 대해 예측하고 제출하기 위한 파일

# Simple EDA
- train.csv와 test.csv의 Column들간 Distribution 보기 위함
- train.csv에서 Target Column의 값이 1인지 0인지에 따른 Distribution difference 확인
- Distribution 확인 함으로써 Feature Engineering 할 때의 방향 설정

# Handling Missing Values
- 가장 어려운 문제 : KNNImputer 사용할 예정이었지만 시간이 너무 오래 걸려서 일단 포기함
-> CPU 기준 1개의 Column당 18분 소요
- StnadardScaler, MinMaxScaler, RobustScaler 사용해보았지만 제대로 동작하는지 아직 확인을 못함

# Kaggle Score
- 1000/1500 .... Feature Engineering 없이 XGBClassifier로 원본데이터 그대로 돌려서 제출            
- 0.764로 나쁘지는 않지만 Feature Engineering + Outlier Imputation or Removal 해봐야 알듯
