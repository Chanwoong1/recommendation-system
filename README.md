# Recommendation Systems

## Outline

### Overview

Recommendation
- 어떤 조건에 적합한 대상을 책임지고 소개함

### Classification

- User data
  - Explicit Feedback
    - Rating
  - Implicit Feedback
    - View counts

- Model
  - Content-based Filtering
    - Recommendation based on item attribute
  - Collaboratice Filtering
    - Recommendation based on users' behavior
  - Hybrid Recommendation
    - Content based + Collaborative Filtering

- Purpose
  - Rating Prediction
    - Matrix Completion Problem
  - Top-K Recommandation

- Recommendation
  - Best Recommendation
  - Related Recommendation
  - Personalize Recommendation
  - Context-Aware Recommendation

### Performance

모델에 대한 성능 평가 단계
- 기존 모델 개선 및 신규 모델 개발 -> 이력 데이터 기반 성능 평가 -> 심사 평가 -> A/B Test -> 기존 모델 개선 및 신규 모델 개발
  - 사전 검증 : 이력 데이터 기반 성능 평가, 심사 평가
  - 사후 검증 : A/B Test

점수 예측에 대한 성능 평가 - 예상 평점과 실제 평점간 오차
- RMSE
  - 큰 오차에 큰 가중치, 작은 오차에는 작은 가중치 부여
- MAE
  - 오차만큼의 가중치 부여

Top-K 성능 평가 지표
- Precision@K
  - 모델이 추천한 K개 아이템 가운데 실제 유저가 관심있어하는 아이템의 비율
- Recall@K
  - 유저가 관심있어하는 전체 아이템 가운데 모델이 추천한 아이템의 비율
- MAP@K
  - Average Precision -> Precision(1) ~ Precision(K)까지의 평균값
  - 모든 유저에 대한 Average Precision 값의 평균 -> 추천시스템의 성능
- NDCG
  - 추천 순서에 따라 가중치가 부여된다. 1에 가까울수록 높은 성능
- DCG

### Considerations
