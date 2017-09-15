# 서체용어
- 세리프: 명조체
- 산세리프: 고딕체

# 서체지정
### font-family / font-size

body{
  font-family: Georgia, Times, serif;
  font-size: 12px;
}
h1, h2 {
  font-family: Arial, Verdana, sans-serif;
  font-size: 200%;
}

### @font-face
- 브라우저 사용자의 컴퓨터에 폰트가 없을 경우 내려 받아 사용  
@font-face{
  font-family: 'ChunkFiveRegular';
  src: url('fonts/chunkfive.eot');
}
h1,h2{
  font-family: ChunkFiveRegular, Georgia, serif;
}
