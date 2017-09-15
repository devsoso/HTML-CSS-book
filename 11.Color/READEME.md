# 텍스트 색상
- /*rgb값*/
```
p {
  color: rgb(100,100,90) ;
}
```
- /*헥사코드*/
```
h2 {
  color: #ee3380 ;
}
```

- /*색상명*/
```
h1{
  color: DarkCyan ;
}
```

# 배경색
- 텍스트 색상처럼 rgb/헥사/색상명을 이용
```
body {
  background-color:  rgb(200,200,200);
}
```

# 투명도
- opacity: 0.0 ~ 1.0 사이 값/ ex 0.5는 투명도 50%
```
p.one{
  background-color: rgb(0,0,0);
  opacity: 0.5;
}
```

- rgba(rgb값+alpha): 0.0 ~ 1.0 사이 값
```
p.two{
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0,0.5);
}
```

# hsl/hsla
## 색조 (hue)
- 0~360도 사이의 각도로 표현
## 채도 (saturation)
- 퍼센트로 표현
## 밝기 (lightness)
- 0%(검정), 100%(흰색)
## 투명도 (alpha)
- 0~1.0
