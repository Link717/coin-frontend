## coin PRJ

- OPEN API를 활용한 웹 어플리케이션 구현

### 개발 기간 및 인원

- 개발 기간: 2021/01/06 ~ 2021/01/14 (1주)

### 적용 기술

#### Main

- React.js(Hooks), React-router

#### Library

- 전역 상태 관리 목적: React-redux, Redux-persist
- 동적 스타일링 적용 목적: styled-component
- 비동기 처리 목적: axios

### 구현 기능

#### 1. 공통

- 데이터 패치 지연시 로딩 에니메이션 구현

#### 2. 메인페이지

- 옵션별 코인 리스트 신규 업데이트 (Rank 기준 오름차순 정렬)
- 더보기 버튼 클릭시 선택한 옵션 기준으로 추가 리스트 업데이트 (Rank 기준 오름차순 정렬)
- 북마크 아이콘 클릭, 해제시 toast 메세지 구현

#### 3. 북마크페이지

- Redux store 사용한 북마크 리스트 관리 구현(Rank 기준 오름차순 정렬)

#### 4. 상세페이지

- 북마크 아이콘 클릭, 해제시 toast 메세지 구현
- 옵션 변경시 currency에 따른 코인 정보 변경
- 코인 단위변환 기능 구현
- 설명보기 버튼 구현

### 미구현 기능 및 아쉬운 점

#### 1. 북마크페이지

- 북마크 제거시 toast 팝업 띄우기 : store에서 데이터 삭제시 리스트의 물리적인 구조가 사라져 해당 component에 포함된 toast가 그려지기 전에 언마운트 되어 구현하지 못함

#### 2. 상세페이지

- 코인 단위변환시, 지수로 입력되는 값을 처리하지 못해 e+, e- 형태의 숫자가 보이는 경우가 있음
- 코인 입력창에 소숫점 8자리 이상 숫자 붙여넣기시 8자리로 변환된 값이 입력됨

### 프로젝트 후기

- 기존에는 팀으로 프로젝트를 진행했는데 이번에는 혼자서 웹 애플리케이션을 구현했다. 혼자라서 자유롭게 컴포넌트 구조를 짤 수 있는 장점도 있었고
 반대로 혼자이기 때문에 무엇이 최선인지를 고민하는 시간이 좀 더 걸렸다. 100% 원하는 기능을 전부 구현하지 못했지만, 재활용성을 고민했고 Redux를
 온전히 스스로 사용해 볼 수 있어 많은 공부가 되었다. 그리고 이번에는 유독 단위 변환하는 과정이 많아 Input 값의 Type을 고려해야 했는데 그러지 못해서 아쉬웠고
 TypeScript의 필요성을 느끼게 되어 공부를 시작하였다.
