---
title: 부도예측모형 및 회계부정탐지를 통한 알파투자전략
subtitle: 재무데이터를 통한 부실기업예측 및 알파투자전략 제공
image: ..\assets\img\portfolio\project2.png
alt: Shirts on a hanger

caption:
  title: 부도예측모형 및 회계부정탐지를 통한 알파투자전략
  subtitle: 재무데이터를 통한 부실기업예측 및 알파투자전략 제공
  thumbnail: ..\assets\img\portfolio\project2.png
---

부실기업에 투자하는 것을 방지하기 위해 재무데이터로 부도예측 및 회계부정탐지를 통한 알파투자전략을 제시함.
Fama-French의 three factor 모형에 따르면 시가총액이 작고 가치가 높은 기업일수록 초과수익을 내기 유리함
추가적으로 부도예측 및 회계부정 탐지를 통해 리스크를 줄이면 안정적으로 초과수익을 얻을 수 있을 것으로 기대할 수 있음.
데이터수집기간 : 2011 ~ 2020년(재무데이터) / 2012~2021년(주가데이터)
기업범위 : KOSPI와 KOSDAQ 상장기업 중 금융권 제외(2,814사)
Feature Data : 총 141개의 재무비율 중 90개의 재무비율(재무데이터 미존재, 결측치가 1/3 초과, 재무데이터 누락 기업제거) 
<br>
![ex_screenshot](..\assets\img\portfolio\project2-1.png){: width="100%" height="100%"}
<br>
위의 순서로 진행했으며, Feature Selection을 통해 90개의 Feature를 각각 6개와 3개로 추출해 모델링을 진행함.<br>
부도예측과 회계부정탐지에 해당하는 기업을 제외하여 KOSPI지수를 벤치마킹하여 Backtesting을 진행함
정상기업(부도로 판단되지 않으면서 회계부정탐지에 해당되지 않는 기업)으로 판단되는 기업의 경우 KOSPI와 비교하여 수익률이 존재한다면 안정적인 초과수익이 발생한다고 판단할 수 있음
정상기업중 기업규모에 따라 Backtesting을 진행한 결과 대기업보다는 중소기업의 수익률이 높은 것을 확인함
따라서 정상기업이면서 중소기업인 경우 안정적이면서 보다 초과적인 수익을 기대할 수 있음

{:.list-inline}

- Date: 2022.02.21~2022.03.18
- Category: Python
- Modeling: Linear Regression, KNN, SVC, Decision Tree, RandomForest, XGB, LGB, MLP