# Python_MachineLearning_Guide

<p align="center">
  <img width="250" height="350" src="https://user-images.githubusercontent.com/45617225/92135103-4ff79080-ee45-11ea-99af-e60505bcbfdd.png">
</p>

## 9. 추천시스템 
|  | 소제목 | 바로가기 | 
| :---: |:---:|:---:|
| 4 | 잠재 요인 협업 필터링 | [SGD를 이용한 행렬분해](https://github.com/jeeyeonLIM/Python_MachineLearning_Guide/blob/master/09_%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C_4.%EC%9E%A0%EC%9E%AC%20%EC%9A%94%EC%9D%B8%20%ED%98%91%EC%97%85%20%ED%95%84%ED%84%B0%EB%A7%81.ipynb) | 
| 5 | 콘텐츠 기반 필터링 | [Kaggle TMDB 영화 데이터셋](https://github.com/jeeyeonLIM/Python_MachineLearning_Guide/blob/master/09_%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C_5.%20%EC%BD%98%ED%85%90%EC%B8%A0%20%EA%B8%B0%EB%B0%98%20%ED%95%84%ED%84%B0%EB%A7%81_TMDB%205000%20%EC%98%81%ED%99%94%20%EB%8D%B0%EC%9D%B4%ED%84%B0.ipynb) | 
| 6 | 아이템 기반 최근접 이웃 협업필터링 | [KNN-Item기반](https://github.com/jeeyeonLIM/Python_MachineLearning_Guide/blob/master/09_%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C_6.%20%EC%95%84%EC%9D%B4%ED%85%9C%20%EA%B8%B0%EB%B0%98%20%EC%B5%9C%EA%B7%BC%EC%A0%91%20%EC%9D%B4%EC%9B%83%20%ED%98%91%EC%97%85%20%ED%95%84%ED%84%B0%EB%A7%81.ipynb) | 
| 7 | 행렬분해를 이용한 잠재요인 협업필터링 | [SGD-잠재요인](https://github.com/jeeyeonLIM/Python_MachineLearning_Guide/blob/master/09_%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C_7.%20%ED%96%89%EB%A0%AC%20%EB%B6%84%ED%95%B4%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%9E%A0%EC%9E%AC%20%EC%9A%94%EC%9D%B8%20%ED%98%91%EC%97%85%20%ED%95%84%ED%84%B0%EB%A7%81.ipynb) | 
| 8 | Surprise 패키지 | [Surprise](https://github.com/jeeyeonLIM/Python_MachineLearning_Guide/blob/master/09_%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C_8.%20%EC%B6%94%EC%B2%9C%EC%8B%9C%EC%8A%A4%ED%85%9C%20%ED%8C%A8%ED%82%A4%EC%A7%80_%60Surprise%60.ipynb) | 

#### 1. 콘텐츠 기반 필터링 
- 유저가 특정 영화를 감상하고 좋아했다면 비슷한 특성/ 속성, 구성요소를 갖는 다른 영화를 추천하는 것 
    - Ex. <인셉션> 재밌게 봤다면 인셉션의 장르인 액션, 공상과학으로 높은 평점을 받은 영화를 추천하거나, 크리스토퍼 놀란 감독의 다른 영화를 추천하는 방식 
- 상품/ 서비스간의 유사성을 판단하는 기준이 영화를 구성하는 다양한 콘텐츠(장르, 감독, 배우, 평점, 키워드, 영화 설명)을 기반으로 하는 방식

#### 2. 최근접이웃 협업필터링 - 아이템 기반
- 최근접 이웃 필터링 -> USER 기반 vs ITEM 기반 
- 일반적으로 ITEM 기반이 더 정확도가 뛰어남.
- Item 기반 : 유저가 비슷한 반응을 보이는 아이템끼리의 유사도를 기반으로 추천
- USER 기반 : 혜택에 유사하게 반응한 TOP-N 고객을 선별하여 그들이 봤던 아이템 추천

#### 3. 행렬 분해를 이용한 잠재 요인 협업 필터링
- NaN많은 user-item 평점 행렬에는 SGD, ALS 기반의 행렬분해 사용 

#### 추가사항
- 모델 평가할떄는 평점 존재하는 경우에 대해서만 계산, 추천할때는 평점 존재하지 않는 경우에 대해서만 추천
- 유저마다 평점 줄때 bias도 고려할 수 있음.




