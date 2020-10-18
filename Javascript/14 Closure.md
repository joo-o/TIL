# Closure (클로져)

내부함수 가 실행시점을 포함해서 외부함수의 context(맥락)에 접근 할 수 있는 것.</br>
즉, 어떤 함수를 정의할 때 외부 스코프에 정의된 변수들까지 캡쳐해서 함수가 실행될 때 사용할 수 있도록 한다.

- 정보은닉과 캡슐화를 제공할 수 있다.
- 함수는 선언 시점과실행 시점이 다를데, 함수의 외부에 있는 여러가지 정의된 변수들의 현재 상태와 함수가 실행되는 시점의 변수들의 상태와 격리가 가능하다.

</br>
<hr>

### Closure 예시

function createTodayExxhangeRate(wonPerDollar){

return <b> function (dollar) {

var result = dollar*wonPerDollar;

console.log(result);

return result;

}</b>

}

// var convertExchange = createTodayExchangeRate(1200);

// 새로운 내부함수가 생성되면서 1200 변수가 캡쳐되어 같이 저장됨 => 환율 기준값이 캡슐화됨.

convertExchange(20); // 1200원 기준으로 20달러 변환
