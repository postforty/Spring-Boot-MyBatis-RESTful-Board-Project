## Spring Boot 웹 프로젝트 - RESTful 게시판 

+ 기술 스택
  + Framework: Spring Boot
    + Type: Gradle
    + Packaging: War(Web application Archive)
    + Java Version: 8
    + Language: Java
    + Dependencies
      + DevTools
      + MySQL
      + MyBatis
      + Thymeleaf
      + Web
      + Lombok
      + Logback
  + DB: MySQL 
  
+ 개발 내용
  + 게시글 목록 조회
  + 게시글 등록
  + 게시글 상세 화면
  + 게시글 수정
  + 게시글 삭제
  + 파일 첨부 및 다운로드
  + REST API
  
    |기능|REST|요청 방식|
    |---|---|---|
    |게시판 목록|/api/board|GET|
    |게시글 작성 화면|/api/board/write|GET|
    |게시글 작성|/api/board/write|POST|
    |게시글 상세 화면|/api/board/글번호|GET|
    |게시글 수정|/api/board/글번호|PUT|
    |게시글 삭제|/api/board/글번호|DELETE|
    |첨부파일 다운로드|/api/board/file?idx=파일번호&boardIdx=글번호|GET|
  
+ 성과
  + 데이터베이스 연동 관련 Hikari CP, MyBatis 사용
  + ***RESTful 게시판 구현***
  + PUT, DELETE 요청 방식을 사용하기 위해 HiddenHttpMethodFilter 등록(HTML에서는 PUT, DELETE 요청 방식을 지원하지 않기 때문)
  + ***REST API 개발***
  
+ 참고 자료
  + 김인우. (2019). 스프링 부트 시작하기. 프로그래밍인사이트
