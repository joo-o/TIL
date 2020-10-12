# DOM (Docoument Object Model)

dom은 자바스트립트 같은 프로그래밍 언어에서 HTML 문서의 정보들을 다룰 수 있게 해주는 프로그래밍 인터페이스이다.
- 프로그래밍 인터페이스 : 코드로 다른 추상적인 객체나 다른 프로그램에 접근 할 수 있게 해주는것.(가져다 쓸 수 있게)</br>
html 코드 -> 웹브라우저에 의해 dom으로 변환 <-> dom 인터페이스로 자바스크립트에서 접근


html로 작성된 화면 요소들을 웹 브라우저가 해석하고 프로그래밍 가능한 인터페이스로 제공하는 객체 모델을 의미
- html 태그로 작성된 요소들은 DOM Object로 표현된다.
- 모든 요소들은 속성, 이벤트 프로퍼티의 구성을 가진다.
- html 코드는 dom 형태로 해석되어 CSS의 적용, javascript와의 상호작용 등이 이루어진다.
- dom은 HTML 파일의 구조를 계층적으로 정리한다.

</br>

### DOM 주요객체
- document : HTML 문서의 최상의 root 객체이고, html문서 전체를 대변한다.
- element : HTML document 하위의 화면 요소 (html tag로 그려지는 요소들 등)들을 의미한다. dom에서는 계층적인 형태로 존재한다.

</br>

### DOM 접근 함수 - 원하는 객체를 리턴받는 함수, document 객체 한정 사용가능

- document.getElementByid(elementld) : 요소의 id 값 (html 태그의 id 속성)으로 요소를 가져옴
- document.getElementsByTagName(name) : 요소의 태그 종류로 (html 태그)으로 요소들을 가져온다. (배열 형태, nodeList)
- document.getElementsClassName(className) : 요소의 class 값 (html 태그의 class속성)으로 요소들을 가져옴 (배열 형태, nodeList)

</br>

### QuerySelector - document/element 객체에서도 사용가능

- document.querySelector(selector) : 선택자 문법으로 문서 내의 요소들을 가져옴. 가장 처음 요소 1개
- document.querySelectorAll(selector) : 모든 요소

// 클래스가 panels인 div 내의 li 요소들을 가져옴 var element = document.querySelector("div.panels li");

</br>

### DOM 객체 추가

Dom 객체를 생성해서 DOM 구조에 추가하면 화면에 표시된다.
- document.createElement(tagName) : 새로운 DOM 노드 객체를 생성한다.
- (특정 element).appendChild(삽입할 DOM 노드 객체) : 특정 DOM 객체 하위에 다른 DOM 객체를 삽입한다.
