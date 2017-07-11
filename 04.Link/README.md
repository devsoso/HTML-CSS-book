# 링크

- 링크는 `<a>` 요소를 이용해 생성한다.
- 링크하려는 페이지는 `href`속성을 이용하여 지정한다.

```html
<a href ="http://imdb.com"> imdb </a>
```
- 웹사이트에서 폴더는 디렉터리라고도 한다.
 - 최상위 폴더는 루트폴더라고 한다.
 - 폴더끼리는 부모(바로 위 폴더) - 자식 (바로 아래)<br />
할아버지(두 번째 위 폴더) - 손자 관계(두 번째 아래)가 형성



#### 상대 url
- 자신의 웹 사이트 내에서 페이지를 링크할 때 사용
- 브라우저에게 파일을 위치를 찾는 축약 방법을 제공

  - 동일한 폴더 :`<a href="reviews.html">reviews</a>`
  - 자식 폴더 : `<a href="music/listings.html">listings</a>`
  - 손자 폴더 : `<a href="movies/dvd/reviews.html">reviews</a>
  - 부모 폴더 : `<a href="../index.html">home</a>`
  - 할어버지 폴더 : `<a href=../../index.html">home</a>`


#### 이메일 링크
`<a href="mailto:devsoso@github.com">e-mail</a>`
#### 새 창에서 링크 열기
`<a href="http://www.naver.com" target="_blank">네이버</a>(새창에서열기)`
#### 동일한 페이지의 특정 부분에 대한 링크
- id속성
 - id의 값이 숫자로 시작하면 안 된다.
 - id의 값에 공백이 들어가면 안 된다.
 - 하이픈, 밑줄, 콜론(:), 마침표 이외의 툭수기호는 들어가면 안 된다.
```html
<h1 id ="top"> 영화 제작 용어 <h1>
<a href="#arc_shot">아크쇼트</a><br />
<a href="#interlude">막간극</a><br />
<h2 id="arc_shot">아트쇼크</h2>
<p> 카메라가 피사체 주위로 원을 그리며 움직이는 쇼트 </p>
<h2 id="interlude">막간극</h2>
<p>줄거리와 상관없는 영화 중간에 등장하는 짧은 장면</p>
<p><a href="#top">맨 위로 </a></p>
```

#### 다른 페이지의 특정 부분에 대한 링크
