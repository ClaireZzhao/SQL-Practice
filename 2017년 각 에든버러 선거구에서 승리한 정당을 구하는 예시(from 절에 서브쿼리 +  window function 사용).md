# 2017년 각 에든버러 선거구에서 승리한 정당을 구하는 예시(from 절에 서브쿼리 +  window function 사용)

<aside>
👉 승리한 정당: 득표수가 가장 높은 정당

</aside>

```sql
select constituency, party 
from (select constituency, 
             party, 
             votes, 
             rank()over(partition by constituency order by votes desc) rk 
             from ge 
             where yr = 2017 and 
             constituency between 'S14000021' and 'S14000026') as new 
where new.rk = 1
```
