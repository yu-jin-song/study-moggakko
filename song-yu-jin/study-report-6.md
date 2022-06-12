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