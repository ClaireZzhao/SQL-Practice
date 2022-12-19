```sql
select d.order_date dt
     , count(distinct d.customer_id) dau 
     , count(distinct w.customer_id) wau
    ,  round(count(distinct d.customer_id)/count(distinct w.customer_id), 2) stickiness
from records d 
    left join records w on w.order_date between date_add(d.order_date, interval -6 day) and d.order_date 
where d.order_date between '2020-11-01' and '2020-11-30' 
group by dt
having dau > 0
order by dt
```
