# css

## __perspective__ 

- 3D 위치 요소에 약간의 원근감을 주기 위해 z=0 평면과 사용자 사이의 거리를 결정
- 투영점(또는 관찰자 관점,원근감,깊이감)
- transform(3D) 에서 함께 사용할 속성

#### [참고사이트 ①](https://webclub.tistory.com/486)
#### [참고사이트 ②](https://nykim.work/26)

<br>

----

계산법 ???????????

front의 translateZ = left 요소 넓이 / 2

left의 translateZ = front요소의 넓이 / 2

left의 위치 값 = translateZ(147px) - (left 요소의 넓이(38px) / 2)

top의 translateZ = front요소의 높이 / 2

top의 위치 값 = top의 translateZ(291px) - (top 높이(38px) / 2)