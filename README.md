# 스테이 얼라이브 홈페이지

남양주 덕소의 로스터리 카페 **스테이 얼라이브(Stay Alive Coffee Roasters)** 의 정적 홈페이지입니다.
네이버 스마트스토어(`smartstore.naver.com/stayalivecoffee`)에 실제 등록된 상품 7개와 매장 정보만으로 만들었습니다.

## 파일 구성

```
index.html          홈페이지 본문 (HTML + CSS + JS 모두 이 파일 하나)
assets/
  barista-pourover.jpg 사장님 핸드드립 (히어로 이미지, 오른쪽 스크롤바 2% 크롭)
  hero-store.jpg    매장 외관 (가게 섹션 · 하단 배너)
  interior.jpg      매장 내부
  cake-chestnut.jpg 보늬밤 치즈케이크
  cafe-roastery.jpg 로스터 드럼 (카페 섹션)
  about-roast.jpg   로스터에서 식는 원두 (소개 섹션)
  about-cupping.jpg 커핑 테이블 (소개 섹션)
  p-dakso.jpg       덕소 블랜드 패키지 (200g·500g·1kg)
  p-nana.jpg        나나파크 블랜드 패키지
  p-decaf.jpg       디카페인 블랜드 패키지
  p-drip.jpg        드립체어
```

## 보는 방법

`index.html` 파일을 브라우저로 열면 바로 보입니다. 별도 서버나 설치가 필요 없습니다.
(글꼴은 Google Fonts를 불러오며, 인터넷이 없으면 시스템 글꼴로 표시됩니다.)

## 수정할 곳

| 바꾸고 싶은 것 | 위치 |
|---|---|
| 상품 가격·배송비 | `index.html`의 `price`, `ship` 부분 |
| 상품 문구 | `card-body` 안의 `h3` / `note` |
| 메뉴와 가격 | `id="menu"` 섹션의 `menu-item` |
| 영업시간·전화·주소 | `id="visit"` 섹션과 하단 `site-footer` |
| 지도 | `id="visit"` 섹션 `map-frame` 안의 `iframe` — 구글 지도 주소의 `q=` 검색어만 바꾸면 됩니다 |
| 매장 사진 | `assets/` 폴더의 같은 파일 이름으로 교체 |

## 배포

정적 호스팅이면 어디든 올릴 수 있습니다. (GitHub Pages, Netlify, Vercel 등)
`index.html`과 `assets/` 폴더를 같은 구조로 올리면 됩니다.

## 데이터 기준

- 상품·가격·배송: 2026년 11월 23일 네이버 스마트스토어 조회 기준
- 매장 정보: 매장 등록 정보 기준 (상호, 주소, 전화, 영업시간)
- 사진: 네이버 스마트스토어 「덕소 블랜드 200g」(상품번호 5370479267) 대표·상세 이미지 및 매장 게시 사진
- 지도: 구글 지도 임베드(API 키 불필요) — 네이버 지도·카카오맵 링크는 지도 아래 바에 있음
