
## Rubbing process

1. Why? 러빙공정 불량 발생이 자주 일어나고 원인이 롤링 가속도에 있다는 것을 파악
   가속도 상승에 따른 러빙 vertical line 불량이 발생하게 되는점 발견 (원인: 베어링 불량)
   가속도 관리 모니터링 시스템 구축 프로젝트
2. 데이터: Acceleration time-series data
3. 접근: 가속도에 대한 데이터는 크게 two, 1)주파수 분석, 2)시계열 분석
   - 우리는 실시간 process이므로 시계열 선택
4. 정상과 불량 (Pass/fail)을 가장 잘 분리해주는 통게적 지표 선정필요
   - 가속도에 Absolute value and Averaging time 0.5s term
   - Sknewness & Kurtosis (NOR, IRF, ORF : Inner & Outer Race Fault)
   ![Image 2024-01-04 at 11 26 AM](https://github.com/scottmsoh/ref_industry/assets/112598791/688a0895-7d88-429e-a670-18a3380791ec)

   - Anova 등 (R square value) 검증 통해 신뢰성 검증
   - 
