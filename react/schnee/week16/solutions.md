1. useState, useReducer 로 생성한 상태를 최상위 컴포넌트에 배치하여 사용할 때의 단점을 설명해보세요.

답:
- props를 계속 넘겨줘야한다.
- 상태가 변경될 때마다 모든 컴포넌트가 리렌더링 된다.

2. 전역 변수를 사용하기 위해서 컴포넌트가 아닌 별도의 모듈에서 변수를 만들고 이를 컴포넌트가 참조하여 사용하면 안되는 이유를 설명해보세요.

답:
- 변수의 값이 변경되어도 리렌더링이 일어나지 않는다.
  -> useState, useReducer 등 훅에 리렌더링을 발생시키는 트리거가 없다
  -> key의 변경이 없다
  -> props의 변경이 없다
  -> 부모 컴포넌트가 리렌더링 되지 않는다
  -> 따라서 컴포넌트 함수도 실행이 되지 않는다. (이어 반환되는 JSX/리액트 파이버 객체도 그대로다)

3. 358-360 페이지에 나오는 createStore로 만든 클로저 객체는 subscribe 함수로 callbacks를 등록하고, set 함수로 callbacks를 순회하여 함수들을 실행 시킵니다. 이는 무슨 패턴일까요?

답:
- 옵저버 패턴