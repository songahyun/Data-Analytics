## Data-Analytics: 정맥 카테터 재삽입 수술 예측 실험

※ This repository reorganizes my individual contributions from a team project conducted as part of a university course.  
※ 이 repository는 대학교 수업의 일환으로 진행된 팀 프로젝트에서 개인적으로 기여한 부분을 재정리한 것입니다.
___
### 프로젝트 배경:
정맥 카테터는 입원 환자의 수액 및 약물 투여를 위해 널리 사용되는 의료 처치이지만, 카테터의 폐색이나 감염, 위치 이상 등의 문제로 인해 재삽입이 필요한 경우가 빈번하게 발생한다. 정맥 카테터 재삽입은 환자에게 추가적인 통증과 불편을 유발할 뿐만 아니라 의료진의 업무 부담과 의료 자원의 소모를 증가시킬 수 있다. 그러나 재삽입 발생 여부를 사전에 판단하기 어려워 선제적인 관리가 이루어지기 힘든 한계가 있다. 따라서 환자의 임상 정보를 기반으로 정맥 카테터 재삽입 가능성을 예측하는 데이터 기반 접근이 필요하다.

### 프로젝트 목표:
- MIMIC-IV 데이터를 활용한 정맥 카테터 재삽입 예측 모델 개발
- 재삽입 발생에 영향을 미치는 주요 요인 분석
- 재삽입 위험 환자의 조기 식별 가능성 확보
- 의료진의 선제적 처치 및 관리 의사결정 지원
- 환자 불편 감소 및 의료 자원 활용 효율성 향상

### 사용 데이터:
- MIMIC-IV: 미국 보스턴의 Beth Israel Deaconess Medical Center(BIDMC)에서 수집된 중환자실 환자 데이터

___
### 프로젝트 소개: 
데이터 분석을 통해 30일 내 재입원 여부(카테터 재삽입 수술 진행 여부)를 예측하는 모델 개발  
프로젝트는 아래와 같은 조건들에 대해 진행됨.
1. 질병변수만 사용 vs 질병 변수와 환자 정보 변수 함께 사용
2. XGBoost vs Logistic Regression vs Random Forest
3. 아무것도 적용 안 함 vs SMOTE vs 클래스 가중치 기법 vs SMOTE와 클래스 가중치 모두 적용
4. 아무것도 적용 안함 vs 하이퍼파라미터 최적화(Hyprtopt, Optuna)
___
Individual Contribution
- 실험 코드 실행
- 클래스 불균형 완화 코드 개발(SMOTE, 클래스 가중치)
- 하이퍼파라미터 튜닝 코드 개발
- 모델 성능 평가
