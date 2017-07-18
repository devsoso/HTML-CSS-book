# 테이블
### 테이블 구조
- `<table>`:테이블 생성
- `<tr>`:table row
- `<td>`:table data 테이블의 각 셀
- `<th>`:table heading 행이나 열의 머리말 <br /> th 요소에 scope속성을 사용해 머리말의 행/열을 정함

  <table>
    <tr>
      <td>15</td>
      <td>10</td>
      <td>12</td>
    </tr>
    <tr>
      <td>45</td>
      <td>60</td>
      <td>35</td>
    </tr>
</table>
```
  <table>
    <tr>
      <td>15</td>
      <td>10</td>
      <td>12</td>
    </tr>
    <tr>
      <td>45</td>
      <td>60</td>
      <td>35</td>
    </tr>
</table>
```

<table>
  <tr>
    <th></th>
    <th scope="col">가</th>
    <th scope="col">나</th>
    </tr>
  <tr>
    <th scope="row">하</th>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <th scope="row">마</th>
    <td>3</td>
    <td>4</td>
  </tr>
</table>

```
<table>
  <tr>
    <th></th>
    <th scope="col">가</th>
    <th scope="col">나</th>
    </tr>
  <tr>
    <th scope="row">하</th>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <th scope="row">마</th>
    <td>3</td>
    <td>4</td>
  </tr>
</table>
```

### 병합
`<th>` 또는 `<td>` 요소에 colspan 속성을 사용

```
<table>
  <tr>
    <th></th>
    <th>9am</th>
    <th>10am</th>
    <th>11am</th>
    <th>12am</th>
  </tr>
  <tr>
    <th>월요일</th>
    <td colspan="2">지리</td>
    <td>수학</td>
    <td rowspan="2">미술</td>
  </tr>
  <tr>
    <th>화요일</th>
    <td colspan="3">체육</td>
  </tr>
</table>
```

<table>
  <tr>
    <th></th>
    <th>9am</th>
    <th>10am</th>
    <th>11am</th>
    <th>12am</th>
  </tr>
  <tr>
    <th>월요일</th>
    <td colspan="2">지리</td>
    <td>수학</td>
    <td rowspan="2">미술</td>
  </tr>
  <tr>
    <th>화요일</th>
    <td colspan="3">체육</td>
  </tr>
</table>

### 긴 테이블
`<thead>/<tbody>/<tfoot>`
