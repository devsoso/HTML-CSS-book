# 폼

### `<form>`
- action : action 속성의 값은 전송시 폼에 있는 정보를 수신할 -서버 페이지의 URL이다.
- method : get(검색) 이나 post(등록) 라는 두 가지 방식 중 하나를 사용해 폼을 전달할 수 있다.

### `<input>`
- type="text" : 한 줄의 텍스트 입력
- type="password" : * 처리 됨
- name : 폼에 입력한 정보가 서버의 어떤 폼 컨트롤에 해당하는지
- maxlength : 필드에 입력하는 문자의 수를 제한

<form action="http://www.example.com/login.php">
  <p> 사용자명:
    <input type="text" name="username" size="14" maxlength="30" /> </p>
  <p> 비밀번호:
    <input type="password" name="password" size="15" maxlength="30" /> </p>
</form>

```
<form action="http://www.example.com/login.php">
  <p> 사용자명:
    <input type="text" name="username" size="14" maxlength="30"> </p>
  <p> 비밀번호:
    <input type="password" name="password" size="15" maxlength="30" /> </p>
</form>
```

- type="radio" : 여러 옵션 중 하나만 선택
- type="checkbox" : 하나 이상 선택 또는 해제 가능
- value : 선택된 옵션이 서버로 전송되는 값
- checked="checked" : 하나의 버튼에만 사용해야 함

<form action="http://www.example.com/login.php">
  <p> 좋아하는 장르를 선택해주세요
<input type="radio" name="genre" value="rock" checked="checked" /> 락
<input type="radio" name="genre" value="pop" /> 팝
</p> </form>

```
<form action="http://www.example.com/login.php">
  <p> 좋아하는 장르를 선택해주세요
<input type="radio" name="genre" value="rock" checked="checked" /> 락
<input type="radio" name="genre" value="pop" /> 팝
</p> </form>
```

<form action="http://www.example.com/login.php">
  <p> 사용하는 음악 서비스들을 선택해주세요.
<input type="checkbox" name="service" value="itunes" checked="checked" /> 아이튠즈
<input type="checkbox" name="service" value="sptify"
 /> 스포티파이 </p></form>

```
<form action="http://www.example.com/login.php">
  <p> 사용하는 음악 서비스들을 선택해주세요.
<input type="checkbox" name="service" value="itunes" checked="checked" /> 아이튠즈
<input type="checkbox" name="service" value="sptify"
 /> 스포티파이 </p> </form>
```

- type="file"
`<input type="file" name="user-song />"`
- type="submit"
`<input type="submit" name="music" value='upload' />`
- type="image": 전송버튼에 이미지를 사용하고 싶은 경우
`<input type="text" name="email />"`
`<input type="image" src="images/subscribe.jpg" width="100" height="20" /`
- type="hidden"

### `<textarea>` - 빈 요소 아님!!
`<textarea name="comments" cols="20" rows="4"> 의견을 입력해 주세요</textarea>`

### `<select>`
- `<option> ~ </option>`
- selected
- size : size 속성을 추가해 하나 이상의 옵션을 보여주는 박스로 변경 가능
size 속성 값은 한번에 보여주고 싶은 옵션의 수
- multiple : 여러개 선택 가능

```
 <form action="http://www.example.com/login.php">
  <p> 어떤 기계를 사용하여 음악을 들으십니까? </p>
<select name="devices">
  <option value="ipod">아이팟</option>
  <option value="radio">라디오</option>
  <option value="computer">컴퓨터</option>
</select>
</form>
```

```
<form action="http://www.example.com/login.php">
 <p> 어떤 기계를 사용하여 음악을 들으십니까? </p>
 <select name="devices" size="3" multiple="multiple">
   <option value="ipod" selected="selected">아이팟</option>
   <option value="radio">라디오</option>
   <option value="computer">컴퓨터</option>
 </select>
 </form>
```

### `<button>`
`<button> <img src="images/add.gif" alt="add" width="10" height="10" /> 추가 </button>`

### `<label>` : 폼컨트롤에 레이블 붙이기 글씨선택해도 체크가능
- 텍스트 설명과 폼 입력을 모두 포함하는 방식 <br />
`<label> 나이 : <input type="text" name="age" /></label> <br />`
- 폼 컨트롤에서 분리한 다음 for 사용하여 레이블을 붙일 폼 컨트롤을 지정하는 방식 <br />
`<input id="female" type="radio" name="gender" value="f"><label for="female">여성</label>
<input id="male" type="radio" name="gender" value="m"><label for="male">남성</label>`
- for : for 속성은 레이블이 속한 폼컨트롤을 의미 <br />
for 속성의 값은 레이블을 붙일 폼 컨트롤의 id속성 값과 일치해야 한다.
id 속성의 값은 페이지에 있는 여러 요소 가운데 해당 요소를 고유하게 식별하는데 사용

### `<fieldset>` / `<legend>`
```
<fieldset>
  <legend>신상정보</legend>
<label> 나이 : <input type="text" name="age" /></label> <br />
성별 :
<input id="female" type="radio" name="gender" value="f"><label for="female">여성</label>
<input id="male" type="radio" name="gender" value="m"><label for="male">남성</label>
</fieldset>
```
### 폼유효성검증 :빈칸을 넘기지 않음
required="required"


- type="date" :사용자에게 날짜요청
```
<label for="depart"> 출발일자: </label>
<input id="depart" type="date" name="depart" />
```
- type="email" :키보드가 자동으로 최적화됨
```
<input type="email" name="email" />
<input type="submit" value="전송" />
```
- type="url" :사용자에게 웹페이지 주소를 요청할 때
- type="search": 검색어 입력하는 한 줄 텍스트박스 제공
  - placeholder : 검색 칸에 텍스트 표시
```
<form action="http://www.example.org/search.php">
<p> 검색 </p>
<input type="search" name="search"
placehoder="키워드 입력" />
<input type="submit" value="전송" />
</form>
```
