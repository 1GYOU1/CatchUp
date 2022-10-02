## __.toFixed()__

<br>

toFixed() 메서드는 숫자를 고정 소수점 표기법(fixed-point notation)으로 표시

```js
numObj.toFixed(digits)
```
- digits : 소수점 뒤에 나타날 자릿수. 0 이상 20 이하의 값을 사용

- Number 객체를 주어진 digits 만큼의 소수점 이하 자리수를 정확하게 갖는 문자열 표현으로 반환 

- 소수점 이하가 길면 숫자를 반올림, 짧아서 부족할 경우 뒤를 0으로 채움.

<br>

```js
var numObj = 12345.6789;

numObj.toFixed();       // Returns '12346': 반올림하며, 소수 부분을 남기지 않습니다.
numObj.toFixed(1);      // Returns '12345.7': 반올림합니다.
numObj.toFixed(6);      // Returns '12345.678900': 빈 공간을 0으로 채웁니다.
(1.23e+20).toFixed(2);  // Returns '123000000000000000000.00'
(1.23e-10).toFixed(2);  // Returns '0.00'
2.34.toFixed(1);        // Returns '2.3'
2.35.toFixed(1);        // Returns '2.4'. 이 경우에는 올림을 합니다.
-2.34.toFixed(1);       // Returns -2.3 (연산자의 적용이 우선이기 때문에, 음수의 경우 문자열로 반환하지 않습니다...)
(-2.34).toFixed(1);     // Returns '-2.3' (...괄호를 사용할 경우 문자열을 반환합니다.)
```

<br>

----
## __.clearRect(0, 0, width, height)__

<br>

전체 캔버스 지우기

```js
ctx.clearRect(0, 0, Width, Height);
```

- clearRect()메서드는 직사각형 영역의 픽셀을 투명 검정( rgba(0,0,0,0))으로 설정

- 사각형의 왼쪽 위 모서리 위치부터 시작 (x, y), 크기는 width및 height로 지정

<br>

----

## __.drawImage(img, 0, 0, imgWidth, imgHeight)__

<br>

__사용예시 ↓↓__

원본 이미지는 너비가 104이고 높이가 124인 좌표 (33, 71)에서 가져오기. 

캔버스의 (21, 20)에 그려지며 너비는 87, 높이는 104.

```js
const canvas = document.getElementById('canvas');
const ctx = canvas.getContext('2d');
const image = document.getElementById('source');

image.addEventListener('load', (e) => {
  ctx.drawImage(image, 33, 71, 104, 124, 21, 20, 87, 104);
});
```

![Untitled-1](https://user-images.githubusercontent.com/90018379/187329480-45f6e3fa-7ed9-4a78-b1f2-fc43dcbfcbf6.jpg)

----
## __img.onload__

<br>

```js
let img = new Image();
img.onload = function(){
  //이미지 로드 된 후, Action
};
```
----

## __canvas.getContext(' ')__

<br>

캔버스에 연결된 그리기 컨텍스트를 정의하는 컨텍스트 식별자를 포함하는 문자열

- __2d__ : 2차원 렌더링 컨텍스트를 나타내는 CanvasRenderingContext2D 객체를 생성. ( 캔버스 랜더링 타입 2d )
- 그 외 옵션 webgl, webgl2, bitmaprenderer 등..

```js
var ctx = canvas.getContext('2d');
```