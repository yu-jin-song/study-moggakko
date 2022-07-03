## 2022.06.26 일요일
### 공부한 내용
- 사이드 프로젝트
  + 로그인 구현
### 공유하고 싶은 내용
- Spring Security 
  + `WebSecurityConfigurerAdapter` deprecated
    - Spring Security 5.7.1 이상 또는 Spring Boot 2.7.0 이상 사용 시 IDEA에서 경고 출력
    - 조치
      + `WebSecurityConfigurerAdapter` 클래스의 메서드를 재정의하는 대신 `SecurityFilterChain` 및 `WebSecurityCustomizer` 빈 을 선언
    - 참고
      + https://spring.io/blog/2022/02/21/spring-security-without-the-websecurityconfigureradapter
      + https://www.codejava.net/frameworks/spring-boot/fix-websecurityconfigureradapter-deprecated
- DB 초기화 옵션
  + `jpa.hibernate.ddl-auto` vs `jpa.properties.hibernate.hbm2ddl.auto`
    - 동일한 옵션
    - properties를 통해 접근하면 다른 Hibernate 기본 속성과 함께 설정 가능

<br>

---

## 2022.06.25 토요일
### 공부한 내용
- 사이드 프로젝트
  + Spring Cloud
    - MSA의 개발, 배포, 운영에 필요한 아키텍처를 쉽게 구성할 수 있도록 지원하는 Spring Boot 기반 프레임워크
    - Eureka
      + MSA의 서비스들의 목록과 위치(IP, Port)가 동적으로 변화하는 환경에서 서비스들을 효율적으로 관리하기 위한 [Service Discovery](https://kobumddaring.tistory.com/44) Server/Client
### 공유하고 싶은 내용
- Spring cloud
  + https://honeywater97.tistory.com/205
- 유레카 클라이언트 활성화 어노테이션

  |항목|설명|
  |:---|:---|
  |**`@EnableEurekaClient`**|• `spring-cloud-commons` 기반<br>• 유레카 외에도 다른 클라이언트 구현체(consul, zookeeper) 등 지원|
  |**`@EnableDiscoveryClient`**|• `spring-cloud-netflix` 기반<br>• 유레카만 지원|

<br>

---

## 2022.06.19 일요일
### 공부한 내용
- velog 포스팅
    + it 용어 정리
- spring security
### 공유하고 싶은 내용
- 없음
<br>

---

## 2022.06.18 토요일
### 공부한 내용
- velog 포스팅
    + xshell 단축키 정리
- 사이드 프로젝트
    + 소셜 로그인 구현
### 공유하고 싶은 내용
- 없음
<br>

---

## 2022.06.12 일요일
### 공부한 내용
- velog 포스팅
    + .gitignore 정리
- 사이드 프로젝트
    + 요구사항 정의서 작성
    + 소셜 로그인 DB 설계
### 공유하고 싶은 내용
- postgresql의 serial type은 비표준 sql이므로 타 DB 마이그레이션 고려시 바람직하지 않음
    + 이 점을 보완한 `GENERATED AS IDENTITY` 타입을 사용 
<br>

---

## 2022.06.11 토요일
### 공부한 내용
- 사이드 프로젝트
    + sns 로그인 구현 공부
        - google
        - github
- velog 포스팅
    + git 명령어 정리
### 공유하고 싶은 내용
- 소셜 로그인 절차
    1. 소셜 로그인 버튼 클릭
    2. 소셜 로그인 페이지 이동
    3. 사용자 승인
    4. 로그인
    5. redirect url 비교
    6. 소셜서비스가 서비스 제공자에게 응답(데이터) 제공
    7. Authorization code, clientID, client secret, redirect URL 일치 확인
    8. Access Token 발급 
- google
    + api 인증 흐름
![google_oauth_api](https://user-images.githubusercontent.com/74666378/173169275-c9974900-d246-45bd-8969-3d21c40f62ab.png)
    + 사용자가 비공개한 정보는 받아올 수 없음(email, 이름 제외)
<br>

---

## 2022.06.05 일요일
### 공부한 내용
- 회사 업무 진행
    + 테이블 구조 수정
- 사이드 프로젝트
    + 화면 설계서 수정
### 공유하고 싶은 내용
- 없음
<br>

---

## 2022.06.04 토요일
### 공부한 내용
- 회사 업무 진행
    + 데이터베이스 다국어 지원
- 사이드 프로젝트
    + 화면 설계서 수정
### 공유하고 싶은 내용
- 없음
