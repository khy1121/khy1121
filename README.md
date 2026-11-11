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

#### 📅 [상담 예약 사이트](https://onlyonereservation.vercel.app) · 개인 · 2026.09 – 운영 중
교수 상담 일정을 관리하는 예약 서비스로, 기획·개발·운영을 모두 맡았습니다. 학번 입력 제거, 상담 장소 수정, 관리자 캘린더는 운영 중 받은 요청으로 추가했습니다.
- Redis `SET NX`로 슬롯을 선점해서, 같은 슬롯에 동시에 요청이 와도 **1건만 성공**하고 나머지는 `409`를 받습니다
- `Next.js 16` `TypeScript` `Upstash Redis` · [repo](https://github.com/khy1121/omfres)

#### 🗓️ [Overlap](https://overlap-liard.vercel.app) · 개인 · 2026.11
가능한 시간을 칠하면 전원이 되는 시간과 추천 시간을 계산해 주는 팀 회의 조율 웹앱입니다. 약 10명이 사용했고 회의 **5회**를 확정했습니다.
- Supabase Realtime으로 실시간 동기화하고, RLS로 본인 일정만 수정할 수 있게 했습니다. PWA로 설치할 수 있습니다
- `React 18` `Vite` `Supabase` `PWA` · [repo](https://github.com/khy1121/overlap)

#### ✈️ [MCM Boarding Pass](https://boardingpass-seven.vercel.app) · 해커톤 팀 6인 · 2026.08
매장 체험 모바일 웹으로, 프론트엔드 2인 중 총괄을 맡았습니다.
- 카카오 가입을 중단했다 돌아오면 보호 화면이 빈 데이터로 깨지던 문제를, 인증 상태를 **비로그인 · 토큰만 보유 · 프로필 완성** 셋으로 나눈 가드로 해결했습니다
- 세션 복원 테스트를 작성했고, 제출 시점에 44개 파일 **368개 테스트**가 통과했습니다
- `React 19` `React Router 7` `three.js` `Vitest` · [repo](https://github.com/Hsu-Likelion-14th-Hackathon/FE)

#### 📚 [NADOK](https://bugitone.vercel.app) · 팀 프로젝트 · 2026.05 – 08 · 🏆 교내 해커톤 대상
독서 기록과 감정 분석 서비스로, 프론트엔드를 맡았습니다.
- HTTPS 배포에서 HTTP 백엔드 호출이 Mixed Content로 막히던 문제를 Vercel Function 프록시로 해결했습니다
- 감정 분석이 실패해도 정상 결과처럼 보이지 않도록 재시도 경로와 안내를 따로 분리했습니다
- 8.79MB SVG 배너를 16KB WebP로 교체했습니다 (**99.8% 감소**)
- `React 18` `Vite` `Tiptap` `PWA` · [repo](https://github.com/khy1121/bugitone)

#### 🌱 [Cropy (CropCare AI)](https://43.202.14.204.sslip.io/splash) · 산학협력 팀 5인 · 2026.09 – 진행 중
사진 한 장으로 농작물 병해를 진단하고 농약을 추천하는 서비스입니다. 팀장을 맡아 기획·디자인·백엔드·모델을 담당하고 있습니다.
- 통신이 끊긴 농지에서도 ONNX Runtime Web, Service Worker, IndexedDB로 브라우저 안에서 진단하고 기록을 저장하며, 다시 연결되면 서버와 동기화합니다
- 팀 저장소에서 PR **48건**을 병합했고, PR마다 GitHub Actions로 테스트·빌드 검사를 돌립니다
- `Next.js 15` `FastAPI` `PyTorch` `ONNX Runtime Web`

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
