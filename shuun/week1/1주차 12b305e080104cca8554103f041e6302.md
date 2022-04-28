# 1주차

# 핵심 키워드 🎯

- 서버와 서비스
    
    서버: 서비스를 주는 객체
    
    클라이언트: 서비스를 받는 객체 
    
    서비스: 제공되는 것
    
- 클라이언트 - 서버 관계
    
    요청과 응답
    
    서버와 클라이언트는 1:N 구조로 연결되어 있음.
    
    서버: 통신망 상에서 다른 컴퓨터 대하여 회선, 디스크 장치 등에 대한 접속을 제어하는 관리 소프트웨어
     또는 컴퓨터를 말한다.
    
    - **[웹서버](http://wiki.hash.kr/index.php/%EC%9B%B9%EC%84%9C%EB%B2%84)**(web server) : [HTML](http://wiki.hash.kr/index.php/HTML)로 만든 웹 페이지가 들어 있는 파일을 사용자에게 제공하는 서버 프로그램이다. 대표적인 웹 서버 프로그램에는 [아파치](http://wiki.hash.kr/index.php/%EC%95%84%ED%8C%8C%EC%B9%98)(Apache), [IIS](http://wiki.hash.kr/index.php/IIS), [웹투비](http://wiki.hash.kr/index.php/%EC%9B%B9%ED%88%AC%EB%B9%84)(WebtoB), [웹티어](http://wiki.hash.kr/index.php/%EC%9B%B9%ED%8B%B0%EC%96%B4)(WebTier) 등이 있다.
    - **[와스서버](http://wiki.hash.kr/index.php?title=%EC%99%80%EC%8A%A4%EC%84%9C%EB%B2%84&action=edit&redlink=1)**(WAS) : Web Application Server의 약자로서, [자바](http://wiki.hash.kr/index.php/%EC%9E%90%EB%B0%94)(Java) 등으로 만든 웹 응용 프로그램이 설치되어 작동하는 웹 애플리케이션 서버를 말한다. 미들웨어의 일종이다. 대표적인 와스(WAS) 제품에는 [톰캣](http://wiki.hash.kr/index.php/%ED%86%B0%EC%BA%A3)(Tomcat), [제우스](http://wiki.hash.kr/index.php/%EC%A0%9C%EC%9A%B0%EC%8A%A4)(JEUS), [제이보스](http://wiki.hash.kr/index.php/%EC%A0%9C%EC%9D%B4%EB%B3%B4%EC%8A%A4)(JBoss), [웹로직](http://wiki.hash.kr/index.php/%EC%9B%B9%EB%A1%9C%EC%A7%81)(WebLogic), [웹스피어](http://wiki.hash.kr/index.php/%EC%9B%B9%EC%8A%A4%ED%94%BC%EC%96%B4)(WebSphere), [레진](http://wiki.hash.kr/index.php/%EB%A0%88%EC%A7%84)(Resin), [글래스피시](http://wiki.hash.kr/index.php/%EA%B8%80%EB%9E%98%EC%8A%A4%ED%94%BC%EC%8B%9C)(GlassFish) 등이 있다. 한국에서는 WAS라고 하지만, 영어권에서는 Application Server(약칭 AS)라고 한다.
        
        [[1]](http://wiki.hash.kr/index.php/%EC%84%9C%EB%B2%84-%ED%81%B4%EB%9D%BC%EC%9D%B4%EC%96%B8%ED%8A%B8#cite_note-1)
        
    - **[디비서버](http://wiki.hash.kr/index.php?title=%EB%94%94%EB%B9%84%EC%84%9C%EB%B2%84&action=edit&redlink=1)**(DB server) : Database Server의 약자로서, [데이터베이스](http://wiki.hash.kr/index.php/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4)(DB)를 저장 및 관리하는 서버를 말한다. [오라클](http://wiki.hash.kr/index.php/%EC%98%A4%EB%9D%BC%ED%81%B4_(%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4))(Oracle), [마이에스큐엘](http://wiki.hash.kr/index.php/%EB%A7%88%EC%9D%B4%EC%97%90%EC%8A%A4%ED%81%90%EC%97%98)(MySQL), [엠에스에스큐엘](http://wiki.hash.kr/index.php/%EC%97%A0%EC%97%90%EC%8A%A4%EC%97%90%EC%8A%A4%ED%81%90%EC%97%98)(MS-SQL), [큐브리드](http://wiki.hash.kr/index.php/%ED%81%90%EB%B8%8C%EB%A6%AC%EB%93%9C)(Cubrid) 등 다양한 [데이터베이스 관리 시스템](http://wiki.hash.kr/index.php/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4_%EA%B4%80%EB%A6%AC_%EC%8B%9C%EC%8A%A4%ED%85%9C)(DBMS)으로 만든 데이터가 저장·관리된다.
    
    클라이언트: 네트워크를 이용하여 서버 시스템에 연결된 pc나 스마트폰 등 디바이스 등 유저
    
- 서버의 동작 방식과 순서(요청이 들어왔을 때 서비스가 어떻게 처리되는가?)
    
    클라이언트가 request를 보내면 서버가 response하는 방식으로 처리됩니다.
    
    세부적으로 유저가 웹페이지에 주소를 입력하면, 웹페이지는 서버에 자료요청을 하고 서버는 웹페이지에 자료, 코드를 제공합니다. 그리고 웹페이지는 화면에 출력하여 유저에게 전달합니다.
    
- 서버의 구조
    - Server Program
        - 웹서버
            
            [웹 서버 - 위키백과, 우리 모두의 백과사전](https://ko.wikipedia.org/wiki/%EC%9B%B9_%EC%84%9C%EB%B2%84)
            
        - nginx
            
            엔진엑스(Nginx)는 Igor Sysoev라는 러시아 개발자가 `동시접속 처리에 특화된` 웹 서버 프로그램이다. `Apache`보다 동작이 단순하고, 전달자 역할만 하기 때문에 동시접속 처리에 특화되어 있다.
            
            동시접속자(약 700명) 이상이라면 서버를 증설하거나 Nginx 환경을 권장한다고 한다. 지금은 아파치가 시장 점유율이 압도적이지만, 아마존웹서비스(AWS) 상에서는 시장 점유율 44%에 달할정도로 가볍고, 성능이 좋은 엔진이라고 한다. (동시접속 처리에 특화)
            
        - apache
            
            [https://velog.io/@ksso730/Nginx-Apache-비교](https://velog.io/@ksso730/Nginx-Apache-%EB%B9%84%EA%B5%90)
            
        
        O Apache 는 Nginx 에 비해 모듈이 다양합니다.
        
        O Apache 의 안정성, 확장성, 호환성을 장점으로 들자면, Nginx 는 성능이 우세하다는 장점이 있습니다.
        
    - Back-end Language
        - java - spring, spring boot
        - javascript - node.js, express
        - python - django, flask
        
    - DB, DBMS
        - SQL
            
            Mysql
            
            mssql
            
            ORACLE
            
        - NoSQL
            
            MongoDB
            
            redis
            
            Cassandra
            
- APM
    
    APM의 A는 Application, 그중에서도 Web Application을 의미합니다. 즉 기업의 웹 서비스 성능을 관리하는 서비스를 APM이라고 합니다.
    
    APM의 P는 Performance, 애플리케이션의 성능을 의미합니다. 그리고 애플리케이션의 성능은 웹서비스의 응답속도를 통해 측정하게 됩니다. 웹서비스의 응답속도를 구하기 위해 APM 서비스는 트랜잭션을 추적하고 분석하는 일을 합니다.
    
    APM의 M은 Management 또는 Monitoring이 사용됩니다. 국내에서도 APM은 애플리케이션 성능 관리 또는 애플리케이션 성능 모니터링으로 불리고 있습니다. 성능을 향상시키는 관리의 의미를 강조할 경우에는 Management를 사용하고 단순 모니터링 의미를 강조할 경우에는 Monitoring이 사용됩니다.
    
    APM은 웹 서비스의 동작 상태를 관찰하고 성능을 분석하며, 특히 미들웨어(WebLogic, Tomcat, JBOSS 등)에서 일어나는 트랜잭션의 사용 시간을 분석하여 각 단계별로 성능에 영향을 미치는 원인을 분석할 수 있습니다.
    
    [https://www.whatap.io/ko/blog/19/](https://www.whatap.io/ko/blog/19/)
    
- 비트나미
    
    비트나미(Bitnami)는 가상 어플라이언스 및 웹 애플리케이션, 개발 스택용 소프트웨어 패키지 및 설치 라이브러리이다.
    
    - **WAMP**(Windows/Apache/MySQL/PHP)윈도우 환경에서 아파치(Server), MySQL(DB), PHP(서버사이드)와 같은 웹 개발환경을 통합적으로 구축해주는 프로그램
    - **MAMP**(Mac/Apache/MySQL/PHP)맥 환경에서 아파치(Server), MySQL(DB), PHP(서버사이드)와 같은 웹 개발환경을 통합적으로 구축해주는 프로그램
- 로컬호스트(localhost)
    
    **127.0.0.1**는
    
    자신의 컴퓨터를 가리키는 IPv4 IP주소로,
    
    자기 자신을 가리킨다고 해서, 루프백 (loopback) 주소라고도 불리는데요.
    
    보내면 자기 자신에게로 다시 돌아오기 때문입니다.
    
    **로컬호스트** (localhost)는 마찬가지로 자신의 컴퓨터를 가리키는 호스트이름 (hostname) / 도메인 입니다.
    
    Windows의 경우
    
    C:\windows\system32\drivers\etc\hosts
    
    여기 이 파일에 정의되어 있습니다.
    
    **[출처]** [[localhost/로컬호스트] 로컬호스트란?](https://blog.naver.com/dpdodpdjo/220897026370)|**작성자** [임글라스](https://blog.naver.com/dpdodpdjo)
    
- 가상머신(Virtual Machine)
    
    가상 머신은 물리적 컴퓨터와 동일한 기능을 제공하는 소프트웨어 컴퓨터입니다. 가상 머신은 물리적 컴퓨터처럼 애플리케이션과 운영 체제를 실행합니다. 그러나 가상 머신은 물리적 컴퓨터에서 실행되고 물리적 컴퓨터처럼 작동하는 컴퓨터 파일입니다. 다시 말해 가상 머신은 별도의 컴퓨터 시스템처럼 작동합니다.
    
    가상 머신은 바이러스에 감염된 데이터에 액세스하고 운영 체제를 테스트하는 등, 호스트 환경에서 수행하기에 위험한 특정 작업을 수행하기 위해 생성됩니다. 가상 머신은 다른 시스템에서 sandbox화되므로, 가상 머신 내의 소프트웨어는 호스트 컴퓨터를 변조할 수 없습니다. 가상 머신은 [서버 가상화](https://www.vmware.com/kr/topics/glossary/content/server-virtualization.html)
     등의 다른 목적으로도 사용할 수 있습니다.
    
    - Virtual Box
    - VMware
- Linux, Ubuntu
- 리눅스 명령어
    
    [[linux] 리눅스 기본 명령어/자주 쓰는 명령어](https://itholic.github.io/linux-basic-command/)
    
    [02. 꼭 알아야 할 리눅스 기본 명령어 10가지](https://gomguard.tistory.com/73)
    
    [리눅스 명령어 모음 BEST 50 초보자 및 전문가용 - 도라가이드](https://dora-guide.com/linux-commands/)
    
- 리눅스 디렉토리 구조
    
    [리눅스 디렉토리 구조](https://webdir.tistory.com/101)
    
- vi(vim) 편집기 사용법
    
    [[리눅스, 유닉스]vi (vim) 편집기 기본 사용법, 명령어, 단축키, 동작법 & 문제](https://jhnyang.tistory.com/54)
    

## 추가 개념 키워드

- Web Server(WS)와 Web Application Server(WAS)
    
    [[Web] 웹 서버와 WAS의 차이를 쉽게 알아보자](https://codechasseur.tistory.com/25)
    
    [WEB 서버와 WAS 서버의 차이](https://sungks.tistory.com/195)
    
    [{즉문즉설} WAS와 WS의 차이점은? (feat. Nginx, Node Express, Flask)](https://www.youtube.com/watch?v=6xl3wKMjmWg)
    
    [[10분 테코톡] 👩‍🦰희봉의 웹서버 vs WAS](https://www.youtube.com/watch?v=NyhbNtOq0Bc)
    
- 운영체제(OS)
    - 운영체제
        
        사용자가 쉽게 컴퓨터를 다룰 수 있게 해주는 인터페이스
        
        하드웨어 위에 커널(kernel)이 올라가고, 커널 위에서 셸(shell)과 애플리케이션(application)이 실행된다. 사용자는 기본적으로 셸을 통해 애플리케이션을 실행한다.
        
        ![Untitled](1%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%2012b305e080104cca8554103f041e6302/Untitled.png)
        
    - Window, MacOS
    
- CLI와 GUI
    - 인터페이스
    - GUI
    - CLI
- HTTP
- 패키지 설치와 컴파일 설치
    - 패키지 매니저
    - 컴파일 설치

# 1주차 수업 후기 📢

- 1주차 **수업을 듣고 서로 느낀 점을 이야기해주세요!**
- **핵심 키워드에 대해 완벽하게 이해했는지? 혹시 이해가 안 되는 부분은 뭐였는지?
서로 이야기해주세요!**

# !주의사항

1. **과제 피드백 기반 진행입니다** - 한명씩 본인의 **과제를 발표**하는 시간 그리고 해온 **과제에 대한 피드백**을 하는 시간 (ex:전 이렇게 생각해서 이런 부분 다르게 해왔는데 저것도 괜찮은 것 같아요!)이 **무조건 기반**이 되어야 합니다!
2. 부가적으로 **워크북에서 제공되는 키워드 혹은 강의에서 들은 디테일 적인 부분**에서 더 토의해봐도 좋을 것 같습니다

# 논의해보면 좋은 것들 🔥

### Warming Up

- 소통과 개발의 중요성
- 스스로를 소통이 잘되는 사람이라고 생각하는가? 이유는?
- 추가로 함께 일하고 싶은 개발자/사람의 특성은 무엇이 있을까요?

### Server

- 세상에는 어떤 종류의 서버스들이 있고 거기에 서버란 어떠한 것을 제공해줄까요?
- 본인이 만들고 싶은 서비스와 서버가 있나요? 있다면 무엇인가요?
- 본인이 생각하는 좋은 서버란? 좋은 서버가 갖추어야 하는 조건은 무엇인가요?
- 실습 과제를 수행하면서 배운 것들, 공유하면 좋은 것들

# 과제 파일 업로드

![Untitled](1%E1%84%8C%E1%85%AE%E1%84%8E%E1%85%A1%2012b305e080104cca8554103f041e6302/Untitled%201.png)