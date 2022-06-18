## 2022.06.18 토요일
### 공부한 내용
#### 학급일지 프로젝트 작업 

##### context-API를 활용 theme 변경 기능 구현
      - redux 와 context-API의 차이 
        + redux 는 store 하나만으로 여러 state를 관리 할 수 있다. 때문에 각 상태별로 Provider를 생성해서 사용하는 context-API에 비해 코드가 간결해진다. 하지만 provider를 활용해서 명시적으로 상태관리를 표시 해 주기 위해 redux를 활용하는 것 보다 context-API를 활용하는 것이 더 좋은 상황도 있다.
        + redux 에서 redux-devtool-extension 을 활 상태 관리 디버깅이 쉬워진다.
        + 다양한 미들웨어(thunk, saga) 를 추가적으로 활용할 수 있다.
      - context-API를 활용한 이유
        + 현재 진행한 프로젝트에서 redux를 활용하여 theme 상태관리와 이벤트 처리를 하는것 보다 context-API를 활용 하는 것이 코드 가독성이 더 좋다고 판단되어 context-API를 활용하기로 했다.
### 공유하고 싶은 내용
- react를 활용하는 이유 와 front-end가 어떤 일을 하는지
<br>