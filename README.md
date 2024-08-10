# 스프린트 미션 5 (개선사항 반영)

## 요구사항

- Javascript
- React 18.3.1
- react-router-dom 6.26.0
- axios 1.7.3

### 배포 웹사이트: https://codeit-react-mck.netlify.app

### 기본

- [x] 중고마켓 페이지 주소는 “/items” 입니다.
- [x] 페이지 주소가 “/items” 일때 상단네비게이션바의 '중고마켓' 버튼의 색상은 “3692FF”입니다.
- [x] 상단 네비게이션 바는 이전 미션에서 구현한 랜딩 페이지와 동일한 스타일로 만들어 주세요.
- [x] 상품 데이터 정보는 https://panda-market-api.vercel.app/docs/#/ 에 명세된 GET 메소드 “/products” 를 사용해주세요.
- [x] '상품 등록하기' 버튼을 누르면 “/additem” 로 이동합니다. ( 빈 페이지 )
- [x] 전체 상품에서 드롭 다운으로 “최신 순” 또는 “좋아요 순”을 선택해서 정렬을 할 수 있습니다.
- [x] 반응형 구현

### 심화

- [x] 페이지네이션 기능을 구현합니다.
- [x] 반응형으로 보여지는 물품들의 개수를 다르게 설정할때 서버에 보내는 pageSize값을 적절하게 설정합니다.

### 변경사항

- 라우팅을 위해 react-router-dom을 사용하였습니다.
- axios를 사용해서 데이터를 가져왔습니다.
- 앞서 제출한 스프린트 미션 5의 코드리뷰 개선사항을 반영하였습니다. 정말 감사합니다. 많이 배우고 있습니다!
  - 비효율적인 코드들을 정리했습니다.
  - api의 파라미터들을 활용하고, utils 폴더에 베스트상품과 전체상품을 가져오는 함수 하나씩 만들어 필요한 곳에서 사용했습니다.
  - 모바일 환경에서 전체 페이지를 표출하면 화면 밖으로 넘어가게 되어 화살표로만 이동하도록 하고, 가운데에 있는 페이지 숫자가 바뀌도록 했으며, 화살표로 이동할 수 있다는 것을 사용자에게 알리는 애니메이션을 사용했습니다.
  - 검색 시 사용자가 입력할 때마다 서버로 요청을 하여 불필요한 자원낭비를 하고 있었습니다. 그래서 엔터를 누르면 서버로 요청하도록 변경했습니다.
  - scrollToTop을 hook 폴더에서 관리하게 변경했습니다.
  - 현재 위치한 상단 메뉴에 파란글자가 나오게 하는 것을 누락하여 새로 적용했습니다.
  - 제품의 title을 description으로 설정했었는데 name으로 변경하였습니다.
  - 

## 스크린샷

|                            중고마켓 페이지                              |                     중고마켓 페이지(태블릿)                      |
| :--------------------------------------------------------------------: | :--------------------------------------------------------------: |
|   <img src="/public/itemPage_desktop.png" width="400" height="400">    | <img src="/public/itemPage_tablet.png" width="400" height="400"> |
|                        중고마켓 페이지 (모바일)                          |
| :--------------------------------------------------------------------: |
|    <img src="/public/itemPage_mobile.png" width="400" height="400">    |

## 멘토에게

- 

