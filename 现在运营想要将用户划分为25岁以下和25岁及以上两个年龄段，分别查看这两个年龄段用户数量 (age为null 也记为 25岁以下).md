# 现在运营想要将用户划分为25岁以下和25岁及以上两个年龄段，分别查看这两个年龄段用户数量 (age为null 也记为 25岁以下)

```sql
select case when age < 25 or age is null then '25岁以下'
            when age >= 25 then '25岁及以上'
            end age_cut, count(*) number
from user_profile
group by age_cut 
```
