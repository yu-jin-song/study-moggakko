# study-moggakko
### 📋 스터디 정보

- 장소 : 스타벅스 군자역점
- 시간 : 토,일 오전 10시 ~ 오후 12시
<br>

### 📋 규칙
1. 9시 55분까지 도착해주세요. 만약 늦을 것 같다면 미리 연락 주세요.
2. 지각 시 벌금 4,000원 입니다. (예정)
    - 스터디 몇 번 진행 후 도입
    - 단톡방 하나 파 모임통장 같은걸로 관리
3. 2시간 후 공부한 내용을 간단히 브리핑 합니다.
    - 스터디 종료하기 5분 전까지 본인이 공부한 내용 github에 정리하여 올리기
    - 같이 못 앉는 경우 카톡에 올리기
4. 한 달에 4번 불참 시 영구제명 됩니다.
    - 입원, 장례식, 컨디션 난조 등의 큰 일이 아닌 이상 스터디 전날까지 말하기
5. 대화명을 실명으로 바꿔주세요.
<br>

### 📋 github 이용 방법
- 리포지토리를 clone 받은 후 각자 사용할 디렉토리 생성
  - 디렉토리명 :: 본명 영어 소문자로(풀네임), 구분자는 `-` ex) song-yu-jin
- 본인 디렉토리 내에 파일 생성하여 올리기
    - 파일명 및 확장자 :: study-report-<월>.md ex) study-report-5.md
    - 형식 :: [template.md](https://github.com/yu-jin-song/study-moggakko/blob/master/template.md) 참고
    - 최신 내용이 최상단에 오게 작성
    - 달이 바뀔 때마다 md 새로 생성하여 올리기
- 다음 절차에 따라 push(필수)
  ``` shell
  $ git stash   # 커밋 충돌 막기 위함
  $ git pull
  $ git stash pop
  $ git add .     # add 안 된 상태일 경우 적용
  $ git commit -m "docs: update study report"
  $ git push <지정한 원격저장소명> master
  ```
