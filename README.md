# 김헌영 | Frontend Developer

**요청이 실패하거나 연결이 끊겨도 사용 흐름이 이어지도록, 화면 상태와 복구 경로부터 설계합니다.**

<a href="https://portfoliokhy.vercel.app"><img src="https://img.shields.io/badge/Portfolio-portfoliokhy.vercel.app-000000?style=flat-square&logo=vercel&logoColor=white" alt="portfolio"/></a>
<a href="mailto:rlagjsdud3@gmail.com"><img src="https://img.shields.io/badge/Email-rlagjsdud3%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="email"/></a>

---

## 🙋‍♂️ 소개

- **실제로 쓰이는 서비스를 끝까지 운영하는 신입 프론트엔드 개발자**입니다. 직접 만든 **상담 예약 사이트**는 **교수 3명·학생 22명**이 사용했고, 연구실 변경 같은 운영 요청은 당일 반영했습니다. 일정 조율 웹앱 **Overlap**은 출시 2주 만에 **17명이 가입해 회의 6건을 확정**했고, "스크롤과 칠하기가 겹쳐 불편하다"는 의견을 받은 당일 '길게 눌러 칠하기'로 바꿨습니다.
- 기능을 만들 때 **"이게 실패하면 사용자는 다음에 무엇을 할 수 있나"**를 먼저 정합니다. 동시 예약 경합, 채팅 전송 실패, 오프라인 진단, 배포 직후 흰 화면처럼 사용자가 막히는 지점을 찾아 복구 경로를 설계해 왔습니다.
- 팀에서는 **PR 단위로 협업**합니다. PR마다 변경 범위, 테스트·빌드 결과, 검증하지 못한 항목을 남깁니다. 코딩 에이전트로 초안을 만들되, 테스트와 린트를 통과한 코드만 직접 읽고 반영합니다.

---

## 🚀 대표 프로젝트

> 각 프로젝트의 **문제와 해결 과정**은 포트폴리오 사이트에 정리했고, 문제 하나를 그대로 재현한 위젯을 **직접 눌러 볼 수 있습니다.**

<table>
<tr>
<td width="200" align="center" valign="top">
<a href="https://portfoliokhy.vercel.app/projects/overlap"><img src="./assets/overlap.gif" width="190" alt="Overlap 동작 화면"/></a>
</td>
<td valign="top">
<h3>🗓️ Overlap <sub><sup>팀 회의 일정 조율 웹앱</sup></sub></h3>
<p><img src="https://img.shields.io/badge/%EC%9A%B4%EC%98%81_%EC%A4%91-34C38F?style=flat-square" alt="운영 중"/> <sub>2026.11 · 개인 · 기획·개발·운영</sub></p>
<p>각자 되는 시간을 칠하면 모두가 겹치는 시간을 찾아 제안합니다. 서너 번씩 오가던 일정 조율 연락을 한 번 입력으로 줄였고, 사용자 의견은 받은 당일 기능으로 반영했습니다.</p>
<p><b>6</b> <sub>확정한 회의 · 2~7명</sub> &nbsp;&nbsp; <b>14</b> <sub>일정 입력 사용자 · 가입 17</sub></p>
<p><code>React 18</code> <code>Vite</code> <code>Supabase</code> <code>PWA</code></p>
<p><a href="https://portfoliokhy.vercel.app/projects/overlap"><b>문제와 해결 과정 · 직접 눌러 보기 →</b></a> &nbsp;·&nbsp; <a href="https://overlap-liard.vercel.app">Live</a> &nbsp;·&nbsp; <a href="https://github.com/khy1121/overlap">Code</a></p>
</td>
</tr>
</table>
<table>
<tr>
<td width="200" align="center" valign="top">
<a href="https://portfoliokhy.vercel.app/projects/omfres"><img src="./assets/omfres.gif" width="190" alt="상담 예약 동작 화면"/></a>
</td>
<td valign="top">
<h3>📅 상담 예약 <sub><sup>교수 상담 예약 시스템</sup></sub></h3>
<p><img src="https://img.shields.io/badge/%EC%9A%B4%EC%98%81_%EC%A4%91-34C38F?style=flat-square" alt="운영 중"/> <sub>2026.09 – · 개인 · 기획·개발·운영</sub></p>
<p>교수 3명이 학생 22명에게 일일이 물어 만들던 상담 시간표를 예약 사이트로 바꿨습니다. 같은 시간대에 동시에 들어온 예약은 Redis SET NX로 먼저 온 요청만 받고 늦은 요청은 409로 거절합니다. 연구실 변경 같은 운영 요청은 당일 반영했습니다.</p>
<p><b>25</b> <sub>사용자 · 교수 3 · 학생 22</sub></p>
<p><code>Next.js 16</code> <code>TypeScript</code> <code>Upstash Redis</code></p>
<p><a href="https://portfoliokhy.vercel.app/projects/omfres"><b>문제와 해결 과정 · 직접 눌러 보기 →</b></a> &nbsp;·&nbsp; <a href="https://onlyonereservation.vercel.app">Live</a> &nbsp;·&nbsp; <a href="https://github.com/khy1121/omfres">Code</a></p>
</td>
</tr>
</table>
<table>
<tr>
<td width="200" align="center" valign="top">
<a href="https://portfoliokhy.vercel.app/projects/bbung"><img src="./assets/bbung.gif" width="190" alt="붕붕어스 동작 화면"/></a>
</td>
<td valign="top">
<h3>🚗 붕붕어스 <sub><sup>커플 드라이브 기록 웹앱</sup></sub></h3>
<p><img src="https://img.shields.io/badge/%EC%A2%85%EB%A3%8C-6B7280?style=flat-square" alt="종료"/> <sub>2026.10 – 11 · 4호선톤 해커톤 · 프론트엔드 2인 · 인증·홈·기록 지도·커플 연결 담당</sub></p>
<p>연인과 함께한 드라이브를 기록하고, 테마별 장소 추천과 기록 지도로 다시 떠날 곳을 찾는 모바일 웹앱입니다.</p>
<p><b>첫 요청 401 해결</b> <sub>앱을 다시 열면 토큰 없이 나가던 요청 · 재현 테스트 추가</sub> &nbsp;&nbsp; <b>Storybook</b> <sub>PR마다 화면 변경 비교</sub></p>
<p><code>React 19</code> <code>TypeScript</code> <code>Vite</code> <code>Storybook</code> <code>Chromatic</code></p>
<p><a href="https://portfoliokhy.vercel.app/projects/bbung"><b>문제와 해결 과정 · 직접 눌러 보기 →</b></a> &nbsp;·&nbsp; <a href="https://2026-line4thon-team6-fe.vercel.app/">Live</a> &nbsp;·&nbsp; <a href="https://github.com/2026-line4thon-team6/2026-line4thon-team6-FE">Code</a></p>
</td>
</tr>
</table>

### 다른 프로젝트

| 프로젝트 | 상태 | 기간 · 팀 | 핵심 | 링크 |
|---|:---:|---|---|---|
| 📚 **[NADOK](https://portfoliokhy.vercel.app/projects/nadok)**<br/><sub>독서 기록 · 감정 분석</sub> | <img src="https://img.shields.io/badge/%EC%A2%85%EB%A3%8C-6B7280?style=flat-square" alt="종료"/> | 2026.05 – 08 · 팀 · 프론트엔드 담당 | 🏆 교내 해커톤 대상, 배포 직후 흰 화면 복구, 첫 방문 전송량 23→2.3MB | [상세](https://portfoliokhy.vercel.app/projects/nadok) · [Live](https://bugitone.vercel.app) · [Code](https://github.com/khy1121/bugitone) |
| 🌱 **[Cropy](https://portfoliokhy.vercel.app/projects/cropy)**<br/><sub>오프라인 농작물 병해 진단</sub> | <img src="https://img.shields.io/badge/%EC%A2%85%EB%A3%8C-6B7280?style=flat-square" alt="종료"/> | 2026.07 – 11 · 산학협력 팀 5인 · 팀장 | 통신이 끊겨도 브라우저에서 진단·저장(ONNX Runtime Web·Service Worker·IndexedDB), 연결되면 동기화, 헷갈리는 결과는 재촬영 안내 | [상세](https://portfoliokhy.vercel.app/projects/cropy) · [Live](https://43.202.14.204.sslip.io/) · [Code](https://github.com/hs-cropy/Cropy) |
| ✈️ **[MCM Boarding Pass](https://portfoliokhy.vercel.app/projects/boardingpass)**<br/><sub>패션 브랜드 매장 체험 웹</sub> | <img src="https://img.shields.io/badge/%EC%A2%85%EB%A3%8C-6B7280?style=flat-square" alt="종료"/> | 2026.07 – 08 · 해커톤 팀 6인 · FE 총괄 | 인증 상태 3단계 구분, 실서버 API 30/31 연동 | [상세](https://portfoliokhy.vercel.app/projects/boardingpass) · [Live](https://boardingpass-seven.vercel.app) · [Code](https://github.com/Hsu-Likelion-14th-Hackathon/FE) |
| ⏳ **[할 일 이자](https://portfoliokhy.vercel.app/projects/timebank)**<br/><sub>미루면 이자가 붙는 할 일 앱</sub> | <img src="https://img.shields.io/badge/%EC%A7%84%ED%96%89_%EC%A4%91-F2B544?style=flat-square" alt="진행 중"/> | 2026.11 – · 개인 | 하루 10% 복리 이자 계산, 기기 우선 저장·동기화, RLS 교차 점검 | [상세](https://portfoliokhy.vercel.app/projects/timebank) |

---

## 🛠️ 보유 기술

| 분야 | 기술 |
|:---:|---|
| **언어** | <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/> <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/> |
| **프론트엔드** | <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/> <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js"/> <img src="https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white" alt="React Router"/> <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/> <img src="https://img.shields.io/badge/three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white" alt="three.js"/> |
| **데이터·API** | <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/> <img src="https://img.shields.io/badge/Upstash%20Redis-00E9A3?style=for-the-badge&logo=upstash&logoColor=black" alt="Upstash Redis"/> <img src="https://img.shields.io/badge/REST%20API-5A5A5A?style=for-the-badge" alt="REST API"/> |
| **오프라인·PWA** | <img src="https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white" alt="PWA"/> <img src="https://img.shields.io/badge/Service%20Worker-3D3D3D?style=for-the-badge" alt="Service Worker"/> <img src="https://img.shields.io/badge/IndexedDB-3D3D3D?style=for-the-badge" alt="IndexedDB"/> <img src="https://img.shields.io/badge/ONNX%20Runtime%20Web-005CED?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX Runtime Web"/> |
| **테스트·품질** | <img src="https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest"/> <img src="https://img.shields.io/badge/Testing%20Library-E33332?style=for-the-badge&logo=testinglibrary&logoColor=white" alt="Testing Library"/> <img src="https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white" alt="Storybook"/> <img src="https://img.shields.io/badge/Chromatic-FC521F?style=for-the-badge&logo=chromatic&logoColor=white" alt="Chromatic"/> <img src="https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white" alt="ESLint"/> |
| **배포·협업** | <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel"/> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions"/> <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/> <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" alt="Figma"/> |
| **AI·모델 (팀 프로젝트)** | <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/> <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code"/> |

---

## 🧭 활동

| 기간 | 활동 | 내용 |
|---|---|---|
| 2026.07 ~ 2026.11 | **Cropy 산학협력 프로젝트** · 팀장 | 팀 5인. 통신이 끊겨도 브라우저에서 진단·저장하는 오프라인 기능 구현, 기획과 팀 운영(스프린트·이슈·PR) 담당 |
| 2026.03 ~ 2026.07 | **멋쟁이사자처럼 14기** · 프론트엔드 트랙 | React 과정 수료. 교내 해커톤 **대상**(NADOK), 연합 해커톤 FE 총괄(MCM) |
| 2026.08 ~ 진행 중 | **창업동아리 · 바더** · 기획 담당 | AI가 먼저 전화를 걸어 대화하고 1인칭 일기를 써 주는 서비스 기획(기획서 v1.6). 기능 명세서·화면 설계서·디자인 스펙 작성, 알파 테스트 지표 설계 |

---

## 🎓 학력 및 자격

- **한성대학교 컴퓨터공학부 웹공학트랙** · 2021.03 ~ 2027.02 (졸업예정) · 전공 평점 **3.94/4.5**
- 단과대 최우수 장학금 (3학년 2학기)
- **SQLD** (2026.09) · **정보처리기사** (2026.12 취득 예정)
- **멋쟁이사자처럼 교내 해커톤 대상** (2026.05)

---

<p align="center">
  <a href="https://portfoliokhy.vercel.app">Portfolio</a> ·
  <a href="https://github.com/khy1121?tab=repositories">Repositories</a> ·
  <a href="mailto:rlagjsdud3@gmail.com">Contact</a>
</p>
