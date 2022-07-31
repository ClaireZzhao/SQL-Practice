# 现在运营想要分别查看学校为山东大学或者性别为男性的用户的device_id、gender、age和gpa数据，请取出相应结果，结果不去重

```sql
select device_id, gender, age, gpa 
from user_profile 
where university = '山东大学'

union all

select device_id, gender, age, gpa 
from user_profile 
where  gender = 'male'
```
