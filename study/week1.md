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
> ***데이터 웨어하우스***
    데이터를 한 곳에 모아서 저장
    여러곳에 저장된 데이터 예시 (Database, 웹, 파일 api 결과 등)
