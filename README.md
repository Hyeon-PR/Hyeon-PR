<div align="center">

  # HyeonJun Lee
  ### AI Product Engineer — LLM serving & agent pipelines in production
  Co-founder & Tech Lead @ Tecketing · CS @ DGIST (on leave)

  <p>I build the systems around LLMs — gates, validators, routing, observability —<br>so the product doesn't depend on the model behaving.</p>

  <a href="mailto:lhbj1115@gmail.com"><img src="https://img.shields.io/badge/Email-00B4AB?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/hyeon-dev/"><img src="https://img.shields.io/badge/LinkedIn-00B4AB?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://hyeondev.blogspot.com/"><img src="https://img.shields.io/badge/Blog-00B4AB?style=for-the-badge&logo=blogger&logoColor=white" alt="Blog" /></a>

</div>

---

## 🔍 Now building — Sleuth

An AI mystery game where players interrogate AI suspects to solve crime-scene cases. Live on iOS and Android since June 2026.
I own the backend: LLM serving, an agent-driven content pipeline (one session taking designer, writer, and reviewer roles in turn), and payments.

<a href="https://apps.apple.com/kr/app/id6759363417"><img src="https://img.shields.io/badge/App_Store-000000?style=flat-square&logo=appstore&logoColor=white" alt="App Store" /></a>
<a href="https://play.google.com/store/apps/details?id=com.sleuth.fictionflare"><img src="https://img.shields.io/badge/Google_Play-000000?style=flat-square&logo=googleplay&logoColor=white" alt="Google Play" /></a>

| 755 | 37m 38s | +52% |
|:---:|:---:|:---:|
| active users, last 90 days | avg. engagement per user | weekly actives, week over week<br>(156 → 237 during our Wadiz campaign) |

<sub>GA4, as of Sep 26, 2026</sub>

---

## 🧭 How I build with LLMs

**Constrain agents with code, not prompts.**
Our authoring agents started approving their own checkpoints. Now checkpoint transitions go through a deterministic gate that re-runs the validator itself instead of trusting the agent's report. → [write-up](https://hyeondev.blogspot.com/2026/08/blog-post.html)

**Decide with production data.**
A 50/50 production A/B test rejected a model swap that looked right on paper (p95 1.5 s → 4.5 s, +57% cost per call). The same test showed our cross-model fallback recovering 82 of 83 paid requests during a provider outage.

**Make money paths exactly-once.**
Idempotency keys plus Firestore transactions: zero double charges across 60 runs of 20 concurrent same-user S-coin spend requests (test env). Requests that can never succeed are quarantined instead of retried forever. → [write-up](https://hyeondev.blogspot.com/2026/09/part-3.html)

**Tie cost to the right variable.**
Designed the notification inbox so cost grows with active users, not with subscriber count. → [write-up](https://hyeondev.blogspot.com/2026/06/fan-out-on-write-vs-fan-out-on-read.html)

---

## 🏢 Beyond code

Co-founded Tecketing in 2024 and ran it as CEO until 2026, then moved to Tech Lead.
6 startup competition awards · KOCCA commercialization program · GSIA 2026 Seattle global program · 61 straight weekly sprints

---

## 🛠️ Stack

![Python](https://img.shields.io/badge/Python-00B4AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-00B4AB?style=flat-square&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-00B4AB?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-00B4AB?style=flat-square&logo=node.js&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex_AI-00B4AB?style=flat-square&logo=googlecloud&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-00B4AB?style=flat-square)
![Claude Code](https://img.shields.io/badge/Claude_Code-00B4AB?style=flat-square&logo=claude&logoColor=white)
![Cloud Run](https://img.shields.io/badge/Cloud_Run-00B4AB?style=flat-square&logo=googlecloud&logoColor=white)
![Firestore](https://img.shields.io/badge/Firestore-00B4AB?style=flat-square&logo=firebase&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-00B4AB?style=flat-square&logo=googlebigquery&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-00B4AB?style=flat-square&logo=flutter&logoColor=white)

---

## ✍️ Featured Writing <sub>(in Korean)</sub>

- [Game scenarios: from outsourcing to our own pipeline](https://hyeondev.blogspot.com/2026/08/blog-post.html) — moving scenario authoring from outsourcing to a gated agent pipeline
- [In-app payments, Part 3: the problems that start after verification succeeds](https://hyeondev.blogspot.com/2026/09/part-3.html)
- [FastAPI and cloud native, Part 1](https://hyeondev.blogspot.com/2026/03/fastapi-llm-part-1.html) — why LLM calls moved to the server

<details>
<summary><b>More</b> — earlier projects & problem solving</summary>
<br>

- [OctaFlip](https://github.com/Hyeon-PR/OctaFlip) — real-time 2-player board game server in C over TCP sockets with a JSON protocol
- Autonomous-driving research — CARLA simulation, lane tracing, Jetson / F1TENTH ([Learning_AD](https://github.com/Hyeon-PR/Learning_AD))
- 3D motion automation (with © BLUE BONFIRE) — Python pipeline for lip-sync retargeting in Cinema 4D

<a href="https://solved.ac/lhbj1115"><img src="http://mazassumnida.wtf/api/v2/generate_badge?boj=lhbj1115" alt="Solved.ac Profile" /></a>
</details>

---

### Latest Blog Posts

- [[스타트업/기술] Sleuth 프로토타입에서 프로덕션까지 | 전체 포스팅 모음](https://hyeondev.blogspot.com/2026/09/sleuth.html)
- [[스타트업/기술] 에이전트의 Self-approval 문제 | LLM 저작 파이프라인을 결정론적 게이트로 막다](https://hyeondev.blogspot.com/2026/09/self-approval-llm.html)
- [[42 글로벌프로그램] 다시 미국에 오다 - (3편/완결)](https://hyeondev.blogspot.com/2026/09/42-3.html)
- [추리 게임 시나리오, 외주에서 자체 파이프라인으로](https://hyeondev.blogspot.com/2026/08/blog-post.html)
- [[42 글로벌프로그램] 다시 미국에 오다 - (2편)](https://hyeondev.blogspot.com/2026/08/42-2.html)

