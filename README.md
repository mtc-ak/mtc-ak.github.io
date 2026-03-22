# 마이크로바이옴 기반 대장암 예측 연구

**Microbiome-Based Colorectal Cancer Prediction**

홈페이지: https://mtc-ak.github.io/

## 연구 개요
- 데이터: ZellerG_2014 (개발 n=290) + YachidaS_2019 (외부 검증 n=212)
- 모델: Logistic Regression, Random Forest, XGBoost
- 전처리: CLR 변환, Rarefaction (depth=10,000), Prevalence filter (≥5%)
- 평가: DeLong 검정, McNemar 검정, Bootstrap CI (2,000회)

## 주요 결과
| 모델 | 개발 AUC | 외부 AUC |
|------|---------|--------|
| LR   | 0.997   | 0.864  |
| RF   | 0.907   | 0.802  |
| XGB  | **0.998** | **0.870** |

데이터 출처: [curatedMetagenomicData (Bioconductor)](https://bioconductor.org/packages/curatedMetagenomicData/)
