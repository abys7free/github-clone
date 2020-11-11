```
/* @media 미디어 타입 and (미디어특성) {
  CSS코드
} */
@media screen and (max-width: 1200px) {
  body {
    color: red;
  }
}
```


####### 미디어 타입

타입    의미                               기본값
all     모든 미디어 타입에 적용             all
screen  컴퓨터 화면, 타블렛, 스마트폰 등
print   인쇄 전용

####### 미디어 특성

특성       의미
width      뷰포트 가로 너비
max-width  뷰포트 최대 가로 너비(이하)
min-width  뷰포트 최소 가로 너비(이상)
height     뷰포트 세로 너비
max-height 뷰포트 최대 세로 너비(이하)
min-height 뷰포트 최대 세로 너비(이상)
orientation 뷰포트 방향(portrait, landscape)
기타        다른 특성들




```
.container {
  width: 100px;
  height: 100px;
  background: tomato;
}
@media screen and (min-width: 700px) {
  .container {
    height: 300px;
    background: blue;
  }
}
```

```
.container {
  width: 100px;
  height: 100px;
  background: tomato;
}
@media screen and (orientation: portrait) {
  .container {
    height: 300px;
    background: blue;
  }
}
```

