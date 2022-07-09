# Annotation

> Meta data를 클래스, 메소드, 인스턴스 변수 등과 같은 프로그램 요소에 연결하는 데 사용

<br /><br />

## ✅ `@Target`
> 사용자가 생성한 Annotation을 적용할 수 있는 타입 지정
- `ElementType`
  + Annotation을 적용할 수 있는 프로그램 요소 선언(클래스, 인터페이스, 생성자 등)의 유형을 지정하는 상수

    |항목|적용 가능한 타입|
    |:---|:---|
    |**`Type`**|클래스, 인터페이스, 열거형(enum)|
    |**`Field`**|필드|
    |**`Constructor`**|생성자|
    |**`Local_Variable`**|로컬 변수|
    |**`Annotation_Type`**|Annotation|
    |**`Package`**|패키지|
    |**`Type_Parameter`**|Type 매개변수|
    |**`Parameter`**|형식 매개변수|

<br />

## ✅ `@Retention`
> Annotation이 적용된 타입의 Annotation 유지 기간 설정
- 유형
  |정책|설명|비고|
  |:---:|:---|:---:|
  |**`RetentionPolicy.SOURCE`**|• 소스코드 유지<br>• 컴파일 시점에 삭제||
  |**`RetentionPolicy.CLASS`**|• 클래스 유지<br>• 클래스 파일(.class)에 기록<br>• 런타임 시 삭제|기본값|
  |**`RetentionPolicy.RUNTIME`**|• 런타임까지 유지<br>• 클래스 파일(.class)에 기록<br>• Reflection API로 어노테이션 정보 조회 가능||

<br />

## ✅ `@AuthenticationPrincipal`
> `Authentication.getPrincipal()` 메소드의 Parameter 확인 시 사용