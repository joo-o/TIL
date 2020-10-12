# 이벤트 (Event)

웹사이트에서 화면 요소 / 도큐멘트에 대해 조건이나 상태가 변경되었을때 웹브라우저에서 발생시키는 사건들을 의미</br>
DOM 기반의 요소들은 event를 감지해 그 이벤트가 감지되었을때 원하는 코드가 실행되도록 할 수 있다.

click 이벤트 (사용자가 마우스 클릭)

<div> -> <event listener>

event listener = 요소에 이벤트가 발생했을때 실행되길 원하는 코드를 사전에 등록하는 개념

</br>

# 대표적인 이벤트 종류

많은 종류의 이벤트를 감지 할 수 있게 DOM 차원에서 미리 정의되어 있다. (https://developer.mozilla.org/en-US/docs/Web/Events)

- click : 해당 객체를 클릭했을 때 발생
- mousemove : 해당 객체 위에서 마우스를 이동했을 때 발생
- keypress : 해당 객체가 선택된 상태에서 키보드 입력이 있을 때 발생
- submit : form의 전송(제출, submit) 버튼이 눌렸을 때 발생
- load : 해당 객체가 화면에 로딩이 완료되어 화면에 표시될때 발생

</br>

# Event 리스너 등록

var element = document.getElementById("panels");

element.addEventListener('click',function() {

alert('안녕');

}); // 등록 시에 익명함수로 바로 선언하거나

or

element.addEventListener('click', preFunc); // 이미 선언된 함수를 사용할수도 있음( 어디선가 함수를 선언 했다는 전제 조건에 한해)

</br>

### 익명함수 / 콜백함수 (익명함수는 콜백함수 안에 포함)

- 익명함수 :  이름을 정하지 않고 함수블록만 정의해서 사용하는 함수 (코드상에서 이름을 부를 필요가 없을경우. 다른 객체에 의해 재사용 될 일이 없을때 )
- 콜백함수 : 이벤트 리스너와 같이 특정 트리거가 발생했을 때 완료시점에 호출받기 위한 함수 (매개변수로 전달하는 함수
