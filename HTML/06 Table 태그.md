# Table 작성하기
표를 작성하기 위해서는 여러 태그를 조합하여 코드를 작성해야함. 표 하나당 table 태그 하나.

<br/>

### table 태그
- 표의 시작과 끝

<br/>

### tr (table row) 태그
- 표의 하나의 행
- 표의 행의 수 만큼 태그 사용. ex) 4행이면 tr태그 4개 사용

<br/>

### th, td 태그
- 표의 열
- th : table head -> 표의 제목칸으로 표현됨. 볼드체로 나온다.
css에서 제목열을 지정할 수 있기에 꼭 사용하지 않아도 되지만 th태그로 제목열을 지정해놓으면 스크린리더에서 빨리 파악되므로 강조하고 싶으면 사용하는게 좋다. 


  <table>
    <tr>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>

    <tr>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>

    <tr>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>
  </table>

<br/>

### 행 / 열 합치기
- rowspan : 행 합치지 (위 아래 합치기)
- colspan : 열 합치기 (좌 우 합치기
- 합쳐진 수 만큼 (td,th)빼고 선언해줘야함. 

\<td rowspan ="n" colspan="n">

