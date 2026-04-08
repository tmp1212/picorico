# PICORICO — Premium Coffee & Dessert Brand Website

## 프로젝트 개요

PICORICO(피코리코)의 공식 브랜드 소개 웹사이트입니다.  
프리미엄 디저트·럭셔리 케이터링·글로벌 브랜드 런칭(PALETTE CAKE MUSEUM)을 소개하는 싱글 페이지 한국어/영어/태국어 3개 국어 지원 사이트.

---

## 구현 완료 기능

### 페이지 섹션
| 섹션 | ID | 내용 |
|------|-----|------|
| Hero | `#hero` | PICORICO 워드마크 + 파티클 배경 + CTA 버튼 |
| 브랜드 스토리 | `#brand-story` | 회사 소개 + 4개 브랜드 가치 카드 |
| 메뉴 | `#menu` | 시그니처 커피 / 프리미엄 디저트 / 특허 제품 탭 |
| 케이터링 | `#catering` | 럭셔리·기업·PALETTE CAKE MUSEUM 카드 |
| 팀 | `#team` | CEO·Executive Chef·AD·로스팅팀 카드 |
| 글로벌 비전 | `#global` | PALETTE CAKE MUSEUM 브랜드 런칭 정보 |
| 직영 매장 | `#stores` | 김포공항·영등포·은평·태국(예정) 4개 매장 |
| 문의 | `#contact` | 이메일 폼 |

### 최근 업데이트 이력 (2025-04 최종)

1. **Hero 워드마크 깜박임 수정** — `letter-rise`와 `glow-pulse`를 완전 분리. JS가 모든 글자 등장 후 `.glow` 클래스를 추가하는 방식으로 모바일 GPU 깜박임 해결. `will-change` 범위 최소화.

2. **브랜드 가치 카드 이미지 교체**
   - 전문가 그룹: `images/expert_team.jpg` (커피 원두 배경)
   - 특허기술력: `images/patent_tech.jpg` (사람 없는 커피 정물)
   - 럭셔리 케이터링: `images/miumiu.jpg` (명품 행사 이미지)
   - 글로벌 비전: `images/global.jpg`

3. **시즌 스페셜 이미지 교체** — `images/season_beans.jpg` (커피잔 없는 원두 클로즈업)

4. **은평점 추가** — 롯데몰 은평점 카드를 직영 매장 섹션에 추가 (`images/eunpyeong_1.jpg`). 매장 그리드 4열로 변경.

5. **글로벌 비전 섹션 전면 교체** — "단순 커뮤니티 카페"에서 **PALETTE CAKE MUSEUM** 브랜드 아이덴티티(2026.07.06 CLOUD 11 Bangkok 런칭, 케이크 디자인 스튜디오, Minimal·Soft·Elegant·Warm 톤, 듀얼 브랜드 전략)로 전면 재작성. `images/global.jpg` 비주얼 추가.

6. **케이터링 카드 업데이트**
   - 럭셔리 케이터링: `images/miumiu.jpg` 배경, 명품 브랜드 목록(Prada·Moncler·Ferragamo·Miu Miu·Mercedes-Benz) 명시
   - 기업·공공기관: `images/company.jpg`
   - 경험형 이벤트 → PALETTE CAKE MUSEUM: `images/museum.jpg`

7. **회사 소개 텍스트 업데이트** — 3개 직영 매장(김포·영등포·은평) 및 명품 케이터링 클라이언트 명시

---

## 파일 구조

```
index.html              메인 페이지 (100 KB+, all-in-one)
README.md
images/
  ├── expert_team.jpg      전문가 그룹 카드 배경 (원두)
  ├── patent_tech.jpg      특허기술력 카드 배경 (커피 정물)
  ├── miumiu.jpg           럭셔리 케이터링 / 브랜드 가치 카드
  ├── global.jpg           글로벌 비전 섹션 이미지
  ├── museum.jpg           PALETTE CAKE MUSEUM 케이터링 카드
  ├── company.jpg          기업·공공기관 케이터링 카드
  ├── luxury_catering_bg.jpg AI 생성 케이터링 배경
  ├── eunpyeong_1.jpg      은평점 매장 이미지
  ├── eunpyeong_2.jpg      은평점 추가 이미지
  ├── eunpyeong_3.jpg      은평점 추가 이미지
  ├── eunpyeong_4.jpg      은평점 추가 이미지
  ├── eunpyeong_5.jpg      은평점 추가 이미지
  └── eunpyeong_signage.jpg 은평점 사인
```

---

## 진입 URI

| 경로 | 설명 |
|------|------|
| `/index.html` | 메인 페이지 (모든 섹션 포함) |
| `/#brand-story` | 브랜드 스토리 직접 앵커 |
| `/#menu` | 메뉴 섹션 |
| `/#catering` | 케이터링 섹션 |
| `/#team` | 팀 섹션 |
| `/#global` | 글로벌 비전 섹션 |
| `/#stores` | 직영 매장 섹션 |
| `/#contact` | 문의 섹션 |

---

## 기술 스택

- **HTML5 / CSS3 / Vanilla JavaScript** (단일 파일 all-in-one)
- **Google Fonts** — Cormorant Garamond (serif), Inter (sans), DM Mono
- **Font Awesome 6** (CDN)
- **외부 이미지** — Pexels CDN

---

## 다국어 지원

`data-lang="ko|en|th"` 속성 + `setLang()` JS 함수로 KO/EN/TH 전환  
`<body class="lang-ko">` 기본값

---

## 향후 개발 권장 사항

1. 은평점 실제 매장 사진(eunpyeong_2~5.jpg) 중 가장 적합한 사진으로 교체
2. 럭셔리 케이터링 명품 행사 갤러리 섹션 추가 (Prada, Moncler 등 슬라이더)
3. PALETTE CAKE MUSEUM 전용 랜딩 섹션 강화 (컬러 팔레트 인터랙티브 UI)
4. Contact 폼 백엔드 연결 (현재 더미 submit)
5. 스토어 찾기 지도 연동 (네이버맵/카카오맵)
6. SEO 메타 태그 정비 (og:image, description 등)
