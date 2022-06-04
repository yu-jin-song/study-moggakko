# study-moggakko
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
