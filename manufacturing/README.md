
전처리
시각화 (인사이트) - 가설 세움 (검증 어려움)
파생 변수 (계측오류 별도 변수로 생성- key feature라고 생각)
주기?? 몇초로 줄지
데이터 불균형; 8:2

이상치 감지
오토엠엘
딥러닝 시계열

검증데이터

*모델
LSTM
CNN_LSTM
따로? 앙상블?: LSTM에 CNN 계층을 추가하는 방식으로 진행
선행연구 없었음

시계열 
이상치 탐지
오토엠엘

보고서
소스코드 통합
발표자료 준비


-- 에너지
발전량 예측, 고장진단
예측값 20~30% 벗어난 것들은 고장으로 진단되지 않을까함

도메인 지식으로의 포트폴리오 작성

스마트폰 아이폰의 핵심모듈인 카메라 샌싱모듈, 
사랑하눈
실시간 설비 고장진단

*JMP 기반 통계적 성능지표 선정 - 가속도 데이터 들어오면 주파수, 시계열 분석(빠르게) 가능
통계적 지표 kurtosis, skewness 
Neural network과 SVM 모델링 구축


머신러닝 기반 모니터링 시스템 구축
롤러 (러빙공정) 가속도 데이터 -> skewness & Kurtosis 데이터 계산 --> Database에 축적(MES, EAS) 조회가능
SQLite--> Python, JSL GUI로 구축

skewness & Kurtosis : RMSE, MSE와 같이 모델 성능 Accuracy나타내는 지표임
롤러베어링 가속도 신호에 절대값을 취하고 0.5초 단위로 AVG 계산 :정상(NOR), 불량(IRF, ORF) inner & outer
Anova 분석 -> 차이가 있나 (유의차)
패턴을 정확하게 분리해낼수 있다

JMP graph builder로 확률이 어떤 패턴을 가지고 있고, 이런 형태로 보여줄수 있다.

I need to get skewness and Kurtosis data from acceleration values in some manufacturing processes. How can I get this? The dataset contains acceleration values and time-series data.






