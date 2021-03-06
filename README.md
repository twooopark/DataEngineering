# DataEngineering
Data Engineering

---
## 학습 

1. 실습할 VM, OS, DBMS 툴 선택(간단한 비교)

	- VirtualBox, VMware, Hyper-V 비교
		
		- 디스크 IO 성능 : Hyper-V 
		
		- 편의성(다중 스냅샷, 디스크 관리 등) : VMware
	
	
	- CentOS, Ubuntu 비교(방화벽 등)
	
		- CentOS7
	
	- Mysql, Mssql 비교(엔진, 복제 등)
  
---

2. 선택한 툴 설치 & 테스트

	- VM1, VM2 각각 HostPC(Win)와 데이터 송수신 테스트
 
	- VM1, VM2 데이터 송수신 테스트
 
	- VM1 -> VM2 데이터 복제
 	
---	

3. 데이터베이스에 대한 이해

	- 여러 복제 방식
	
	- SQL문 이해
	
		- DDL : 정의어
	
		- DML : 조작어
	
		- 쿼리 성능 향상법, 집합 처리
	
		- 서버에 대한 옵션을 통한 성능 향상
	
		- SQL문을 통한 성능 향상(인덱스, 프로시저)
	
	- OLTP, ETL, DW, DM, OLAP
		
		- OLTP(Online transaction processing, OLTP) : 컴퓨터 시스템을 사용하는 트랜잭션 데이터 관리
		
		- ETL : 다양한 원본에서 데이터를 수집하고, 비즈니스 규칙에 따라 데이터를 변환하고, 대상 데이터 저장소로 로드하는 데 사용되는 데이터 파이프라인
		
		- DW : 수년간 발생한 데이터를 분석할 수 있게 하는 통합 시스템, 통합된 데이터의 조직적인 중앙 관계형 리포지토리
		
		- DM : 좀 더 작고 좀 더 특정 영역을 중심으로 하는 데이터 웨어하우스
		
		- OLAP : 데이터를 분석해서 의미있는 형태로 만들기 위한 과정 및 도구.
		
		- https://docs.microsoft.com/ko-kr/azure/architecture/data-guide/relational-data/online-transaction-processing
	
	- 데이터 큐브
		
		- 기존의 2차원인 데이터 테이블 구조를 다차원의 속성으로 표현
	
	
---

4. 데이터 관리(Google Cloud Platform)
	
	- 데이터 분석

		- BigQuery
		
			- 머신러닝이 내장된 확장성이 우수한 완전 관리형 클라우드 데이터 웨어하우스(기업용 서버리스 DW)

			- BigQuery의 관리형 열 형식 저장소, Cloud Storage, Cloud Bigtable, 스프레드시트, 드라이브에 저장된 데이터를 쿼리

			- 특징
				- NoOps / SQL / Replica / StreamInput 

				- Hadoop, Spark 등의 설치& 클러스터 유지 보수 등의 요구인력 절감

				- No-Key, No-Index(Full SCAN ONLY)

				- No update&delete row

				- eventual consistency

			- 출처: http://bcho.tistory.com/1116 [조대협의 블로그]
		
		- Cloud Dataflow
			
			- 스트림(실시간) 및 기록 모드에서 데이터를 변환하고 강화하는 전체 관리형 서비스
			
			- Apache Beam SDK에서 표현식을 사용하는 자바 및 Python API를 통해 빠르고 단순한 파이프라인 개발을 지원
	
	- 저장소
	
		- Cloud Storage
		
			- 개발자와 기업을 위한 통합 객체 저장소
			
			- 객체 수명 주기 관리 기능
		
			- 용도 예시
			
				- 웹사이트 콘텐츠를 제공
				
				- 보관 및 재해 복구를 위해 데이터를 저장
				
				- 직접 다운로드를 통해 사용자에게 대량의 데이터 객체를 배포
				
			- https://cloud.google.com/storage/
	
	- 데이터베이스
	
		- Cloud SQL
			
			- MySQL 및 PostgreSQL 데이터베이스 서비스
			
			- https://cloud.google.com/sql/
		
		- Cloud Bigtable
		
			- NoSQL 와이드 컬럼 데이터베이스 서비스
			
			- https://cloud.google.com/bigtable/
		
		- Firebase
			- Firebase 실시간 데이터베이스, 서버리스 앱 개발에 사용
			
			- https://firebase.google.com/products/realtime-database/
	

	- 로그 수집을 위한 ETL Tool 비교
	
		- Pentaho Data Integration (Hitachi Vantara)
			
		- Talend Open Studio (Talend)
		
		- PowerCenter (Informatica)
		
		- https://www.etltool.com/list-of-etl-tools/
				
---

5. Data Engineering?
	
	- 정의

6. Data Pipeline?

	- 정의
	
	- 구조 예시
		
		- 구조별 특징, 장단점, 사용예시
		
		- Hadoop Eco, Elastic Stack, GCP 등

7. 5, 6번을 주제로 발표

	- 10/05 목차 검토 

	- 10/12 발표

