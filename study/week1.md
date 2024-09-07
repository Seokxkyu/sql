# SQL Assignment Week 1


## 1. BigQuery 기초 지식
데이터베이스 : 데이터의 저장소<br>
테이블: 데이터가 저장된 공간<br>
저장된 데이터를 제품에서 사용

### OLTP
- Online Transaction Processing
- 거래를 하기 위해 사용되는 데이터베이스
- 보류, 중간 상태가 없음
- 데이터의 추가(INSERT), 변경(UPDATE) 많이 발생 
- SQL 사용해 데이터 추출할 수 있으나, 분석을 위해 만든 데이터베이스가 아니라 쿼리 속도가 느릴 수 있음

### SQL
- Structured Query Language
- 데이터베이스에서 데이터를 가지고 올 때 사용하는 언어
- 데이터베이스의 데이터를 관리하기 위해 설계된 특수 목적의 프로그래밍 언어

### OLAP
- OLTP로 데이터 분석을 하다가 속도, 기능 부족의 이슈로 OLAP 등장
- ***OLAP***: Online Analytical Processing
> ***데이터 웨어하우스***<br>
    데이터를 한 곳에 모아서 저장<br>
    여러곳에 저장된 데이터 예시 (Database, 웹, 파일 api 결과 등)

### BigQuery
Google Cloud의 OLAP + Data Warehouse

***장점***
1. 난이도<br>
SQL을 사용해 쉽게 데이터 추출 가능
2. 속도<br>
OLAP 도구이므로 속도가 빠름
3. Firebase, Google Analytics 4의 데이터를 쉽게 추출할 수 있음<br>
사용 기기, 위치, OS 버전, 이벤트 행동 획득 가능 (별도의 로깅 필요)
4. 데이터 웨어하우스를 사용하기 위해 서버 (컴퓨터)를 띄울 필요 없음<br>
구글에서 인프라 관리

### Big Query 사용하는 이유
- 회사에서 앱이나 웹에서 Firebase, Google Analytics 4를 활용할 경우
- 운영을 적은 비용으로 진행하기 위해 