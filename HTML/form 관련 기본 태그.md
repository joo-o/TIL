### input 태그 (홀태그)
- 입력상자를 만드는 태그
주요속성
- type : 입력 형태 지정. text, password, button, submit, radio, checkbox, number
- name : 입력 값의 이름을 지정
- value :입력 상자의 값을 지정

#### - radio / checkbox

\<input type="radio" name="fruit"/>사과<br/>
\<input type="radio" name="fruit"/>오렌지<br/>
\<input type="radio" name="fruit"/>포도<br/>

\<input type="checkbox" name="fruit"/>사과<br/>
\<input type="checkbox" name="fruit"/>사과<br/>
\<input type="checkbox" name="fruit"/>사과<br/>

#### - button

\<input type="button" value="클릭"/><br/>
\<button>클릭\</button><br/>
둘다 같음.<br/>
<br/>
button / submit 두가지 다 버튼이지만 submit은 최종적으로 전달 할 때 쓰는 타입.<br/>
submit--> 제출 완료로 페이지가 이동함(회원가입 완료/로그인완료) button --> (본인인증/중복확인)

<br/>

### select 태그
- 드롭다운 박스를 만듬. option 태그를 사용해서 선택지를 추가함<br/>

\<select name="job" id="job"><br/>
\<option value="programing">프로그래밍</option><br/>
\<option value="design">디자인</option><br/>
\</select><br/>

인풋에서 value 는 상자에 직접 입력한 서버에 전송되는것
셀렉에서 value = 이미 정해놓은 값을 사용자가 선택하여 서버에 전송되는 값
