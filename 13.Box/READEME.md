### 박스크기
- width, height
- 픽셀, 퍼센트, em(박스 안에 있는 텍스트의 크기에 따라 박스크기가 달라짐.)

### 너비제한
- min-width, max-width
- 브라우저 창이 축소/확대 됐을 때 표시/확장 할 수 있는 최소/최대 크기

### 높이제한
- min-height, max-height

### 내용이 넘칠 땐 overflow
- overflow: hidden; 박스의 크기보다 큰 부분을 숨김
- overflow: scroll; 박스에 스크롤바 추가

### MBP [테두리]
- margin: 테두리 밖
- border: 테두리  
- padding: 테두리 안

### border-width
- thin/ medium/ thick
- 퍼센트 사용 못함
- border-top-width / border-right-width / border-bottom-width / border-left-width 로 개별 적용도 가능

### border-style
- solid(실선) / dotted(점선) / dashed(긴점선) / double (이중선)
- groove (움푹 들어간 입체적인 선) / ridge(앞으로 튀어나온 선) / inset(박스 전체가 움푹) / outset
- hidden/none(테두리 숨기기)
- border-top-style / border-right-style / border-bottom-style / border-left-style

### border-color
- border-top-color / border-right-color / border-bottom-color / border-left-color
- border-color: 상 우 하 좌 ;

### 단축형
- border: 너비 스타일 색상 ;
- ex) border: 3px dotted #0088dd;

### padding
- 패딩은 박스의 너비에 더해 짐. 즉 박스가 더 커짐
- padding-top / padding-right / padding-bottom / padding-left
- padding: 10px 5px 3px 1px;

### margin
- 여백은 박스의 너비에 더해짐
- 한 박스가 또 다른 박스위에 위치하면 마진은 두개 중 큰 마진이 사용 되며 작은 마진은 무시 된다.
- margin-top / margin-right / margin-bottom / margin-left
- margin: 상 우 하 좌;
- margin: 좌우 상하;

### 가운데 정렬
- left-margin 과 right-margin을 auto로 설정
- margin: 10px auto 10px auto;

### display:
- 인라인/블록 변경
- inline; 블록레벨 요소를 인라인 요소로  
- block
- inline-block; 블록레벨 요소를 인라인 요소로, 높이 설정 가능
- none; 페이지에서 요소를 숨김. 위치하던 공간도 사라짐

### visibility   
- hidden: 요소를 숨김. 위치하던 공간은 남아있음
- visible

### box-shadow: 수평 수직 번짐 확장;
- 수평거리: -값(왼쪽) +값(오른쪽)
- 수직거리: -값(위) +값(아래)
- 번짐거리: 생략시 테두리처럼 단색 됨
- 확장거리: 양수 값은 확장 음수값은 축소
- inset: 박스 안쪽에 그림자. 수평 앞에 적음

### border-radius
- 값은 반지름의 크기를 의미
- 단위는 픽셀
- border-top-right-radius / border-bottom-right-radius / border-bottom-left-radius / border-top-left-radius
- border-radius: 10px; 는 살짝 동그란 네모
- border-radius: 상 우 하 좌 ; 모두 다르게 설정하면 찌그러진 네모
- border-radius: 100%; 는 원형 , 길이에 따라 타원
