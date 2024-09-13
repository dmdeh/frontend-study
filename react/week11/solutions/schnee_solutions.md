1. 가상 DOM / 파이버의 장점을 설명해주세요.

답:
- 사용자의 인터랙션에 따라 DOM이 변경되야할 사항을 수동으로 추적하지 않아도 된다.
- reflow, repainting 같은 DOM 계산이 한 인터랙션에 여러번 있을 수 있는데, 이를 메모리 안에서 먼저 계산하고 최종 계산 결과만 렌더링한다. (브라우저의 계산을 최적화 한다.)

2. 더블 버퍼링이 무엇인지 설명하고, 리액트에서 렌더링을 하는 과정에서 이 기법을 쓰는 이유를 설명해주세요.

답:
- 화면에 그릴 그래픽을 사용자 화면이 아닌 보이지 않는 곳에서 미리 그린 다음, 렌더링이 완료되면 이전의 화면과 렌더링 된 화면을 바꾸는 기술
- 화면에 렌더링 하는 과정을 그대로 사용자에게 보여주면 사용자에게 렌더링이 덜 된 화면을 보여주는 경우가 생기기 때문에

3. 다음 리액트 코드와 리액트 코드를 파이버 트리로 표현한 그림을 참고해서 파이버의 작업 순서를 그림으로 그려주세요.

```
<A1>
  <B1>안녕하세요</B1>
  <B2>
    <C1>
      <D1 />
      <D2 />
    </C1>
  </B2>
  <B3 />
</A1>
```

<img src="img/react_fiber.jpg" alt="파이버 트리" width="600">

답: <br>
<img src="img/react_fiber_answer.jpg" alt="파이버 트리 정답" width="600">