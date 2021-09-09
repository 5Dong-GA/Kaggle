# 타이타닉 생존자 예측
![titanic](https://user-images.githubusercontent.com/69240893/132626842-eac06036-0ded-4dc1-9234-5bba04723aff.PNG)
캐글 처음 시작하면 누구나, 모두가 권장하는 Competition인 타이타닉 생존자 예측에 대해 혼자 해본 내용입니다.

# OverView
데이터는 두 그룹으로 분할되었습니다.
- train.csv
- test.csv


train.csv는 모델을 구축하는 데 사용

test.csv는 train.csv를 통해 제작한 모델로 직접 예측하는 데 사용

# 구성 IPYNB 파일
1. Moo-titanic1.ipynb : train.csv에서 Columns 분석 후 간단한 전처리 진행
2. Moo-titanic2.ipynb : 간단한 전처리 과정 적용한 train.csv에 대해서 machine Learning 진행하기 위한 전처리 + 모델링 과정 + 모델평가
