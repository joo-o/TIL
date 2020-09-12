### input 태그 (홀태그)
- 입력상자를 만드는 태그
주요속성
- type : 입력 형태 지정. text, password, button, submit, radio, checkbox, number
- name : 입력 값의 이름을 지정(서버가 보기 위한 이름표)
- value :입력 상자의 값을 지정
#### - radio / checkbox

\<input type="radio" name="fruit"/>사과<br/>
\<input type="radio" name="fruit"/>오렌지<br/>
\<input type="radio" name="fruit"/>포도<br/>

\<input type="checkbox" name="fruit"/>사과<br/>
\<input type="checkbox" name="fruit"/>사과<br/>
\<input type="checkbox" name="fruit"/>사과<br/>

#### - button

\<input type="button" value="클릭><br/>
\<button>클릭\</button><br/>
둘다 같음. 인풋타입 버튼보다는 버튼태그 사용해서 하는것이 더 직관적이고 스타일 시트 입력할때 편함<br/>
<br/>
button / submit 두가지 다 버튼이지만 submit은 최종적으로 전달 할 때 쓰는 타입.<br/>
<b>submit</b>--> 제출 완료로 페이지가 이동함(회원가입 완료/로그인완료 등에 사용)<br/>
<b>button</b> --> (본인인증/중복확인 등에 사용)

<br/>

### select 태그
- 드롭다운 박스를 만듬. option 태그를 사용해서 선택지를 추가함<br/>

\<select name="job" id="job"><br/>
\<option value="programing">프로그래밍</option><br/>
\<option value="design">디자인</option><br/>
\</select><br/>

인풋에서 value 는 상자에 직접 입력한 서버에 전송되는것
셀렉에서 value 는 이미 정해놓은 값을 사용자가 선택하여 서버에 전송되는 값

<br/>

### textarea 태그
- 두 줄 이상의 긴 글을 입력 받로고 해주는 입력 칸을 만듬.
- 쌍 태그로 만들어지고 태그 사이에 값을 미리 넣을 수 있음.
- textarea 내부의 컨텐츠는 줄바꿈 인식

\<textarea>
  안녕하세요.
  값을 미리 입력합니다.
\</textarea>
  
<br/>  

### label 태그
- 사용자에게 각 입력 칸을 설명해주는 레이블을 표시.
- 입력 태그에 id 속성으로 지정된 값을 for 속성으로 넣어주면 그 입력 태그를 수식함.

\<input type="text" id='username'>
\<label for="username">이름<label>

<br/>

<b>label</b> : 화면 form요소 수식 -> 사용자 눈에 보이는 이름표 <br/>
<b>name</b> : 서버가 보기 위한 이름표 -> 전송되는 데이터를 수식 -> 사용자 안보임\

  
  <br/>

### fieldset / legend 태그
- 여러 입력 태그를 하나의 그룹으로 묶고 원하는 제목을 달 수 있음
- 사용자 눈에 보이는 태그
- label이랑 비슷하지만 조금 더 큰 개념. 여러개의 인풋 및 폼 관련 태그를 그룹핑하여 사용자에게 보여줌

\<fieldset><br/>
  \<legend> 가장 좋아하는 음식은? </legend><br/>
  \<input type="radio" name="food" id="food-apple"/><br/>
  \<label for="food-apple">사과</label><br/>
  \<input type="radio" name="food" id="food-pasta"/><br/>
  \<label for="food-pasta">파스타</label><br/>
  \<input type="radio" name="food" id="food-meat"/><br/>
  \<label for="food-meat">고기</label><br/>
\</fieldset>
