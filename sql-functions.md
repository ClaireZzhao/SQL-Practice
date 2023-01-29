- DATE functions
```sql
# DATE_ADD(기준날짜, INTERVAL)
select DATE_ADD(NOW(), INTERVAL 1 SECOND)
select DATE_ADD(NOW(), INTERVAL 1 MINUTE)
select DATE_ADD(NOW(), INTERVAL 1 HOUR)
select DATE_ADD(NOW(), INTERVAL 1 DAY)
select DATE_ADD(NOW(), INTERVAL 1 MONTH)
select DATE_ADD(NOW(), INTERVAL 1 YEAR)
select DATE_ADD(NOW(), INTERVAL -1 YEAR)

# DATE_SUB(기준날짜, INTERVAL)
select DATE_SUB(NOW(), INTERVAL 1 SECOND)
```


- like 연산자
```sql
select *
from table
where discount like '__\%' -- percent 표시하려면 \%
```

- 결과에 %를 붙이고 싶을때
```sql
concat(cast(sum(tip)*100 / sum(total_bill) as char), '%')
```

- pivot table
```sql
SELECT region AS Region
     , COUNT(DISTINCT CASE WHEN category = 'Furniture' THEN order_id END) AS Furniture
     , COUNT(DISTINCT CASE WHEN category = 'Office Supplies' THEN order_id END) AS "Office Supplies"
     , COUNT(DISTINCT CASE WHEN category = 'Technology' THEN order_id END) AS Technology
FROM records
GROUP BY Region
ORDER BY Region
```

- DML
```sql
INSERT INTO 테이블명 (Id, Salary) VALUES ('2', '550');

UPDATE 테이블명 SET 칼럼 = 값 WHERE 조건식; -- '=' 대입연산자
UPDATE 테이블명 SET 칼럼 = CASE WHEN id = 1 THEN '가'
                             WHEN id = 2 THEN '나'
                             WHEN id = 3 THEN '다'
                        ELSE '확인필요'
                        END;	
													
DELETE FROM 테이블명 WHERE 조건식;
# delete + subquery
DELETE 
FROM Person 
WHERE id not in (
    select sub.min_id 
    from (
        select email
             , min(id) as min_id
        from person 
        group by email
        ) sub
)
# delete + join 
delete t1, t2    # t1만 써도 됨
from t1 inner join t2 on t1.id = t2.ref
where t1.id = 1
```

- case when 절의 then 뒤에 여러 개의 컬럼을 한꺼번에 쓸 수는 없습니다. 이런 경우 문자열을 합쳐 하나의 값으로 만들어 주는 concat을 활용합니다.
```sql
count(distinct case when … then concat(user_pseudo_id, "-", ga_session_id) else …)
```
