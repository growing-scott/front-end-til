## CSS z-index depth 관계

1. z-index를 다루다보면 아무리 값을 높게 주어도 변하지 않는 현상을 경험할 수 있다.
2. 원인은 대부분 부모 요소의 z-index 순위에 따른 자식 요소를 컨트롤 하다보면 발생한다.
3. z-index가 후순위인 자식 요소에 z-index값을 아무리 크게 부여하여도 선 순위 부모 요소의 항상 뒤에 위치한다.
4. 이러한 경우를 피하려면 body영역 하위에 요소를 위치시켜야 한다. 그러면 동적으로 z-index를 자유롭게 변경할 수 있다.
    - Modal, Tooltip등 항시 최상위로 나와야하는 컨텐츠의 경우.

#### 참고
    - https://developer.mozilla.org/ko/docs/Web/CSS/Understanding_z-index/The_stacking_context
