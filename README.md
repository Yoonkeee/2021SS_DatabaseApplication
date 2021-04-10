# 2021SS_DatabaseApplication(COM4011)  
## Database Application(데이터베이스응용) by [이동호 교수님](http://database.hanyang.ac.kr)  
### PBL(Problem-Based Learning)

## 핵심 학습 목표  
- 우리나라 40세 이상 100만명의 일반겅간검진 데이터를 활용하여 연령별, 지역별, 성별 건강검진 내역의 건강상 특이점 분석, 중요 데이터 속성 추출 및 패턴 분석  

## 문제 시나리오
- 단순한 체지방지수(BMI)나 일반건강검진의 일부 항목만을 이용하여 당뇨병을 예측하는 모델은 정확도가 매우 떨어지는 상황이다.
- 다양한 항목들을 복합적으로 분석하여 향후 당뇨병 발생 여부를 미리 예측할 수 있는 새로운 데이터 모델을 개발하려 한다.

### 문제 상황
- 데이터에 일부 값이 누락되어있으며, 잘못 기재된 값들도 존재함  
  
### 목표
- 2017, 2018년도 국민건강정보데이터 건강검진정보를 활용하여 당뇨병 발병 확률을 예측하는 인공지능 모델 구현

#### 세부 목표
1. 단순 데이터 전처리 뿐만 아니라 데이터의 오류나 이상 유무 검출
2. 일반건강검진 항목들 중에서 당뇨병 발생과 관련이 깊은 항목 추출
3. 개발된 예측 모델들의 성능 측정

### Libraries
- Scikit-learn

### Outliers Filtering
- Data Read 단계에서 Feature와 Outlier로 판정할 최댓값, 최소값을 dict형식으로 전달하여 Filtering하였음    

### Scaler
- Robust Scaler 사용  

### To-Do
- Hyper Parameters Tuning (Grid Search)
- Decide **valid(medically)** pivots to verify outliers
- Decide Features with medical informations