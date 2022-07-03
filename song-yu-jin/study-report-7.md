## 2022.07.03 일요일
### 공부한 내용
- 사이드 프로젝트
  + 로그인 구현
    - Optional
    - Base64
### 공유하고 싶은 내용
- Optional
  + https://homoefficio.github.io/2019/10/03/Java-Optional-%EB%B0%94%EB%A5%B4%EA%B2%8C-%EC%93%B0%EA%B8%B0/
  + https://pkolaczk.github.io/overhead-of-optional/
  + https://www.daleseo.com/java8-optional-effective/

--- 

## 2022.07.02 토요일
### 공부한 내용
- 사이드 프로젝트
  + 로그인 구현
    > + `@ConfigurationProperties`
    >   -  `*.properties` 나 `*.yml` 파일에 있는 property를 자바 클래스에 값을 바인딩하여 사용할 수 있게 해주는 어노테이션
    > + `WebMvcConfigurer`
    >   - `@EnableWebMvc`가 자동적으로 세팅해주는 설정에 원하는 설정 추가 가능(Override)
    >     + `@EnableWebMvc`
    >       - `ViewResolver` 값 자동 등록
    >       - 추가적인 세팅을 위해서는 ①기존 세팅과 동일한 Bean을 구현하여 ②원하는 추가적인 세팅을 해서 Bean을 직접 정의해야함<br>→ 불편함
    > + `CorsRegistry`
    >   - `CorsConfiguration` 매핑에 기반한 global, URL pattern 등록 지원

### 공유하고 싶은 내용
- HTTP 메소드
  + `OPTIONS` : 목표 리소스에 대한 통신 옵션 설명
    - 예시
      + curl을 이용하여 `OPTIONS` 요청을 서버에 보내 **서버에서 지원하는 method** 확인 가능
        ```shell
        curl -X OPTIONS http://example.org -i

        HTTP/1.1 200 OK
        Allow: OPTIONS, GET, HEAD, POST
        Cache-Control: max-age=604800
        Date: Thu, 13 Oct 2016 11:45:00 GMT
        Expires: Thu, 20 Oct 2016 11:45:00 GMT
        Server: EOS (lax004/2813)
        x-ec-custom-error: 1
        Content-Length: 0
        ```
      + `OPTIONS` 메소드를 통해 **Preflight 요청**을 보내어 서버가 **해당 parameters를 포함한 요청을 보내도 되는지**에 대한 응답을 반환하게 함
        ```shell
        OPTIONS /resources/post-here/ HTTP/1.1
        Host: bar.other
        Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
        Accept-Language: en-us,en;q=0.5
        Accept-Encoding: gzip,deflate
        Accept-Charset: ISO-8859-1,utf-8;q=0.7,*;q=0.7
        Connection: keep-alive
        Origin: http://foo.example
        Access-Control-Request-Method: POST
        Access-Control-Request-Headers: X-PINGOTHER, Content-Type
        ```