# 서체용어
- 세리프: 명조체
- 산세리프: 고딕체

# 서체지정

### font-family / font-size

```css
body{
  font-family: Georgia, Times, serif;
  font-size: 12px;
}
h1, h2 {
  font-family: Arial, Verdana, sans-serif;
  font-size: 200%;
}
```

### @font-face
- 브라우저 사용자의 컴퓨터에 폰트가 없을 경우 내려 받아 사용  
```css
@font-face{
  font-family: 'ChunkFiveRegular';
  src: url('fonts/chunkfive.eot');
}
h1,h2{
  font-family: ChunkFiveRegular, Georgia, serif;
}
```

### font-weight
- normal
- bold

### font-style
- normal
- italic: 필기체를 기울인 것
- oblique: 일반폰트를 기울인 것

### text-transform
- uppercase
- lowercase
- capitalize : 첫글자 대문자

### text-decoration
- none : 텍스트에 적용한 효과 제거
- underline: 밑줄
- overline: 윗줄
- line-through: 가운데줄
- blink: 깜빡

```css
.credits{
  font-weight: bold ;
  font-style: italic ;
  text-transform: capitalize ;
}
```

### line-height = 리딩(행간)
### letter-spacing / word-spacing = 커닝(자간)
- 문자 사이의 간격  / 단어 사이의 간격
- 3개다 em 단위로 설정

```css
h1, h2 {
  letter-spacing: 0.2em ;
  word-spacing: 1em ;
}
```


### text-align : 정렬
- left / right / center
- justify : 단락에서 마지막 줄을 제외하고 양쪽 정렬

### vertical-align: 세로 정렬
- 테이블셀과 함께 사용
- ```<img>, <em>, <strong> ```요소 같은 인라인 요소와 함께 사용
- baseline
sub
super
top
text-top
middle
bottom
text-bottom

### text-indent
- 텍스트의 첫번째 줄을 들여쓰기
- 양수 값은 들여쓰기, 음수 값은 브라우저창 밖으로 벗어남

### text-shadow
- 첫번째 값: 그림자 가로 길이 -값(왼) +값(오)
- 두번째 값: 그림자 세로 길이 -값(위) +값(아래)
- 세번재 값: 그림자의 범짐 효과 / 선택
- 네번째 값: 그림자의 색상

```css
p.one {
  text-shadow: 1px 1px 0px #000000 ;
}
```

# 유사요소 / 유사클래스
### first-letter, first-line
- 유사요소: 다른 요소에서 처럼 값을 설정
- 첫 문자나 첫 줄을 다른 값으로 지정  
```css
p.intro:first-letter {
  font-size: 200%;
}
p.intro:first-line {
  font-weight: bold;
}
```
### link, visited
### hover, active, focus
- 유사클래스: class 속성에 대한 부가적인 값
- hover: 마우스 등을 요소위에 올려 놓을 때
- focus: 폼 입력시 클릭하는거 같은거
- 유사클래스 작성시 순서 : link / visited / hover / focus / active

```css
a:link {
  color: deeppink ;
  text-decoration: none ;
}
a:visited {
  color: black ;
}
a:hover {
  color: deeppink;
  text-decoration: underline ;
}
a:active {
  color: darkcyan ;
}
```

### 속성 선택자
pass 
