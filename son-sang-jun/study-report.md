## 2022.07.03 일요일
### 공부한 내용

> React Native 시작하기

1. React Native 개발 환경 구성
      - react native의 장점
        + javascript library 인 react로 안드로이드와 ios 두 플랫폼 모두 개발 할 수 있다.
        + react를 사용해 대상 플랫폼의 UI 라이브러리로 렌더링 할 수 있기 때문에, React 코드를 활용해 네이티브 환경과 비슷한 성능의 앱을 만들어 낼 수 있다.(가존의 webview에서의 단점을 해결한것이다.)
      - react native의 단점
        + react native 와 대상 플랫폼의 native 코드와의 사이에서 발생하는 문제의 디버깅이 쉽지 않다.
        + 대상 플랫폼의 업데이트가 될때마다 API를 react native에서 곧바로 사용 할 수 없을 수 있다.(이럴 경우 하이브리드로 문제를 해결하기도 한다.)
### 공유하고 싶은 내용
> React Native 의 장 단점
1. https://ssollacc.tistory.com/10

## 2022.07.02 토요일
### 공부한 내용

> 네트워크 학습

1. 네트워크 기본 개념
      - Https 의 동작 방식
        + https 통신이 일어날때 최초에 클라이언트와 서버에서는 각각 랜덤 데이터를 생성하고 통신이 일어나면서 클라이언트는 서버에서 인증서와 랜덤 키를 받아온다.
        + 클라이언트가 인증서를 서버에서 전송 받으면 우선 브라우저에서 신뢰할 수 있는 인증서 인지 확인한다(이때 브라우저에는 기본적으로 신뢰할 수 있는 인증서 목록이 저장되어있다. 만약 목록에 없는 인증서라면 경고 화면이 뜬다)
        + 신뢰할 수 있는 인증서라면 인증서에 있는 인증기관의 public키를 활용해 pre-master-key를 암호화하여 서버로 전송한다(이는 대칭키 이며 서버와 클라이언트에서 생성된 랜덤 데이터로 만들어진다.)
        + 서버에서는 private키를 활용해 pre-master-key가 암호화 된 것을 복호화한다.
        + 이 상황에서 클라이언트와 서버는 모두 pre-master-key를 가질 수 있게 되고 이 pre-master-key를 활용해 클라이언트와 서버는 안전하게 통신을 할 수 있게 된다.
### 공유하고 싶은 내용
> SSL 통신에 관한 자세한 내용이 포스팅 된 블로그
1. https://juliecho.tistory.com/2

## 2022.06.26 일요일
### 공부한 내용

> 네트워크 학습

1. 네트워크 기본 개념
      - Https 와 http의 차이 
        +  http 는 http 메시지를 아무런 암호화 매커니즘없이 주고 받는 프로토콜 이고, https 는 SSL이라는 layer 위에서 동작하며 주고받는 http 메시지에 암호화된 매커니즘이 추가된 프로토콜이다.
      - 대칭키 와 비 대칭키
        +  '대칭키'란 주고받는 메시지의 암호화와 복호화에 같은 key 를 활용하여 암호,복호화 하는 방식이다.
        +  
### 공유하고 싶은 내용
> SSL이란 무엇인가 에 대한 만화
1. (https://koonsland.tistory.com/42)
2. (https://opentutorials.org/course/228/4894)
3. 1번 의 공개키에 대한 개념을 이해하고 2번의 생활코딩 영상을 보면 이해가 간다.
## 2022.06.25 토요일
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

## 2022.06.19 일요일
### 공부한 내용

> 학급일지 프로젝트 작업 

1. context-API를 활용 theme 변경 기능 구현
      - grommet-icons theme provider와 custom theme provider와의 충돌
        + 어떻게 해결해야 할지 방법 모색

<br>
<br>

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

