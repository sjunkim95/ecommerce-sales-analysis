# E-Commerce Sales Analysis

Exploratory Data Analysis (EDA) project on the Online Retail dataset using Python, Pandas, and Matplotlib.

---

## Project Information

- **Analysis Type:** Exploratory Data Analysis (EDA)
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib
- **Environment:** Jupyter Notebook
- **Dataset:** Online Retail Dataset (UCI Machine Learning Repository)

---

## Project Overview

Python과 Pandas를 활용하여 데이터 정제(Data Cleaning), 특성 생성(Feature Engineering), 탐색적 데이터 분석(EDA)을 수행하였다.

이를 통해 매출, 고객, 상품 관점에서 데이터의 주요 패턴과 특징을 확인하고자 하였다.

---

## Data Cleaning

분석에 앞서 다음과 같은 데이터 정제를 수행하였다.

- CustomerID 결측치 제거
- Quantity가 0 이하인 데이터 제거
- UnitPrice가 0 이하인 데이터 제거
- 취소 주문(Cancelled Order) 제거

---

## Feature Engineering

분석을 위해 다음과 같은 파생 컬럼을 생성하였다.

- Sales = Quantity × UnitPrice
- Year
- Month
- YearMonth

---

## Exploratory Data Analysis (EDA)

### 1. Monthly Sales Analysis

- 월별 매출을 집계하고 시각화하여 매출 추이를 확인하였다.

### 2. Country Sales Analysis

- 국가별 총매출을 집계하여 매출이 높은 국가를 확인하였다.
- United Kingdom의 매출 비중이 매우 높아 영국을 제외한 국가별 매출도 추가로 비교하였다.
- 국가별 고객 수와 매출의 관계를 함께 분석하였다.

#### Country Sales (Excluding UK)
<img width="700" height="300" alt="sales_exclude_UK" src="https://github.com/user-attachments/assets/91e2f3e2-afea-4a15-b48a-8e7730aff027" />

#### Customer Count (Excluding UK)
<img width="700" height="300" alt="customer_count_excludeUK" src="https://github.com/user-attachments/assets/f36eaf6a-8498-4fb6-8091-3b3a83f1f665" />



### 3. Product Sales Analysis

- 상품별 판매 수량을 집계하여 가장 많이 판매된 상품을 확인하였다.
- 판매량이 높은 상품과 매출이 높은 상품의 차이를 비교하였다.
- 상품 가격이 매출에 미치는 영향을 함께 확인하였다.

### 4. Customer Sales Analysis

- 고객별 총매출을 집계하여 매출 기여도가 높은 고객을 확인하였다.
- 상위 고객의 매출 집중도를 분석하였다.

---

## Key Findings

- 월별 매출은 전반적으로 증가하는 추세를 보였다.
- United Kingdom이 전체 매출과 고객 수의 대부분을 차지하였다.
- Netherlands와 EIRE는 고객 수가 적음에도 높은 매출을 기록하였다.
- 고객 수보다 고객당 구매 규모가 매출에 더 큰 영향을 줄 수 있음을 확인하였다.
- 판매량이 높은 상품과 매출이 높은 상품은 일부 차이를 보였다.
- 고객별 매출 편차가 크게 나타나 매출 집중 현상이 존재함을 확인하였다.

---

## Conclusion

이번 프로젝트에서는 Online Retail 데이터를 활용하여 매출, 고객, 상품 관점의 탐색적 데이터 분석(EDA)을 수행하였다.

향후에는 고객별 구매 이력 데이터를 활용하여 재구매 패턴과 고객 특성을 분석하고, 고객 그룹별 구매 행동의 차이를 비교하는 분석도 진행해볼 수 있을 것으로 생각된다.
