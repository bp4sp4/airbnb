# 에어비앤비 클론 코딩(w.fastcampus)

## 24/02/02(금) 시작 ~ 24/02/05 끝

<h3>데모사이트 - <a href="https://bp4sp4.github.io/airbnb/">airbnb</a></h1>

<h2>24/02/02</h2>
<h3>CSS flex</h3>

- 매운 간단한 클론코딩 -헤더

  - display : flex를 활용해 space-between으로 양쪽좌우를 잡음
  - gap을 알고있었지만 유용하게 쓰이게되는 주관적인 생각으로는 마진이나 패딩보다 유용하다 생각한다.
  - 사실 클론 코딩에서 제일 중요한 자바스크립트 구문

  ```
  <script>
  // 문서에서 클래스가 'category-button'인 모든 요소를 선택
  document.querySelectorAll('.category-button').forEach(button => {
    // 각 버튼에 대해 클릭 이벤트에 대한 리스너를 추가
    button.addEventListener("click", event => {
        // 현재 활성화된 카테고리 버튼의 id를 삭제
        document.querySelector("#active-category-button").removeAttribute('id');

        // 현재 클릭된 버튼에 'active-category-button' id를 추가
        button.setAttribute('id', 'active-category-button');
    });
  });

  </script>
  ```

- 메인
  - grid를 사용해 배치를 했다.
  - flex를 많이사용하다보니 grid는 많이 안써봤다 이번기회에 한번 공부해보는것도 좋을거 같다.
  - lorem ipsum 과 비슷한 사진 https://picsum.photos/ 애용해야겠다.
- 플로팅
  - 사실 가운대 배치 누르게 되면 커짐 별거 없었다.

<h2>24/02/02</h2>
<h3>CSS flex</h3>

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
