```html
<div class="text_box" style="--myColor: skyblue;">
```
```css
.text_box{color: var(--myColor)}
```

```css
-webkit-background-clip: text; /* 텍스트 마스크 */
-webkit-text-fill-color: transparent; /* 텍스트 마스크 */
background-image: linear-gradient( /* 배경 그라데이션 추가*/
    45deg,
    #73caf2 30%, /* % 단계별 그라데이션 적용 */
    #fff 35%, /* % 단계별 그라데이션 적용 */
    #fff 36%, /* % 단계별 그라데이션 적용 */
    #013ebf 50%, /* % 단계별 그라데이션 적용 */
    #013ebf 100% /* % 단계별 그라데이션 적용 */
);
```

```css
@keyframes clip-height {
	0% {
		clip-path: polygon(0% 0, 100% 0%, 100% 100%, 0% 100%); /* 엘리먼트 박스 모양 변경 */
	}
	100% {
		clip-path: polygon(0% 0, 0% 0%, 100% 100%, 0% 100%); /* 엘리먼트 박스 모양 변경 */
	}
}
```

```css
@keyframes clip-height {
	0% {
		clip-path: polygon(0% 0, 100% 0%, 100% 100%, 0% 100%); /* 엘리먼트 박스 모양 변경 */
	}
	100% {
		clip-path: polygon(0% 0, 100% 0%, 100% 0%, 0% 0%); /* 엘리먼트 박스 모양 변경 */
	}
}
```