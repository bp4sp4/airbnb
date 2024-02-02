# 에어비앤비 클론 코딩

## 24/02/02(금) 시작

<h1>CSS flex</h1>

- flex-grow
  - 할당 가능한 공간의 정도
  - 형제 아이템들이 모두 동일한 flex-grow 값 = 동인한 공간
  - 형제 아이템들이 다른 flex-grow 값 = 다른 공간
- flex-shrink
  - 아이템의 크기가 container 보다 클 때 사용
  - 설정된 값에 따라 크기가 축소
  - flex-shrink : 0 = 줄어들지 않겠다!
- flex-basis
  - 아이템의 초기 크기
  - 'auto가 아닌 flex-basis'와 'with(direction : column 이면 height)' 중 flex-basis가 우선
