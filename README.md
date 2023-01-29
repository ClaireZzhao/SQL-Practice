# SQL-Practice
SQL 연습 레포지토리

## Query 문법
### [DATE 함수](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### [like 연산자](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### [결과에 %를 붙이고 싶을때](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### [pivot table](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### [DML](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### not in
- [모든 나라의 인구수가 25000000보다 적은 대륙을 구하는 예시](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EB%AA%A8%EB%93%A0%20%EB%82%98%EB%9D%BC%EC%9D%98%20%EC%9D%B8%EA%B5%AC%EC%88%98%EA%B0%80%2025000000%EB%B3%B4%EB%8B%A4%20%EC%A0%81%EC%9D%80%20%EB%8C%80%EB%A5%99%EC%9D%84%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%98%88%EC%8B%9C%20(not%20in%20%EC%82%AC%EC%9A%A9).md)

### substring_index
- [现在运营想要统计每个性别的用户分别有多少参赛者，请取出相应结果](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E7%8E%B0%E5%9C%A8%E8%BF%90%E8%90%A5%E6%83%B3%E8%A6%81%E7%BB%9F%E8%AE%A1%E6%AF%8F%E4%B8%AA%E6%80%A7%E5%88%AB%E7%9A%84%E7%94%A8%E6%88%B7%E5%88%86%E5%88%AB%E6%9C%89%E5%A4%9A%E5%B0%91%E5%8F%82%E8%B5%9B%E8%80%85%EF%BC%8C%E8%AF%B7%E5%8F%96%E5%87%BA%E7%9B%B8%E5%BA%94%E7%BB%93%E6%9E%9C.md)
- [每个年龄的用户分别有多少参赛者](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E6%AF%8F%E4%B8%AA%E5%B9%B4%E9%BE%84%E7%9A%84%E7%94%A8%E6%88%B7%E5%88%86%E5%88%AB%E6%9C%89%E5%A4%9A%E5%B0%91%E5%8F%82%E8%B5%9B%E8%80%85.md)

### group by
- [现在运营想要将用户划分为25岁以下和25岁及以上两个年龄段，分别查看这两个年龄段用户数量 (age为null 也记为 25岁以下)](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E7%8E%B0%E5%9C%A8%E8%BF%90%E8%90%A5%E6%83%B3%E8%A6%81%E5%B0%86%E7%94%A8%E6%88%B7%E5%88%92%E5%88%86%E4%B8%BA25%E5%B2%81%E4%BB%A5%E4%B8%8B%E5%92%8C25%E5%B2%81%E5%8F%8A%E4%BB%A5%E4%B8%8A%E4%B8%A4%E4%B8%AA%E5%B9%B4%E9%BE%84%E6%AE%B5%EF%BC%8C%E5%88%86%E5%88%AB%E6%9F%A5%E7%9C%8B%E8%BF%99%E4%B8%A4%E4%B8%AA%E5%B9%B4%E9%BE%84%E6%AE%B5%E7%94%A8%E6%88%B7%E6%95%B0%E9%87%8F%20(age%E4%B8%BAnull%20%E4%B9%9F%E8%AE%B0%E4%B8%BA%2025%E5%B2%81%E4%BB%A5%E4%B8%8B).md)
- [现在运营想要统计每个性别的用户分别有多少参赛者，请取出相应结果](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E7%8E%B0%E5%9C%A8%E8%BF%90%E8%90%A5%E6%83%B3%E8%A6%81%E7%BB%9F%E8%AE%A1%E6%AF%8F%E4%B8%AA%E6%80%A7%E5%88%AB%E7%9A%84%E7%94%A8%E6%88%B7%E5%88%86%E5%88%AB%E6%9C%89%E5%A4%9A%E5%B0%91%E5%8F%82%E8%B5%9B%E8%80%85%EF%BC%8C%E8%AF%B7%E5%8F%96%E5%87%BA%E7%9B%B8%E5%BA%94%E7%BB%93%E6%9E%9C.md)

### union all
- [现在运营想要分别查看学校为山东大学或者性别为男性的用户的device_id、gender、age和gpa数据，请取出相应结果，结果不去重](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E7%8E%B0%E5%9C%A8%E8%BF%90%E8%90%A5%E6%83%B3%E8%A6%81%E5%88%86%E5%88%AB%E6%9F%A5%E7%9C%8B%E5%AD%A6%E6%A0%A1%E4%B8%BA%E5%B1%B1%E4%B8%9C%E5%A4%A7%E5%AD%A6%E6%88%96%E8%80%85%E6%80%A7%E5%88%AB%E4%B8%BA%E7%94%B7%E6%80%A7%E7%9A%84%E7%94%A8%E6%88%B7%E7%9A%84device_id%E3%80%81gender%E3%80%81age%E5%92%8Cgpa%E6%95%B0%E6%8D%AE%EF%BC%8C%E8%AF%B7%E5%8F%96%E5%87%BA%E7%9B%B8%E5%BA%94%E7%BB%93%E6%9E%9C%EF%BC%8C%E7%BB%93%E6%9E%9C%E4%B8%8D%E5%8E%BB%E9%87%8D.md)

### sub query
- [2017년 각 에든버러 선거구에서 승리한 정당을 구하는 예시](https://github.com/ClaireZzhao/SQL-Practice/blob/main/2017%EB%85%84%20%EA%B0%81%20%EC%97%90%EB%93%A0%EB%B2%84%EB%9F%AC%20%EC%84%A0%EA%B1%B0%EA%B5%AC%EC%97%90%EC%84%9C%20%EC%8A%B9%EB%A6%AC%ED%95%9C%20%EC%A0%95%EB%8B%B9%EC%9D%84%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%98%88%EC%8B%9C(from%20%EC%A0%88%EC%97%90%20%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC%20%2B%20%20window%20function%20%EC%82%AC%EC%9A%A9).md)
- [프랑스와 이탈리아의 코로나 신규감연자수 구하는 예시](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%ED%94%84%EB%9E%91%EC%8A%A4%EC%99%80%20%EC%9D%B4%ED%83%88%EB%A6%AC%EC%95%84%EC%9D%98%20%EC%BD%94%EB%A1%9C%EB%82%98%20%EC%8B%A0%EA%B7%9C%EA%B0%90%EC%97%B0%EC%9E%90%EC%88%98%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%98%88%EC%8B%9C%20(%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC%20%2B%20window%20function%20%EC%82%AC%EC%9A%A9).md)

### window function
- [누적합 구하기](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EB%88%84%EC%A0%81%ED%95%A9%20%EA%B5%AC%ED%95%98%EA%B8%B0.md)
- [2017년 각 에든버러 선거구에서 승리한 정당을 구하는 예시](https://github.com/ClaireZzhao/SQL-Practice/blob/main/2017%EB%85%84%20%EA%B0%81%20%EC%97%90%EB%93%A0%EB%B2%84%EB%9F%AC%20%EC%84%A0%EA%B1%B0%EA%B5%AC%EC%97%90%EC%84%9C%20%EC%8A%B9%EB%A6%AC%ED%95%9C%20%EC%A0%95%EB%8B%B9%EC%9D%84%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%98%88%EC%8B%9C(from%20%EC%A0%88%EC%97%90%20%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC%20%2B%20%20window%20function%20%EC%82%AC%EC%9A%A9).md)
- [查询2020年饿了么平台上每个门店GMV最高那天的日期和GMV](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E6%9F%A5%E8%AF%A22020%E5%B9%B4%E9%A5%BF%E4%BA%86%E4%B9%88%E5%B9%B3%E5%8F%B0%E4%B8%8A%E6%AF%8F%E4%B8%AA%E9%97%A8%E5%BA%97GMV%E6%9C%80%E9%AB%98%E9%82%A3%E5%A4%A9%E7%9A%84%E6%97%A5%E6%9C%9F%E5%92%8CGMV%20%EF%BC%88window%20function.md)
- [프랑스와 이탈리아의 코로나 신규감연자수 구하는 예시](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%ED%94%84%EB%9E%91%EC%8A%A4%EC%99%80%20%EC%9D%B4%ED%83%88%EB%A6%AC%EC%95%84%EC%9D%98%20%EC%BD%94%EB%A1%9C%EB%82%98%20%EC%8B%A0%EA%B7%9C%EA%B0%90%EC%97%B0%EC%9E%90%EC%88%98%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%98%88%EC%8B%9C%20(%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC%20%2B%20window%20function%20%EC%82%AC%EC%9A%A9).md)

### case when
- [复旦大学每个用户8月份答题情况](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%E5%A4%8D%E6%97%A6%E5%A4%A7%E5%AD%A6%E6%AF%8F%E4%B8%AA%E7%94%A8%E6%88%B78%E6%9C%88%E4%BB%BD%E7%BB%83%E4%B9%A0%E6%83%85%E5%86%B5.md)
- [case when 절의 then 뒤에 여러 개의 컬럼을 한꺼번에 쓸 수는 없습니다. 이런 경우 문자열을 합쳐 하나의 값으로 만들어 주는 concat을 활용합니다.](https://github.com/ClaireZzhao/SQL-Practice/blob/main/sql-functions.md)

### 사용자정의함수 
- [사용자정의함수+limit사용법](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EC%82%AC%EC%9A%A9%EC%9E%90%EC%A0%95%EC%9D%98%ED%95%A8%EC%88%98.md)

## 분석 기법

### 리텐션

클래식 리텐션 vs 롤링 리텐션
- 클래식 리텐션: 구매주기가 긴 서비스에서는 클래식 리텐션을 사용하면 실제보다 많이 이탈했다고 잘못 이해할 수 있음 -> [클래식 리텐션](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%ED%81%B4%EB%9E%98%EC%8B%9D%20%EB%A6%AC%ED%85%90%EC%85%98.md)
- 롤링 리텐션: 최근 코호트일수록 리텐션 값이 낮게 계산되고, 이전 코호트일수록 리텐션 값이 올라갈 수밖에 없음, 다른 코호트(1월과 11월을 비교한다든지)와 단순 비교해서 보기가 어려움 (나중에라도 결제를 했으면 그 전 달에도 결재했다고 간주하기 때문) `숫자가 계속 바뀌기 때문에 보고용으로 적합하지 않을 수 있음` -> [롤링 리텐션](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EB%A1%A4%EB%A7%81%20%EB%A6%AC%ED%85%90%EC%85%98.md)

- [리텐션 계산법 정리(sql코드포함)](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EB%A6%AC%ED%85%90%EC%85%98%20%EA%B3%84%EC%82%B0%EB%B2%95(%EB%A1%A4%EB%A7%81%EB%A6%AC%ED%85%90%EC%85%98%EC%8B%A4%EC%8A%B5%ED%8F%AC%ED%95%A8).md)
- [코호트 분석(sql코드포함)](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EC%BD%94%ED%98%B8%ED%8A%B8%EB%B6%84%EC%84%9D.md)
- [퍼널분석 계산법(sql코드포함)](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%ED%8D%BC%EB%84%90%EB%B6%84%EC%84%9D%EA%B3%84%EC%82%B0%EB%B2%95.md)
- [다음날 리텐션 분석](https://github.com/ClaireZzhao/SQL-Practice/blob/main/%EB%8B%A4%EC%9D%8C%EB%82%A0%20%EB%A6%AC%ED%85%90%EC%85%98%20%EA%B5%AC%ED%95%98%EA%B8%B0.md)

### Stickiness
- [Stickiness](https://github.com/ClaireZzhao/SQL-Practice/blob/main/Stickiness.md) -> 우리 서비스에 딱 붙어있는지 측정하는 지표 -> WAU/MAU와 DAU를 함께 본다면 WAU/MAU만 볼 때 알 수 없었던 고객들의 방문 패턴을 알 수 있음
