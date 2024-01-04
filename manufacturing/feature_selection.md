
```python

## Feature_selection

1. 개요 및 Goal
   - 연중 발생하는 고질불량에 대한 개선을 위해 6개월 치 데이터를 활용해 특정 요소를 발견하고자 함.

2. Dataset
   - 2016.06~2016.12 'time', '1'~'589':variable, 'Pass/fail'

3. Classification cases

4. Data exploration
   - Check NaN, 0, outlier, shape 확인
   - Multicollinearity (변수 많으니 상관석 분석하여 상관관계 큰 것은 삭제 필요)
     But 어떤것을 삭제할지 도메인지식, feature삭제 후 모델 검증통해 유무에 따른 perforamnce 확인필요)
     (confusion matrix:accuracy, F1-score, R square, RMSE)

5. 모델: SVM, XGBoost, Regressor classifier

6. Hyper parameter tune (XGBoost):
   - Grid search & Random Search

7. Confusion matrix
   - Accuracy, F1-score, R square, RMSE

8. Sampling method
    - Undersample & Oversample, but in this case oversampling is better

9. PCA (Dimension reduction)
    - But not out-perform

10. Feature selection (from XGBoost feature importance)
    - 4 features are most important to specify the fail case

```
