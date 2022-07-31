# 프랑스와 이탈리아의 코로나 신규감연자수 구하는 예시 (서브쿼리 + window function 사용)

```sql
select name, date, 每天新增治愈人数, rank()over(partition by name order by 每天新增治愈人数 desc) rk 
from (select name, date_format(whn, '%Y年%m月%d日') date, (recovered - lag(recovered, 1) over(partition by name order by whn)) 每天新增治愈人数 
      from covid where name in ('France', 'Italy')) re
order by rk
```
