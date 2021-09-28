# Natural Language Processing
- 자연어 처리-> 재밌는 거 같음
- 지금 하고 있는 Kaggle Competition 2개
- Spooky Author, Natural Language Processing with tweet disaster
- 조만간 이 두개 Competition도 올릴 예정

# Status
- nltk library, geotext library 이용해서 2600개의 결측치중 600개를 처리하였다.
- 무지성 최빈값이 아닌 내가 생각해서 해낸 나름의 세련된 방법이다.
- text를 nltk library 이용해서 tokenize한후 geotext library에서 제공하는 api를 이용하여
- 도시인지, 도시이면 어떤 나라인지, 나라면 어떤 나라인지 반환해주는 세련된 api이다.
- 이용해서 text를 tokenize 해놓은 결과물에 대해서 돌려서 location에 나라, 도시이름을 채워주는 방식으로 진행하였다.
- 이 과정중에 set의 특성인 중복 허용x를 이용하여 함수를 만들었다.

# Google Translator
- 예전에는 Kaggle에서 잘 동작했던 것 같은데 지금은 동작하지 않는다.
- version 문제인데 virtual env에서 삭제하고 새로 설치해야할 library들이 하두 많아서 일단 포기하였다
- google translator 이용해서 러시아, 스페인어등등 번역해서 가짓수를 줄이려고 하였는데...
- 
# Handling Text
- text에서 불용어를 포함해서 특수문자들을 다 지우고 위에 적어놓은 방법으로 한번 더 처리해볼 필요성을 느꼈다.
- 예를 들어 location에는 U.S, USA, United Statesm US등 다양한 종류의 location이 존재하는데
- 이를 통합해서 ML을 돌려야 더 높은 정확도가 나올 것 같아서 현재 진행중이다.
