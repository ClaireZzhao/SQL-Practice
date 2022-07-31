1. classic 리텐션: Day N 리텐션 (N일 뒤에 다시 돌아온 유저의 비율)
   - 계산법: classic 리텐션(Day N 리텐션) = D+N일 뒤에 방문한 사람 수 / D0에 방문한 사람 수
   - 단점: 일별 이벤트에 영향을 많이 받는다
        - D0 ~ D+N 사이에 여러본 오더라도 Day N 리텐션에 계산되지 않는다
        - 얼마나 자주 왔는지가 반영되지 않는다는 것이 큰 단점

2. range 리텐션: 다음 period에 다시 돌아온 유저의 비율, period의 일반적인 기준은 주 혹은 월
   - 계산법: range 리텐션 = next period에 방문한 사람 수 / 최초 period에 방문한 사람 수
   - 단점: period 기간만큼 시간이 지나야 지표를 확인할 수 있다
   - 유의할 점: period를 비즈니스에 맞게 정하는 것이 중요하다
        - 배달음식 - 7일을 period로 설정한다
        - 구독형식 - 30일로 retention range를 설정한다
   - 코호트 분석은 range 리텐션을 각각 산출한 버전이다
3. rolling 리텐션: 
   - 일정 기간 이후에 리턴한 유저의 비율
   - 몇 일이 지나도 여전히 살아있는 유저가 몇명이냐 하는 비율
   - 긴 관계를 유지하는 유저의 수를 판단하는 데 적합한 지표
   - 계산법: rolling 리텐션 = N일 이후 방문한 사람 수/D0에 방문한 사람 수
   - 장점: 이탈에 대한 정보를 얻을 수 있다 -> 아직 완전히 떨어져 나가지 않는 비율을 구한 것이 rolling 리텐션이기 때문임
   - 단점: 
     - 충성고객과 N일 이후 한번만 온 사람을 같게 취급한다
     - 원래는 오지 않았던 고객이 기간 후 오게 되면 리텐션에 카운트가 되게 된다
   - 그래서, 기존 리텐션 지표의 보조로 사용되는 경우가 많다.
 
 실습: rolling 리텐션 구하기 - 한 달이 지나도 여전히 살아 있는 고객은 몇프로 정보 되는가?
   - rolling 리텐션에서는 고객의 최초 구매 일자와 마지막 구매 일자가 필요하다.
   - 그 둘의 차이가 30일 rolling 리텐션 기준으로 30일보다 크냐 작냐를 따져보면 된다.
 ```sql
 select COUNT(customer_id) total_customer,
        COUNT(CASE WHEN diff_day >= 29 THEN 1 END) retention_customer,
        COUNT(CASE WHEN diff_day >= 29 THEN 1 END) / COUNT(customer_id) rolling_retention_rate
 from (select customer_id, 
              DATE(MIN(invoice_date)) first_purchase_date, 
              DATE(MAX(invoice_date)) recent_purchase_date,
              DATE_DIFF(DATE(MAX(invoice_date)), DATE(MIN(invoice_date)), DAY) diff_day
       from data.sales
       group by customer_id)
 ```
     
   

