### 독타입
- 다양한 버전의 HTML이 존재하기 때문에 각 웹 페이지는 HTML페이지가 사용하는 버전을 브라우저에게 알려주기 위해 DOCTYPE선언 으로 시작하여야 한다.
- <!DOCTYPE html>

### HTML에서의 주석
- ```<!--주석내용-->```

### id 속성
- 페이지에 있는 다른 요소들과 해당 요소를 고유하게 식별하는데 사용
- ex) ``` <p id="pullquote"> ~ </p> ```

### class 속성
- 페이지에서 몇 개의 특정 요소를 식별하는데 사용 <br />
예컨대 중요한 정보가 포함된 일부 텍스트 단락이 있어 이러한 요소를 구분하기 원하거나, 현재 사이트 내의 페이지를 가리키는 링크와 외부사이트를 가리키는 링크를 구분
- ex) ```<p class="important"> ~ </p>```

### 블록요소 / 인라인요소
- 블록레벨 : 새로운 줄에서 시작하는 요소 <br />
 ex) ```<h1>, <p>, <ul>, <li>```
- 인라인요소 : 같은 줄에 나란히 나타나는 요소 <br />
ex) ```<a>, <b>, <em>```

### ```<div> ``` / ```<span> ```
#### ```<div> ```
- div: 텍스트와 요소를 하나의 블록으로 그룹화 <br />
  div요소에 id나 class속성을 사용하면 div에 포함된 모든 요소에 css 스타일 규칙을 적용 가능
```
<div id="header">
<img src = ~ />
<p> ~ </p>
</div>
```

#### ```<span> ```
- span: 텍스트와 요소를 인라인으로 그룹화  <br />
 span요소는 div의 인라인 형태라 할 수 있음
 - 해당 텍스트를 주변텍스트와 구별하고 싶은데 다른 적절한 요소가 없는 경우
 - 인라인 요소가 많은 경우
- span요소와 함께 class나 id속성을 사용
 - span 요소의 목적을 설명하는데 사용
```
<p> 아니쉬 카푸어는 1991년 터너상을 수상했으면 2003년에는 <span class="gallery">데이트 모던</span> 갤러리에서 전시했다.</p>
```

### 아이프레임
현재 창에서 또 다른 페이지를 볼 수 있다.
 - src: src 속성은 표시할 페이지 url
 - height
 - width
 - scrolling: html5에서 지원하지 않음.
 - frameborder: html5에서 지원하지 않음.
 - seamless: 스크롤바를 없앰
```
<iframe
  width="450"
  height="350"
  src="https://maps.google.co.kr/>"
</iframe>
```

### ```<meta>```
- head 요소에 위치
- 검색 엔진이 파악할 수 있는 키워드, 제작자, 유횩간 설정같이 다양한 목적에 사용.
- 페이지의 유효기간 설정 가능
- 빈요소
- name의 속성값은 설정팔 프로퍼티이며
 - description
 - keywords: 쉼표로 구분된 단어
 - robots
- content 속성의 값은 해당 프로퍼티에 설정할 값임.
 - pragma: 페이지 캐시를 막음
 - expires: 페이지 만료일을 지정
```
<!DOCTYPE HTML>
  <html>
    <head>
      <title>페이지에 대한 정보</title>
      <meta name="description" content="설치 미술에 대한 에세이" />
      <meta name="keywords" content="설치,예술,의견" />
    </head>
    <body>
      <p> 메타데이터(meta data)를 검사하려면 이 페이지의 소스를 참고하기 바란다</p>
    </body>
  </html>
