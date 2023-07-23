# JavaScript & JQuery 학습하기
JavaScript와 JQuery 학습을 위한 Repository입니다.

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
```
=== substring() ===
str.substring(1, 0); => str.substring(0, 1);
str.substring(3, -1); => str.substring(0, 3);

=== slice() ===
str.slice(1, 0); => "" 리턴
str.slice(3, -1); => python과 통일
``` 
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

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/animation_method/about_fadeTo.html"> 📜 fadeTo() 메서드 </a>
```
$("요소 선택").효과 메서드("slow"|"normal"|"fast"|1000|500 , "swing"|"linear" , 콜백함수);
```
- fadeTo() : 지정한 투명도를 적용
- fadeIn() : 숨겨진 요소가 점점 선명해
- hide() : 요소를 숨김
- slideUp() : 요소가 위로 접히며 숨겨짐
- slideToggle() : slideUp()/slideDown() 효과 적용
<br/>

### 2. Array
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/array/about_each.html"> 📜 each() </a>
```
$("요소 선택").each(function)
$.each($("요소 선택"), function)
```

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/array/about_inArray.html"> 📜 inArray() | isArray() | merge() </a>
- $.inArray() : 배열에 저장된 데이터 중 지정한 데이터를 찾아 인덱스 값 반환
- $.isArray() : 지정한 데이터가 배열 객체면 true를, 배열 객체가 아니면 false를 반환
- $.merge() : 두 배열 객체를 하나의 객체로 묶음

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/array/about_map.html"> 📜 map() | grep() </a>
- $.map() : 배열에 저장된 데이터 수만큼 메서드를 반복 실행 / 메서드에 반환된 데이터는 새 배열에 저장되고 그 배열 객체 반환
- $.grep() : 배열에 저장된 데이터 수만큼 메서드를 반복 실행하며 인덱스 오름차순으로 배열의 데이터를 불러옴 / 메서드의 반환값이 true면 데이터가 새 배열에 저장되고 배열 반환
<br/>

### 3. Event Method
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_%24(this).html"> 📜 $(this) | index() </a>
- $(this) : 이벤트가 발생한 요소를 선택하여 이벤트가 발생한 요소 추적 가능
- index() : 인덱스 반환 메서드 / 이벤트를 등록한 요소 중 이벤트가 발생한 요소의 인덱스값 반환

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_changeMethod.html"> 📜 change() </a>
- 포커스가 이동하면 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_keyboardMethod.html"> 📜 키보드 이벤트 </a>
- keyup() : 자판의 키를 눌렀다 키에서 손을 떼면 이벤트 발
- keydown() : 선택한 요소에서 키보드 자판을 눌렀을 때 이벤트 발생 / 모든 키(한글 키 제외)에 대해서 이벤트 발생
- keypress() : 선택한 요소에서 키보드 자판을 눌렀을 때 이벤트 발생 / 기능키(F1~F12, Alt, Ctrl, Shift 등)에 대해서는 이벤트 발생 X

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_liveEvent.html"> 📜 라이브 이벤트 </a>
- on() 메서드 등록 방식은 이벤트를 등록한 다음에 새롭게 생성되거나 복제된 요소에는 이벤트를 등록할 수 없음
```
$(document).on("이벤트", "요소 선택", function);
```

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_loadingMethod.html"> 📜 로딩 이벤트 메서드 </a>
- ready() : 사용자가 사이트를 방문할 때 요청한 HTML 문서 객체의 로딩이 끝나면 이벤트 발생
- load() : 외부에 연동된 소스(iframe, img, video)의 로딩이 끝나면 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_mousemove.html"> 📜 mousemove() </a>
- 선택한 요소 범위에서 마우스 포인터를 움직였을 때 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_scrollEvent.html"> 📜 scroll() </a>
- 가로, 세로 스크롤바가 움직일 때마다 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/about_trigger.html"> 📜 trigger() | off() </a>
- trigger() : 강제로 이벤트 발생
- off() : 이벤트 제거

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/focus_vs_focusin.html"> 📜 focus() | blur() | focusin() | focusout() </a>
- focus() : 대상 요소로 포커스가 이동하면 이벤트 발생
- blur() : 포커스가 대상 요소에서 다른 요소로 이동하면 이벤트 발생
- focusin() : 대상 요소의 하위 요소 중 입력 요소로 포커스가 이동하면 이벤트 발생
- focusout() : 대상 요소의 하위 요소 중 입력 요소에서 외부 요소로 이동하면 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/mouseover_vs_hover.html"> 📜 mouseover VS hover </a>
- mouseout() : 선택한 요소에서 마우스 포인터가 벗어날 때마다 이벤트 발생
- mouseover() : 선택한 요소에 마우스 포인터를 올릴 때마다 이벤트 발생
- hover() : 선택한 요소에 마우스 포인터가 올라갈 때와 선택한 요소에서 벗어날 때 각각 이벤트 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/mouseover_vs_mouseenter.html"> 📜 mouseover VS mouseenter </a>
- mouseover() : 직접 이벤트를 걸지 않은 자식 요소에 마우스 포인터가 와도 이벤트 발생
- mouseenter() : 자기 자신에게 마우스 포인터가 와야만 발생

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/event_method/mouseover_vs_mouseoverFocus.html"> 📜 mouseover VS mouseover focus </a>
- mouseover : 마우스 올렸을 때만 반응
- mouseover focus : 키보드 Tab으로 버튼이 선택되었을 때에도 반응
<br/>

### 4. 객체 조작 메서드
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/object_control_method/attrControl.html"> 📜 속성 조작 메서드 </a>
- attr() : 선택한 요소에 새 속성을 생성하거나 기존의 속성을 변경할 때 또는 요소의 속성값을 불러올 때 사용
- removeAttr() : 선택한 요소에서 기존의 속성을 삭제할 때 사용
- !!!! CSS 방식은 removeAttr() 메서드로 제거 불가능 !!!!

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/tree/main/JQuery/object_control_method"> 📜 수치 조작 메서드 </a>
```
$("요소 선택").position().[left | right | top | bottom];
```
- 기준이 되는 요소를 기준으로 선택한 요소의 위치 좌표값을 반환
```
$("요소 선택").offset().[left | top];
```
- 문서를 기준으로 선택한 요소의 위치 좌표값을 반환
```
$("요소 선택").scrollTop();
$("요소 선택").scrollLeft();
```
- 스크롤바가 수직 또는 수평으로 이동한 위칫값 반환
```
$("요소 선택").scrollTop(새 값);
$("요소 선택").scrollLeft(새 값);
```
- 입력한 수치만큼 수직 또는 수평으로 스크롤바 이동
<br/>

### 5. 선택자
#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_adjacencySelector.html"> 📜 인접 관계 선택자 </a>
- $("요소 선택").parent() : 부모 요소 선택자
- $("요소 선택").parents() : 상위 요소 선택자
- $("요소 선택").closest("div") : 가장 가까운 상위 요소 선택자
- $("요소 선택>자식 요소") : 자식 요소 선택자
- $("요소 선택").children() : 자식 요소들 선택자
- $("요소 선택").prev() : 형(이전) 요소 선택자
- $("요소 선택").prevAll() : 형(이전) 요소들 선택자
- $("요소 선택").prevUntil("요소명") : 지정 형(이전) 요소들 선택자
- $("요소 선택").next() : 동생(다음) 요소 선택자
- $("요소 선택+다음 요소") : 동생(다음) 요소 선택자
- $("요소 선택").nextAll() : 동생(다음) 요소들 선택자
- $(".box_1").siblings() : 전체 형제 요소 선택자

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_attributeSelector.html"> 📜 속성과 값에 따른 탐색 선택자 </a>
```
$("요소 선택[속성]") : 선택한 요소 중 지정한 속성이 포함된 요소만 선택
$("요소 선택[속성^=값]") : 선택한 요소 중 속성값이 명시한 값으로 시작하는 요소만 선택
$("요소 선택[속성$=값]") : 선택한 요소 중 속성값이 명시한 값으로 끝나는 요소만 선택
$("요소 선택[속성*=값]") : 선택한 요소 중 속성값이 명시한 값을 포함하는 요소만 선택
$(":type 속성값") : input 요소 중 type 속성값이 일치하는 요소만 선택
```

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_basicSelector.html"> 📜 기본 선택자 </a>
- $("*") : 전체 선택자
- $("#아이디명") : 아이디 선택자
- $(".클래스명") : 클래스 선택자
- $("요소명") : 요소 선택자
- $("선택1, 선택2, 선택3, ...) : 그룹 선택자
- $("p.txt_1) : 종속 선택자

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_containsSelector.html"> 📜 콘텐츠 탐색 선택자 </a>
- $("요소 선택:contains(텍스트)") : 텍스트를 포함하는 요소만 선택
- $("요소 선택").contents() : 선택한 요소의 하위 요소 중 가장 가까운 하위 요소 선택
- $("요소 선택:has(요소명)") : 선택한 요소 중 요소명을 포함하는 요소만 선택
- $("요소 선택").has(요소명) : 선택한 요소 중 요소명을 포함하는 요소만 선택
- $("요소 선택:not(:제외 요소)") : 제외 요소만 제외하고 선택
- $("요소 선택").not(:제외 요소) : 제외 요소만 제외하고 선택
- $("요소 선택").filter(".list2") : 요소 중 class 값이 "list2"인 요소만 선택
- $("요소 선택1").find("요소 선택2") : '요소 선택1'의 하위 요소인 '요소 선택2'만 선택

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_firstOfTypeSelector.html"> 📜 first VS last </a>
```
li:first => 첫 번째 요소 선택
li:last => 마지막 요소 선택
li:first-of-type => li 요소 중 첫 번째 요소만 선택
li:last-of-type  => li 요소 중 마지막 요소만 선택
```

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_nthChild.html"> 📜 nth-child </a>
```
$("요소 선택:nth-child(1)")
```

#### <a href="https://github.com/shinyeeun789/Study-Javascript-Jquery/blob/main/JQuery/selector/about_onlyChild.html"> 📜 탐색 선택자 </a>
- $("요소 선택").slice(1, 3) : 1, 2 요소 선택
- $("요소 선택:only-child") : 선택한 요소가 부모 요소에게 하나뿐인 자식 요소면 선택
