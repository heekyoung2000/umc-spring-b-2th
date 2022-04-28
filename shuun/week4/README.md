# Server 4주차 워크북

# 핵심 키워드 🎯

- RDBMS
    - RDB
        
        관계형 데이터 베이스
        
        주로 2차원 데이터 베이스를 활용함
        
        key값과 value값을 메핑함
        
    - DBMS
        
        데이터 베이스 관리를 하는 시스템
        
    - NoSQL
        
        No SQL, Not Only SQL, Non-Relational Operational Database SQL
        
        ACID(Atomic, Consistency, Integrity, Duarabity)의 특성을 따르지 않는, 비관계형, 분산형 데이터들이 등장했다.
        
        인터넷 활성 및, SNS 등 비정형 데이터가 많아지면서 이러한 정보를 담을 수 있는 구조를 가진 데이터 베이스들이 각광받게 되었다.
        
        - 관계형 모델을 사용하지 않으며 테이블간의 조인 기능 없음
        - 직접 프로그래밍을 하는 등의 비SQL 인터페이스를 통한 데이터 액세스
        - 대부분 여러 대의 데이터베이스 서버를 묶어서(클러스터링) 하나의 데이터베이스를 구성
        - 관계형 데이터베이스에서는 지원하는 Data처리 완결성(Transaction ACID 지원) 미보장
        - 데이터의 스키마와 속성들을 다양하게 수용 및 동적 정의 (Schema-less)
        - 데이터베이스의 중단 없는 서비스와 자동 복구 기능지원
        - 다수가 Open Source로 제공
        - 확장성, 가용성, 높은 성능
        
        ex) 
        
        - Key Value DB
        
        Key와 Value의 쌍으로 데이터가 저장되는 가장 단순한 형태의 솔루션으로 Amazon의 Dynamo Paper에서 유래되었습니다. Riak, Vodemort, Tokyo 등의 제품이 많이 알려져 있습니다.
        
        - Wide Columnar Store
        
        Big Table DB라고도 하며, Google의 BigTable Paper에서 유래되었습니다. Key Value 에서 발전된 형태의 Column Family 데이터 모델을 사용하고 있고, HBase, Cassandra, ScyllaDB 등이 이에 해당합니다.
        
        - Document DB
        
        Lotus Notes에서 유래되었으며, JSON, XML과 같은 Collection 데이터 모델 구조를 채택하고 있습니다. MongoDB, CoughDB가 이 종류에 해당합니다.
        
        - Graph DB
        
        Euler & Graph Theory에서 유래한 DB입니다. Nodes, Relationship, Key-Value 데이터 모델을 채용하고 있습니다. Neo4J, OreientDB 등의 제품이 있습니다.
        
- SQL
    - DDL
    - DCL
    - TCL
    
    ![Untitled](Server%204%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%20%E1%84%8B%E1%85%AF%E1%84%8F%E1%85%B3%E1%84%87%E1%85%AE%E1%86%A8%2082c94eba03ef4b3a8ae7fe9530f41c38/Untitled.png)
    
- Database 용어
    - Table
    - Row
    - Column
    - Schema
    - Key
        
        
- 1:1 관계 / 1:N관계 / N:M관계

# 4주차 수업 후기 📢

- 4주차 **수업을 듣고 서로 느낀 점을 이야기해주세요!**
- **핵심 키워드에 대해 완벽하게 이해했는지? 혹시 이해가 안 되는 부분은 뭐였는지?
서로 이야기해주세요!**

### 📝 실습 체크리스트

- [x]  실습 1. 인스타그램 데이터베이스 설계
    - [x]  3단계에 맞춰서 데이터베이스 설계하기
        - [x]  시스템 분석
        - [x]  논리
        - [x]  물리

# !주의사항

1. **과제 피드백 기반 진행입니다** - 한명씩 본인의 **과제를 발표**하는 시간 그리고 해온 **과제에 대한 피드백**을 하는 시간 (ex:전 이렇게 생각해서 이런 부분 다르게 해왔는데 저것도 괜찮은 것 같아요!)이 **무조건 기반**이 되어야 합니다!
2. 부가적으로 **워크북에서 제공되는 키워드 혹은 강의에서 들은 디테일 적인 부분**에서 더 토의해봐도 좋을 것 같습니다

# 논의해보면 좋은 것들 🔥

- NoSQL의 종류
- MySQL을 제외한 RDBMS 종류

BigTable, Dynamo, Cassandra, CouchDB, MongoDB, Hbase, Riak, Voldemort

대표적인 **NoSQL**
로는 카산드라(Cassandra), HBASE, MongoDB가 있다. 일반 RDBMS 방식을 채택한 SQL 방식은 구조를 한 번 고정시키면, 데이터와 구조의 안정성은 보장된다. 일정한 형식을 유지해, 보기에도 편하고 훨씬 직관적이다

실제로 line이 nosql을 채택하고 비용절감을 많이함.

카톡은 mysql

Line → mongodb 

원래 nosql은 스키마로부터 자유로운데(변경이 용이), mongodb는 스키마를 지원함

누적되는 데이터가 많아지고 데이터베이스 관리가 어려워지고 연결관리가 어려워지면서 nosql사용이 증가

![Untitled](Server%204%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%20%E1%84%8B%E1%85%AF%E1%84%8F%E1%85%B3%E1%84%87%E1%85%AE%E1%86%A8%2082c94eba03ef4b3a8ae7fe9530f41c38/Untitled%201.png)

![Untitled](Server%204%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%20%E1%84%8B%E1%85%AF%E1%84%8F%E1%85%B3%E1%84%87%E1%85%AE%E1%86%A8%2082c94eba03ef4b3a8ae7fe9530f41c38/Untitled%202.png)

## 과제 제출

![Untitled](Server%204%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%20%E1%84%8B%E1%85%AF%E1%84%8F%E1%85%B3%E1%84%87%E1%85%AE%E1%86%A8%2082c94eba03ef4b3a8ae7fe9530f41c38/Untitled%203.png)