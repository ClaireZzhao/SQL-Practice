# 查询2020年饿了么平台上每个门店GMV最高那天的日期和GMV （window function）

```sql
select 门店名称, 日期, GMV 
from (select 门店名称, 日期, row_number() over(partition by 门店名称 order by GMV desc) r, GMV 
      from ddm.shop where substring(日期,1,4) = '2020' and 平台='eleme') a 
where a.r = 1
```
