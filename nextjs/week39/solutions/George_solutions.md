## 1. 스트리밍에 대해 설명해주세요.
- 페이지의 구성요소를 더 작은 청크로 나누고 준비되는 대로 서버에서 클라이언트로 점진적으로 스트리밍 할 수 있는 데이터 전송 기술입니다.

## 2. URL 검색 매개변수를 사용해 검색 상태를 관리하는 이유는 무엇인가요?
- 검색 매개변수가 URL에 있어 사용자는 검색 쿼리 및 필터를 포함한 현재 상태를 북마크하여 참조, 공유할 수 있습니다.
- URL 매개변수는 서버에서 직접 사용되어 초기 상태를 렌더링할 수 있으므로 서버 렌더링을 더 쉽게 처리할 수 있습니다.
- URL에 직접 검색어와 필터를 적용하면 추가적인 클라이언트 측 로직없이 사용자 행동을 쉽게 추적할 수 있습니다.

## 3. Server Actions에 대해 설명해주세요.
- 비동기 코드를 클라이언트가 아닌 서버에서 직접 실행하는것을 말합니다.
- 서버 액션을 사용하면 다양한 유형의 공격으로부터 데이터를 보호하고, 암호화된 클로저, 엄격한 입력 검사, 오류 메시지 해싱, 호스트 제한과 같은 기술을 통해 앱의 안전성을 크게 향상시킬수 있습니다.