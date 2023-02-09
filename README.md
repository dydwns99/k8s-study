# 📖 K8S - study 실습용 프로젝트

---
✏️ 설명


- 본 프로젝트는 쿠버네티스 스터디 실습에 사용하기 위한 프로젝트 입니다.

- spring boot 를 사용하여 '회원등록' 과 '회원조회' 을 할 수 있는 웹페이지를 간단하게 구현하였습니다.

---
🐳 도커 컨테이너로 실행하는 방법

1. zip 파일을 풀어서 프로젝트를 연다. 

- [ 완성 후 해당 spring프로젝트를 zip파일로 묶어서 commit할 예정 ]
- [ 추가로 ./src/main/resources/application.properties 파일에서 spring.datasource.url의 값을 h2 실행시 jdbc url과 일치 시킨다.]


2. H2 데이터베이스를 실행한다. 
- [ 추후에 h2 설치 방법 공개]


3. docker build --build-arg JAR_FILE=build/libs/business-spring-0.0.1-SNAPSHOT.jar -t myorg/myapp --platform linux/amd64 . 입력


4. docker run -p 8080:8080 myorg/myapp 입력

---
🛠️ 적용기술

- Spring Boot

- H2 데이터베이스

- JPA