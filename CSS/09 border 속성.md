# border 속성
특정 요소에 테두리를 지정 할 수 있다.

- border-width : 굵기(px로 표현)
- border-style : 선 종류 (solid:실선,  dotted:점선, dashed:대시선, double:이중선 등)
- border-color : 선 색
- border : 위의 3 속성을 한 번에 사용 가능 (border:1px solid #000000;)


</br>

# box-shadow 속성
테두리 외부에 그림자 효과를 준다.
- box-shadow : 5px 10px; (offset이라고 부름) -> 오른쪽으로 5px, 아래로 10px 
- box-shadow : 5px 10px #000000;  -> 위의 속성 값에 그림자 색을 검정색으로 지정
- box-shadow : 5px 10px 8px #000000;  -> 위의 속성들에 8px 정도 그림자 흐리게 지정
- box-shadow : 5px 10px 8px 10px #000000; : 위의 속성들에 10px 정도 주변으로 그림자를 퍼지게

</br>

# border-radius 속성

테두리의 둥글기를 지정한다.
- border-radius : 25px;  -> 25px 만큼 상하좌우 테두리를 둥글게
- border-radius : 20px 5px;  -> 좌측상단, 우측하단은 20px, 우측상단, 좌측하단은 5px;
- border-radius : 15px 30px 50px;  -> 좌측상단, 우측상단과 좌측하단, 우측하단 순으로 적용
- border-radius : 15px 30px 30px 20px;  -> 좌측상단, 우측상단, 우측하단, 좌측하단 순
