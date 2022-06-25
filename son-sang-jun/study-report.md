## 2022.06.18 토요일
### 공부한 내용
> 학급일지 프로젝트 작업 

1. context-API를 활용 theme 변경 기능 구현
      - redux 와 context-API의 차이 
        + redux 는 store 하나만으로 여러 state를 관리 할 수 있다. 때문에 각 상태별로 Provider를 생성해서 사용하는 context-API에 비해 코드가 간결해진다. 하지만 provider를 활용해서 명시적으로 상태관리를 표시 해 주기 위해 redux를 활용하는 것 보다 context-API를 활용하는 것이 더 좋은 상황도 있다.
        + redux 에서 redux-devtool-extension 을 활 상태 관리 디버깅이 쉬워진다.
        + 다양한 미들웨어(thunk, saga) 를 추가적으로 활용할 수 있다.
      - context-API를 활용한 이유
        + 현재 진행한 프로젝트에서 redux를 활용하여 theme 상태관리와 이벤트 처리를 하는것 보다 context-API를 활용 하는 것이 코드 가독성이 더 좋다고 판단되어 context-API를 활용하기로 했다.
### 공유하고 싶은 내용
> react를 활용하는 이유

1. react 활용하는 이유
<br>
<br>
## 2022.06.19 일요일
### 공부한 내용

> 학급일지 프로젝트 작업 

1. context-API를 활용 theme 변경 기능 구현
      - grommet-icons theme provider와 custom theme provider와의 충돌
        + 어떻게 해결해야 할지 방법 모색

<br>
<br>

## 2022.06.19 일요일
### 공부한 내용


> 네트워크 학습

1. 네트워크 기본 개념
      - 'public address'와 'private address'의 차이 
        +  'public address'는 통신사에서 제공한 외부 ip이고 'private address'는 내부 네트워크 장비 '공유기 등' 에 의해 내부적으로 적용된 아이피이다.
      - 'WAN'과 'LAN' 이란 무엇인지, 어떻게 사용되는지
        +  'WAN'은 광역 네트워크 로 통신사에서 제공한 회선을 네트워크 장비에 연결할 때는 'WAN'포트에, 'LAN'은 지역 네트워크로 네트워크 장비에서 내부 각 PC에 장비에 연결할때 'LAN'포트에 연결한다. 
      - gateway address 란?
        + 'gateway'란 이종 프로토콜 및 네트워크 간에 통신을 가능하게 하며 다른 네트워크로 들어가는 '문' 역할을 하는 네트워크 포인트 이다.
        + 'gateway' 가 없다면 '로컬 네트워크' 에서만 통신이 가능하고 '외부 네트워크' 와 인터넷을 사용할 수 가 없다.
      - 'NAT' 란?
        + 'NAT'란 network address translation으로 네트워크 워크 장비에서 private ip 를 public ip 로 변경한 후 외부에 요청을 하고 해당 요청에대한 응답을 다시 private ip 로 전달 할 수 있게 해 주는 기능이다.
2. 네트워크 장비
      - '라우터'란?
        +  '라우터'는 서로다른 네트워크의 통신을 담당하는 기기로 '네트워크 경로 설정' 과 '스위칭' 의 역할을 한다.
      - '공유기'란?
        + '공유기'란 '라우터'의 많은 기능 중 'NAT'기능을 특화한 장비이다.
      - 
3. OSI 7계층 
### 공유하고 싶은 내용
> 생활코딩 네트워크 강의

1. (https://opentutorials.org/course/3265/20033)
<br>