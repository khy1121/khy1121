<h1 align="center">Hi there, I'm 김헌영 👋</h1>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=520&lines=Frontend+Engineer;%EB%82%B4%EA%B0%80+%EB%A8%BC%EC%A0%80+%EC%93%B0%EB%8A%94+%EC%A0%9C%ED%92%88%EC%9D%84+%EB%A7%8C%EB%93%AD%EB%8B%88%EB%8B%A4;Keep+Building%2C+Keep+Shipping+%F0%9F%9A%80" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <a href="https://portfoliokhy.vercel.app"><img src="https://img.shields.io/badge/Portfolio-portfoliokhy.vercel.app-000000?style=flat-square&logo=vercel&logoColor=white" alt="portfolio"/></a>
  <a href="mailto:rlagjsdud3@gmail.com"><img src="https://img.shields.io/badge/Email-rlagjsdud3%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="email"/></a>
  <img src="https://komarev.com/ghpvc/?username=khy1121&label=Profile%20Views&color=58A6FF&style=flat-square" alt="visitor count"/>
</p>

<p align="center">
  <b>내가 먼저 쓰는 제품을 만들고, 왜 그렇게 만들었는지 설명할 수 있는 코드를 짭니다.</b><br/>
  한성대학교 컴퓨터공학부 웹공학트랙 · 2027.02 졸업예정
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake-dark.svg" alt="snake animation" width="100%"/>
</p>

---

### 🙋‍♂️ About Me

**실제로 쓰이는 서비스를 기획부터 운영까지 직접 만드는 프론트엔드 엔지니어입니다.**

교수님이 학생에게 한 명씩 물어 만들던 상담 시간표를 예약 사이트로 바꿔 **교수 3명·학생 22명**이 쓰고 있고,
팀 회의 일정을 맞추느라 서너 번씩 오가던 연락을 **한 번 입력하면 끝나도록** 줄인 웹앱도 만들어 운영하고 있습니다.
운영하면서 받은 요청을 바로 기능으로 반영합니다.

- 🧭 **일하는 방식**: 기능이 실패했을 때 사용자가 다음에 무엇을 할 수 있는지부터 정합니다
- 🤖 **AI 활용**: AI로 초안을 만들고, 테스트와 린트를 통과한 코드만 직접 읽고 반영합니다

---

### 📈 Highlights

| 25 | 368 | 99.8% | 48 | 5 |
|:---:|:---:|:---:|:---:|:---:|
| 상담 예약 실사용자<br/><sub>교수 3 · 학생 22</sub> | 해커톤 제출 때<br/>통과한 테스트 | NADOK 배너<br/>용량 감소 | Cropy 팀 저장소<br/>병합 PR | Overlap으로<br/>확정한 팀 회의 |

---

### 🚀 Projects

> 각 프로젝트의 **▶ 자세히 보기**를 누르면 실제로 겪은 문제와 해결 과정을 볼 수 있어요.

#### 📅 [상담 예약 사이트](https://onlyonereservation.vercel.app) · 개인 · 2026.09 – 운영 중
교수님이 학생에게 한 명씩 물어 표로 정리하던 상담 일정을 예약 사이트로 옮겼습니다. 기획·개발·운영을 혼자 맡았고, **교수 3명·학생 22명**이 실제로 쓰고 있습니다.
교수 선택 → 날짜 → 시간 → 이름 순서로 예약하고, 관리자는 상담자·제약조건·전체 예약을 관리합니다.

`Next.js 16` `TypeScript` `Route Handlers` `Upstash Redis` `Tailwind CSS` · [repo](https://github.com/khy1121/omfres)

<details>
<summary><b>▶ 자세히 보기</b></summary>

**1. 같은 시간에 두 명이 동시에 예약하는 문제**
- 예약 가능 여부를 확인하고 저장하는 사이에 다른 요청이 끼면 두 사람 모두 예약될 수 있었습니다.
- 슬롯 하나를 Redis 키 하나로 두고 `SET NX`로 먼저 차지한 요청만 통과시켰습니다. 늦게 온 요청은 `409`로 거절합니다.
- DB 트랜잭션 대신 이 방식을 고른 이유: 선점이 명령 하나로 끝나고, 서버리스 환경에서 DB 연결을 오래 붙잡지 않기 때문입니다.

**2. 계정 없이 관리자 화면을 지키는 방법**
- 관리자 화면에 계정 체계를 붙이기엔 과했지만, PIN 하나만 두면 유출됐을 때 대응할 방법이 없었습니다.
- PIN은 해시로 저장하고, 세션 서명 키를 PIN 해시에서 만들었습니다. **PIN을 바꾸면 기존 세션이 모두 무효화**됩니다.

**3. 운영하면서 바꾼 것**
- 처음 넣었던 학번 입력을 빼고 **이름만** 받도록 바꿨습니다. 상담 예약에 가입 절차를 두면 예약하는 사람만 줄어든다고 판단했습니다.
- 교수님의 연구실 변경 요청은 당일 반영했고, 관리자 캘린더·교수별 필터·예약 옮기기·CSV 내보내기·상담자 추가/수정을 운영 중에 추가했습니다.
- 요일별 시간대·상담 단위·예약 불가 날짜를 조합해 슬롯을 만드는 로직을 분리해서, 관리자 화면에서 상담자를 추가하면 바로 예약을 받을 수 있습니다.
- 환경변수가 없으면 메모리 저장소로 동작하게 해 로컬 개발과 배포 환경을 분리했습니다.

</details>

#### 🗓️ [Overlap](https://overlap-liard.vercel.app) · 개인 · 2026.11
각자 되는 시간을 시간표에 칠하면, 전원이 가능한 시간과 추천 시간을 계산해 주는 일정 조율 웹앱입니다. 일정을 정할 때마다 서너 번씩 오가던 연락을 **한 번 입력**으로 줄였고, 약 10명이 써서 회의 **5회**를 확정했습니다.

`React 18` `Vite` `Supabase (Postgres·Auth·Realtime·Edge Functions)` `Tailwind CSS` `PWA` · [repo](https://github.com/khy1121/overlap)

<details>
<summary><b>▶ 자세히 보기</b></summary>

**1. 여러 명이 동시에 칠하는 시간표**
- 가능 / 조율 가능 / 불가 세 단계로 칸을 칠하고, 요일·시간 줄 전체를 한 번에 칠하거나 키보드로 입력할 수 있습니다.
- Supabase Realtime으로 다른 사람이 칠한 내용이 바로 보이고, RLS 정책으로 자기 일정만 고칠 수 있게 했습니다.
- 추천 시간은 연속으로 되는 전체 구간과 시작 시각을 함께 보여 주고, 입력한 사람이 절반이 안 되면 확정 대신 초대부터 권합니다.

**2. 가입과 초대의 부담 줄이기**
- 이메일 없이 이름·생년월일·비밀번호로 가입합니다. Edge Function이 `SHA-256(이름|생년월일)`로 내부 식별자를 만들고, 생년월일은 저장하지 않습니다.
- 카카오 로그인을 붙이고, 카카오톡 공유로 약속 초대·친구 코드를 보낼 수 있게 했습니다. 카톡 친구 중 Overlap 사용자를 찾아 친구 신청도 할 수 있습니다.
- Google 캘린더 연동은 free/busy 범위만 요청해서 일정 제목이나 내용은 받지 않습니다.

**3. 직접 쓰면서 고친 것들**
- 카카오톡 인앱 브라우저나 갤럭시에서 글자 크기를 키우면 화면이 옆으로 밀리던 문제를 고쳤습니다.
- 새 버전을 배포한 직후 흰 화면이 뜨던 문제(MIME `text/html`)를 막고, 앱을 켜 둔 사이 새 버전이 나오면 "새로고침" 안내를 띄웁니다.
- 웹 푸시 알림, 설정 화면, 회원 탈퇴, 카카오 연결 해제 웹훅, 개인정보처리방침과 만 14세 미만 가입 제한, 사용자 의견함까지 실제 서비스에 필요한 기능을 갖췄습니다.

</details>

#### ✈️ [MCM Boarding Pass](https://boardingpass-seven.vercel.app) · 해커톤 팀 6인 · 2026.08
매장 방문을 비행에 빗대어 가입(여권) → 설문(탑승권) → AI 추천 동선 → 3D 여권 스탬프로 이어지는 모바일 웹입니다. 프론트엔드 2명 중 총괄을 맡아 **커밋 259/345(75%), PR 24/30**을 작성했습니다.

`React 19` `React Router 7` `Vite` `Tailwind CSS 4` `three.js` `Vitest` · [repo](https://github.com/Hsu-Likelion-14th-Hackathon/FE)

<details>
<summary><b>▶ 자세히 보기</b></summary>

**1. 가입 중 이탈한 사용자가 돌아오면 화면이 깨지던 문제**
- 카카오로 인증한 뒤 추가 정보를 안 넣고 나간 사용자가 다시 들어오면, 보호된 화면이 빈 데이터로 깨졌습니다. 가드가 토큰 유무만 봤기 때문입니다. 실기기 테스트에서 발견했습니다.
- 사용자 상태를 **비로그인 · 토큰만 있음 · 프로필 완성** 셋으로 나누고, 프로필이 완성되지 않았으면 가입 2단계로 돌려보내게 했습니다.
- 개발 환경에서 StrictMode 때문에 인가 코드가 두 번 소비되던 문제는 StrictMode를 끄지 않고 1회 소비 가드로 해결했습니다.

**2. 실서버 API 31개 연동**
- 목 데이터로 만든 18개 화면을 실제 API 31개(인증·상품·위시·쇼핑백·AI 피팅·여정·여권)에 맞춰 옮겼습니다.
- 응답 처리·에러 타입·401 처리를 공통 `apiFetch` 하나로 모으고, 삭제는 낙관적으로 처리하되 실패하면 되돌립니다.
- 31개 중 30개를 연동했고, 막힌 4건(Azure CORS, 카카오 401 등)은 원인을 좁혀 문서로 백엔드에 넘겼습니다.

**3. 3D 여권과 테스트**
- WebGL을 지원하지 않거나 모션 축소 설정인 기기에서는 DOM으로 대신 보여 주고, three.js는 별도 청크로 나눠 필요할 때만 불러옵니다.
- 테스트에서 실제 네트워크 요청을 막고 ESLint 경고 0을 커밋 조건으로 걸었습니다. 테스트는 38개 → **44개 파일 368개**로 늘었고, 라인 커버리지는 76.8%입니다.
- 개발 서버를 LAN에 열어 팀원 휴대폰에서 배포 없이 바로 확인하도록 했습니다.

</details>

#### 📚 [NADOK](https://bugitone.vercel.app) · 팀 프로젝트 · 2026.05 – 08 · 🏆 교내 해커톤 대상
책을 읽고 쓴 기록을 감정 분석해 캐릭터로 보여 주는 독서 기록 서비스입니다. 프론트엔드를 맡아 FE 저장소 **커밋 129/135(96%)**를 작성했습니다.

`React 18` `Vite` `Axios` `Tiptap` `DOMPurify` `PWA` `Vercel Functions` · [repo](https://github.com/khy1121/bugitone)

<details>
<summary><b>▶ 자세히 보기</b></summary>

**1. 배포하자마자 백엔드 호출이 전부 막힌 문제**
- HTTPS 페이지에서 HTTP 백엔드를 부르니 브라우저가 Mixed Content로 막았고, 서버 주소도 클라이언트 코드에 그대로 드러나 있었습니다.
- Vercel Function 프록시와 rewrite로 `/api` `/uploads` 요청을 거쳐 가게 하고, 실제 주소는 Vercel 환경변수에만 두었습니다.
- 같은 실수가 다시 나오지 않도록, HTTPS 페이지에서 HTTP 주소를 쓰면 axios 단계에서 막히게 했습니다.

**2. 감정 분석이 실패해도 성공처럼 보이던 문제**
- 분석 API가 실패하면 기본 캐릭터가 그대로 떠서 사용자가 실패를 알 수 없었습니다.
- 실패하면 오류 화면과 재시도로 보내고, 백엔드가 대체 결과를 줄 때는 "임의 추천" 배너를 붙였습니다.

**3. 새 버전을 배포해도 사용자가 모르던 문제**
- PWA라서 배포 후에도 캐시된 옛 화면이 보였습니다. 30분마다, 그리고 앱으로 돌아올 때 업데이트를 확인해 배너로 알립니다.
- 8.79MB SVG 배너를 16KB WebP로 바꿔 **99.8%** 줄였고, Tiptap으로 쓴 HTML은 DOMPurify로 허용 태그를 제한해 저장합니다.

</details>

#### 🌱 [Cropy (CropCare AI)](https://43.202.14.204.sslip.io/splash) · 산학협력 팀 5인 · 2026.09 – 진행 중
사진 한 장으로 농작물 병해를 진단하고 농약을 추천하는 서비스입니다. 팀장을 맡아 기획·디자인·백엔드·모델을 담당하고 있으며, 팀 저장소에서 PR **48건**을 병합했습니다.

`Next.js 15` `React 19` `FastAPI` `PyTorch (ResNet50)` `ONNX Runtime Web` `Docker` `GitHub Actions`

<details>
<summary><b>▶ 자세히 보기</b></summary>

**1. 아무것도 없는 상태에서 팀이 바로 일할 수 있게**
- 첫날 PRD·API 명세·ERD·모델 스펙·스프린트 백로그 등 문서 21종과 백엔드·프론트·ML 파이프라인 기본 코드를 올렸습니다.
- 모델 파일이 없으면 Mock 모드로 돌게 해서 팀원이 ML 없이도 프론트를 개발할 수 있게 했고, CODEOWNERS로 담당 영역을 나눴습니다.

**2. 정확도는 93%인데 특정 두 병해를 계속 헷갈리는 문제**
- ResNet50을 9개 클래스로 파인튜닝해 **test 정확도 93.1%**를 얻었지만, 오분류 44건 중 26건(59%)이 무 검은무늬병 ↔ 무 노균병 한 쌍에 몰려 있었습니다.
- 두 후보의 신뢰도가 비슷하면 결과를 하나로 단정하지 않고, 구분에 필요한 부위를 다시 찍어 달라고 안내한 뒤 두 결과를 합쳐 확정하는 흐름을 설계했습니다.
- 이 쌍만 따로 구분하는 분류기도 실험했지만 본 모델보다 나은 점이 없어 채택하지 않았고, 그 결과를 모델 문서에 남겼습니다.

**3. 통신이 끊긴 농지에서도 쓸 수 있게**
- ONNX Runtime Web·Service Worker·IndexedDB로 브라우저 안에서 진단하고 기록을 저장하며, 다시 연결되면 서버와 동기화합니다.
- PR마다 GitHub Actions로 테스트·빌드 검사를 돌리고, Docker Compose 한 번으로 전체 서비스를 띄울 수 있게 했습니다.

</details>

---

### 🛠️ Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white" />
  <br/>
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Upstash%20Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" />
  <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white" />
</p>

---

### 📊 GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=khy1121&show_icons=true&theme=tokyonight&hide_border=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=khy1121&layout=compact&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=khy1121&theme=tokyonight&hide_border=true" alt="streak stats"/>
</p>

---

<p align="center">
  <a href="https://portfoliokhy.vercel.app">Portfolio</a> ·
  <a href="https://github.com/khy1121?tab=repositories">Repositories</a> ·
  <a href="mailto:rlagjsdud3@gmail.com">Contact</a>
</p>
