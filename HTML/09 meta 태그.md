# meta tag
- 웹문서의 정보(메타데이터)를 알려주기 위해 작성하는 태그.
- 사용자에겐 보이지 않지만, 웹 브라우저, 검색엔진, 메타데이터를 활용하는 웹서비스들이 사용.
- <head>태그 내 위치하고 홀태그 형식으로 사용.

\<br/>

### meta charset
- 웹문서의 문자 인코딩을 알려주는 역할. 현재는 유니코드 기반인 UTF-8인코딩을 사용하기 때문에 <b>charset="UTF-8"</b>로 작성

<br/>

### viewport
- 웹 문서가 그려지는 영역(viewport)에 대해 크기나 확대 비율을 어떻게 조정 할 지 정하는것
- 모바일이 나오면서 중요함
<br/>

\<meta name="viewport" content="width=device-width, initial-scale=1.0">

- width : 웹문서가 표현되는 영역의 너비 지정. 모바일 기기 너비에 맞추려면 device-width 값 사용
- initial-scale : 처음 화면에 보여질 때의 배율 결정. 1.0이면 기본 크기이고 2.0이면 2배 크기
- user-scalable : 모바일에서 확대축소 가능 유무 ex) no
- maximum-scale : 확대축소 맥시멈값 ex) 2.0
- minimum-scale : 확대축소 미니멈값

<br/>

### meta 태그 : author, descriotion, keyword
- 검색엔진(SEO)이나 외부 웹 서비스에 알려질 정보들 표현하는 것

\<mata name="author" content="인프런"><br/>
\<mata name="keywords" content="HTML"><br/>
\<mata name="description" content="웹개발 오리지널">

<br/>

### meta 태그 : open graph
- 위 메타 태그로도 정보를 나타낼 수 있지만 open graph 메타 태그를 사용하면 페북과 같은 sns에 더 자세한 정보를 알려 줄 수 있음
- 위에서는 meta name을 사용했다면 property를 사용. 구글에서 사용하는 타이틀, sns 웹브라우져에서 뜨는 타이틀을 다 구분해서 사용 할수 있음

\<meta proprerty="og:title" content= "인프런"/><br/>
\<meta proprerty="og:type" content= "article"/><br/>
\<meta proprerty="og:url" content= "실제 주소 및 대표 url"/><br/>
\<meta proprerty="og:image" content= "이미지썸네일"/>
