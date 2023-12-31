
```python

## Rubbing process (Rule-based systems using kurtosis and skewness)

1. Why? 러빙공정 불량 발생이 자주 일어나고 원인이 롤링 가속도에 있다는 것을 파악
   가속도 상승에 따른 러빙 vertical line 불량이 발생하게 되는점 발견 (원인: 베어링 불량)
   가속도 관리 모니터링 시스템 구축 프로젝트

2. 데이터: Acceleration time-series data
   - 'time', 'acceleration', 'pass/fail'

3. 접근: 가속도에 대한 데이터는 크게 two, 1)주파수 분석, 2)시계열 분석
   - 우리는 실시간 process이므로 시계열 선택

4. 정상과 불량 (Pass/fail)을 가장 잘 분리해주는 통게적 지표 선정필요
   why? interpretability: Summarize certain aspects of the distribution 
   - 선정 방법: 여러가지 있음 (peak, RMS, average)
     segmentation해서 여러 지표들이 pass/fail을 잘 구분하는지 plot 그려봄 (아래와 같이)
   - Segmentation 방법: (가속도에 Absolute value and Averaging time 0.5s term)
   - Plot 예시: Sknewness & Kurtosis (NOR, IRF, ORF : Inner & Outer Race Fault)
```
   ![Image 2024-01-04 at 11 26 AM](https://github.com/scottmsoh/ref_industry/assets/112598791/688a0895-7d88-429e-a670-18a3380791ec)

```python
   - Anova 등 (R square value) 검증 통해 신뢰성 검증

5. Database에 실시간 적재 가능하도록

6. ML 모델 (예측모델 개발)
   - 입력: 'skewness', 'kurtosis', Label: NOR, IRF, ORF
   - Classifier 모델: ANN (Layer, node), SVM, Logistic
   - Confusion matrix (Accuracy, F1-score)
   - RMSE, R square,
   - Cross-validation
   - 모델 output: p

7. Rule-based systems VS ML prediction Model 
   Choosing: Rule-based systems
   Efficiency: the rule-based system is computationally less expensive and provides       
               sufficient performance
   ML model: Complementary Use (providing a secondary check)

8. Python GUI 
```

![Image 2024-01-04 at 12 34 PM](https://github.com/scottmsoh/ref_industry/assets/112598791/6734f9a6-e27a-450b-ab41-e22b1350b6f5)

![Image 2024-01-04 at 1 04 PM](https://github.com/scottmsoh/ref_industry/assets/112598791/364f4bb3-f605-4fd0-9884-06b8c1ba17ec)

![Image 2024-01-04 at 1 04 PM](https://github.com/scottmsoh/ref_industry/assets/112598791/f8e35b5b-0f2e-4700-b554-ee91e1f40896)


