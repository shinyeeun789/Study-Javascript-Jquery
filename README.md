# Study About JavaScript & JQuery
JavaScript와 JQuery 학습을 위한 Repository

## 📦 JAVASCRIPT
### 1. Function
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/function/about_arguments.html"> 📜 arguments란? </a>
- 함수에 전달되는 인수들을 배열 형태로 나타낸 객체
- 형태만 배열이기 때문에 배열 메서드(map, forEach 등) 사용 불가능

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/function/about_definition.html"> 📜 함수 정의 방식 </a>
- 일반 정의 함수는 호이스팅 기술 지원
- 익명 함수 참조 방식은 호이스팅 기술 지원X

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/function/about_objectConstructorFunction.html"> 📜 객체 생성자 함수 </a>
- 메모리 절약을 위해 프로토타입 사용
- 프로토타입 사용 시 원형(객체 생성자 함수)에서 생성된 객체 공유 가능

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/function/about_scope.html"> 📜 함수 스코프 </a>
- 전역 스코프
- 블록 스코프

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/function/lexicalScope_vs_dynamicScope.html"> 📜 Lexical Scope VS Dynamic Scope </a>
- 렉시컬 스코프(Lexical Scope): 함수를 어디에서 호출하는지가 아니라 어디에 선언하였는지에 따라 결정
- 동적 스코프(Dynamic Scope): 함수의 호출에 따라 상위 스코프가 결정
<br/>

### 2. String Method
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/string_method/match_vs_search_indexOf.html"> 📜 match VS search VS indexOf </a>
- 공통점: 처음 검색된 문자열의 인덱스 반환
- match: 찾는 값이 없다면 null 반환
- search: 찾는 값이 없다면 -1 반환 / 두 번째 혹은 다른 시작 위치를 인수로 지정할 수 없음
- indexOf: 찾는 값이 없다면 -1 반환 / 시작 인덱스 지정 가능

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/string_method/slice_vs_substring_vs_substr.html"> 📜 slice VS substring VS substr </a>
- 공통점: 문자열을 잘라주는 함수
<br/>

### 3. Variable
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/variable/about_const.html"> 📜 const </a>
- 초기화와 동시에 선언이 이루어져야 함
- const 자체가 값을 불변으로 만드는 것은 아님
- 상수를 선언할 때 사용

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/variable/about_let.html"> 📜 let </a>
- 블록 레벨 스코프를 가지고 있음
- 키워드 생략 불가능
- 중복 선언 불가능
- 호이스팅 당함 (단, TDZ를 통해)

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JAVASCRIPT/variable/about_var.html"> 📜 var </a>
- 함수 레벨 스코프를 가지고 있음
- 키워드 생략 가능
- 중복 선언 가능
- 호이스팅 당함
<br/>

## 📦 JQuery
### 1. Animation Method
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/animation_method/about_animate.html"> 📜 animate() 메서드 </a>
- 선택한 요소에 다양한 동작(Motion) 효과 적용 가능
- 요소를 앞으로 이동시키거나 점차 커지게 하는 등 다양한 동작 적용 가능
