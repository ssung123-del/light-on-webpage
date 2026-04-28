# 🕯️ 2026 새생명축제 Light On — 오륜교회

> **"빛이 있으라 하시니 빛이 있었고"** (창세기 1:3)

2026 오륜교회 새생명축제 **Light On** 공식 랜딩 페이지입니다.  
초청받은 분들이 축제의 취지와 일정을 한눈에 파악하고, 자연스럽게 참여할 수 있도록 설계되었습니다.

---

## ✨ 주요 특징

- **시네마틱 카드 디자인** — 인물 이미지를 풀블리드 배경으로 사용하고, 하단 그래디언트 오버레이로 텍스트 가독성 확보
- **다크 모드 기반 UI** — 몰입감 있는 어두운 톤 위에 골드·화이트 타이포그래피
- **반응형 레이아웃** — 데스크톱 · 태블릿 · 모바일 모두 최적화
- **스크롤 진입 애니메이션** — Intersection Observer 기반 `fadeInUp` 모션
- **순수 HTML/CSS/JS** — 프레임워크 없이 단일 파일로 구성

---

## 📋 섹션 구성

| 섹션 | 설명 |
|---|---|
| **Hero** | 축제 메인 비주얼 + 태신자 작정하기 CTA |
| **Family Seminar** | 3인 3색 릴레이 세미나 (송길원·최은영·곽상학) |
| **Outreach** | 전교인 아웃리치 안내 |
| **Invitation Day** | 위로의 아침 (이호선 교수) + 문화의 밤 (바이올린·뮤지컬) |
| **Wishlist** | 전도자 위시리스트 캠페인 + 인증 참여 CTA |
| **Closing** | 축제 마무리 메시지 |

---

## 🎨 디자인 시스템

### 컬러

| 토큰 | 값 | 용도 |
|---|---|---|
| `--ink` | `#1a2a3a` | 본문 텍스트 |
| `--blue` | `#1a5fb4` | 프라이머리 |
| `--blue-ink` | `#0d3b7a` | 강조 텍스트 |
| `--gold` | `#ffc928` | 액센트·태그·날짜 |
| `--paper` | `#f7f1e7` | 밝은 배경 |

### 타이포그래피

- **폰트**: Pretendard (Variable)
- **웨이트**: 750 (본문) ~ 950 (타이틀)
- **크기**: `clamp()` 기반 반응형

### 카드 스타일 (시네마틱)

```css
/* 인물 이미지가 카드 전체를 채우는 풀블리드 레이아웃 */
.card {
  position: relative;
  overflow: hidden;
  border-radius: 18px;
  background: #0a1929;
}

/* 하단 35%에 집중된 그래디언트로 인물은 선명하게, 텍스트는 읽기 쉽게 */
.card::after {
  background: linear-gradient(180deg, transparent 40%, rgba(6,19,31,0.88) 78%);
}
```

---

## 🛠️ 기술 스택

| 기술 | 버전/사양 |
|---|---|
| HTML5 | Semantic markup |
| CSS3 | Custom Properties, Grid, Flexbox, `clamp()` |
| JavaScript | Vanilla (Intersection Observer API) |
| 폰트 | [Pretendard](https://cactus.tistory.com/306) via CDN |
| 호스팅 | GitHub Pages |

---

## 🚀 로컬 실행

```bash
# 클론
git clone https://github.com/ssung123-del/light-on-webpage.git
cd light-on-webpage

# 브라우저에서 열기 (별도 서버 불필요)
open index.html
```

---

## 📱 반응형 브레이크포인트

| 브레이크포인트 | 대상 |
|---|---|
| `≤ 960px` | 태블릿 (1열 그리드) |
| `≤ 660px` | 모바일 (축소된 패딩·폰트) |

---

## 📂 프로젝트 구조

```
light-on-webpage/
├── index.html          # 메인 페이지 (HTML + CSS + JS 통합)
├── assets/
│   ├── light-on-hero-new.webp   # 히어로 배경
│   ├── lee-hosun.webp           # 이호선 교수
│   ├── song-gilwon.webp         # 송길원 목사
│   ├── choi-eunyoung.webp       # 최은영 교수
│   ├── kwak-sanghak.webp        # 곽상학 목사
│   ├── joypeople.webp           # 뮤지컬 출연진
│   ├── park-jihye.webp          # 바이올리니스트 박지혜
│   └── light-on-lantern.webp    # 등불 이미지
└── README.md
```

---

## 📄 라이선스

이 프로젝트는 오륜교회 새생명축제 전용으로 제작되었습니다.

---

> 🕯️ **Light On** — 어둠 속에 빛을 켜는 사람들의 이야기
