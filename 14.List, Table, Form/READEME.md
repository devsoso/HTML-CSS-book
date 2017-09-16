### list-style-type
- 순서 없는 목록(ul) : none, disc(⚫️), circle(⚪️), square
- 순서 있는 목록(ol) : decimal(123), decimal-leading-zero(01 02 03), lower-alpha(abc), upper-alpha(ABC), lower-roman(i ii iii), upper-roman(I II III)

### list-style-image

```css
ul{
  list-style-image: url("images/star.png");
}
li{
  margin: 10px 0px 0px 0px;
}
```

### list-style-position
- outside: 글머리 기호가 텍스트 박스 밖에 위치
- inside: 글머리 기호가 텍스트 박스 내부, 들여쓰기 되어 위치

### 단축형
- list-style: 순서무관
- ex) list-style: inside circle;

### 테이블
### empty-cells
- :show; 빈 셀에 테두리 표시
- :hide; 테두리 표시 x
- :inherit; 테이블이 또다른 테이블 안에 있을 시 부모 테이블 규칙 따름

### border-spacing, border-collapse
##### border-spacing: 테이블 셀간의 거리를 줄이고 늘리고
##### border-collapse: 테두리와 테이블 셀이 만날 경우 선 두께가 두배 되는걸 조절
- : collapse; 테두리들이 하나의 테두리로 합쳐진다. empty-cells은 보여짐.
- : separate; 테두리들이 서로 떨어진다. empty-cells는 설정값으로 나타남.

### 폼컨트롤 정렬
- width 프로퍼티를 설정하여 제목이 동일한 너비를 차제하게 한다.
- float 프로퍼티를 사용하여 위치를 지정한다.
- text-align 프로퍼티를 사용하여 제목을 너비의 한 곳에 치우치게 한다


### cursor
- 마우스 커서의 타입. 예컨대 폼에서 사용자가 마우스를 올려 놓았을 때의 커서 모양을 설정
- auto, crosshair, default, pointer, move, text, wait, help, url("cursor.gif");
