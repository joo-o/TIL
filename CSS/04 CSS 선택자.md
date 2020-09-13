# CSS 셀렉터
- 내부/외부 스타일 시트에서 문서의 HTML 요소를 선택할 수 있게 하는 문법
- tag 선택자 : html 문서의 모든 특정 태그를 선택할 때 사용
- id 선택자 : html 문서의 하나의 요소를 특정해서 선택할 때 사용
- class 선택자 : html 문서의 여러 요소를 <b>그룹으로 선택</b>할 때 사용

<br/>

### tag 선택자
- html 태그의 이름으로 바로 선택 할 수 있음
- 어떠한 기호도 붙이지 않고 태그 이름 바로 사용
- 모든 문서 내 태그에 적용

p {<br/>
...css 속성 선언...<br/>
}

<br/>

### id 선택자
- html 태그의 속성으로 id를 지정/선언 할 수 있다.
- 하나의 id는 문서 내 하나만 존재해야함
- #기호로 표현함

\<p id="description-text-1"></p>
<b>#description-text-1 {...css 속성 선언...}</b>

<br/>

### class 선택자
- html 태그의 속성으로 class를 지정할 수 있음
- 하나의 class는 문서 내 여러 개에 지정할 수 있음
- .기호로 표현함

\<p class="description-text">\</p><br/>
\<p class="description-text">\</p><br/>
\<p class="description-text">\</p><br/>
<b>.description-text {...css 속성 선언...}<b/>


