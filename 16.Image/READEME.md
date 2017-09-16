#### css를 사용한 이미지 정렬
- float 프로퍼티 이용

#### css를 사용한 이미지 가운데 정렬하는 방법 2가지
- 기본적으로 이미지는 inline 요소 = 이미지가 텍스트에 둘려싸여 위치한다는 의미
- 첫번째 방법
  1. display 프로퍼티를 사용 block레벨 요소로 변환해야 함
  2. 이미지 자체에서 margin 프로퍼티를 사용하고 왼쪽 오른쪽 값을 auto 설정
- 두 번째 방법
  1. 부모 요소에서 text-align 프로퍼티의 값을 center로 설정


#### background-image
#### background-repeat
- repeat: 배경이미지를 가로와 세로로 반복
- repeat-x: 가로로 반복
- repeat-y: 세로로 반복
- no-repeat: 한번만 나타냄
#### background-attachment
- 이미지를 한곳에 고정시킬지 스크롤하여 이동할 때 같이 움직일지 여부
- fixed
- scroll

#### background-position
- 이미지를 반복하지 않을 경우 브라우저 창에서의 배경 이미지 위치를 지정
- 한쌍의 값을 설정한다. 첫번째 값은 가로, 두번째 값은 세로. 값을 하나만 지정하면 두번째 값은 자동으로 center
- left top / left center / left bottom
- center top / center center / center bottom
- right top / right center / right bottom

```css
body{
  background-image: url("images/tulip.gif");
  background-repeat: no-repeat;
  background-position: center top;
}
```

#### 단축형
- 1. background-color
  2. background-image
  3. background-repeat
  4. background-attachment
  5. background-position

```css
body{
    background: #ffffff url(images/"tulip.gif") no-repeat top right ;
}
```

#### 이미지 롤오버&스프라이트
- 사용자가 링크나 버튼위에 마우스를 올려 놓으면 (롤오버)
- 하나의 이미지가 인터페이스의 여러 부분에 사용되는 경우를 (스프라이트)

- 롤오버할 경우 두번째 스타일로 바퀴고 클릭하면 세번째 스타일로 바뀌는 링크나 버튼을 만드는 방법-> 사용자가 요소 위로 마우스를 이동하거나 요소를 클릭하면 배경 이미지의 위치는 관련 이미지를 보여주기 위해 이동한다.

```css
a.button {
  height: 36px;
  background-image: url("images/button-sprite.jpg");
  text-indent: -9999px;
  display: inline-block;
}
a#add-to-basket {
  width: 174px;
  background-position: 0px 0px;
}
a#framing-options {
  width: 210px;
  background-position: -175px 0px;
}
a#add-to-basket:hover {
  background-position: 0px -40px;
}
a#framing-options:hover {
  background-position: -175px -40px;
}
a#add-to-basket:hover {
  background-position: 0px -80px;
}
a#framing-options:hover {
  background-position: -175px -80px;
}
```

- <a>요소는 인라인 요소이므로 이링크의 display 프로퍼티를 inline-block으로 설정
- 이를 통해 해당 버튼의 크기와 일치하도록 각 <a>요소의 너비와 높이를 지정할 수 있음
- background-position 프로퍼티는 이미지를 이동하여 알맞은 상태의 버튼을 보여주는데 사용
- 마우스를 올려높으면 :hover 유사 클래스가 실해오디어 버튼의 다른 상태를 보여주기 위해 이미지의 background-position을 이동하는 규칙이 수행
- 클릭하면 :active 유사 클래스가 실해오디어 버튼의 세번째 상태를 보여주는 규칙 수행

#### css3: 그라디언트
```css
#gradient{
  /*대안색상*/
  background-color: #66cccc;
  /*대안이미지*/
  background-image: url("images/fallback-image.png");
  /*파이어폭스 3.6+*/
  background-image: -moz-linear-gradient(#336666,#66cccc);
  /*사파리4+, 크롬 10+*/
  background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#336666), to (#66cccc);
  /*사파리 5.1, 크롬 10+*/
  background-image: -webkit-linear-gradient(#336666,#66cccc);
  /*오페라 11.10+*/
  background-image: -o-linear-gradient(#336666, #66cccc);
  height: 150px;
  width: 300px;
}
```
