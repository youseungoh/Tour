# TourRo(투어로) 🗺️

**대한민국 전국 여행 가이드** — 17개 시도, 전국 시군구의 관광지·맛집·문화시설·축제·숙박·레포츠 정보를 한눈에.

> © Produced by You Seung-oh · [youtube.com/@pianocanvas](https://youtube.com/@pianocanvas)

---

## 주요 기능

- 🏙️ **17개 시도 선택** — 대표 이미지와 함께 시도별 탐색
- 🔍 **시군구 검색** — 상단 검색창으로 전국 시군구 즉시 검색
- 📂 **카테고리 탭** — 관광지 / 맛집 / 문화시설 / 축제·행사 / 숙박 / 레포츠
- 📍 **장소 상세** — 사진·주소·전화번호·카카오맵 연동
- 📱 **반응형 UI** — 모바일·태블릿·PC 모두 지원

## 기술 스택

| 항목 | 내용 |
|------|------|
| 구조 | 단일 파일 HTML (`index.html`) — 빌드 도구 없음 |
| 데이터 | [한국관광공사 TourAPI 4.0](https://apis.data.go.kr/B551011/KorService2) |
| UI 아이콘 | [Lucide Icons](https://lucide.dev) (CDN) |
| 지도 연동 | 카카오맵 링크 |
| 이미지 | [Unsplash](https://unsplash.com) (시도 대표 이미지) |

## 사용 API

```
한국관광공사 KorService2
- areaBasedList2  : 지역 기반 관광정보 목록
- searchFestival2 : 축제·행사 검색 (날짜 범위)
- detailCommon2   : 관광정보 상세
- areaCode2       : 지역코드 조회
```

## 실행 방법

별도 서버 설치 없이 `index.html` 파일을 브라우저에서 바로 열면 됩니다.

```bash
# 파일 직접 열기
open index.html
```

또는 GitHub Pages를 통해 웹에서 접근:
```
https://youseungoh.github.io/Tour/
```

## 파일 구조

```
Tour/
├── index.html          # 앱 전체 (HTML + CSS + JS 단일 파일)
├── gobawu.jpg          # 고창 고바우장어 사진
├── tutbat.jpg          # 고창 텃밭쌈밥 사진
├── config.example.js   # API 키 설정 예시
└── README.md
```

## 데이터 출처

본 서비스는 **한국관광공사 TourAPI 4.0** 공공데이터를 활용합니다.  
데이터 등록·갱신은 관광공사 DB에 의존하며, 신규 관광지·맛집 등은 공공데이터 업데이트 시 자동 반영됩니다.

---

*TourRo(투어로) · 대한민국 전국 여행 가이드 · 데이터: 한국관광공사 TourAPI 4.0*
