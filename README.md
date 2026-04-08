
# Hariom Dhage
 
**Software Engineer · Co-Founder · Systems Builder**
 
*Regulated industries. AI workflows. Low-latency infrastructure.*
 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hariom-dhage-20b18923b/)
[![Email](https://img.shields.io/badge/haiomdhage@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:haiomdhage@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HariomDhage)
 
</div>
 
---
 
## What I actually build
 
Most engineers write CRUD. I build systems where the data has legal weight — audit trails that can't be tampered, compliance workflows that map to regulatory clauses, execution pipelines where milliseconds matter.
 
Two tracks, running in parallel:
 
**→ AI × Compliance SaaS** — Co-founded and shipped two live B2B platforms from zero. One for enterprise sales teams, one for pharma regulatory teams. Real customers. Real data.
 
**→ Quantitative / Low-Latency Systems** — Re-architected production algo trading bots from Python to Rust + C++. Built a prediction market trading engine from scratch implementing GARCH, VPIN, Avellaneda-Stoikov from first principles.
 
---
 
## Live Products *(private repos — links below)*
 
<table>
<tr>
<td width="50%" valign="top">
 
### 🟦 [NovaFlow CRM](https://crm-hazel-theta.vercel.app/)
**AI-Powered Revenue Operating System**
 
Co-founded. Built the entire product.
 
B2B CRM with autonomous AI agents that research leads, score deals, and trigger follow-ups without human input. Visual pipeline with 18 customizable stages, omnichannel inbox, Jira-style ticketing, RBAC, and real-time collaboration.
 
`Next.js 15` `TypeScript` `Supabase` `PostgreSQL`
 
**What's under the hood:**
- Multi-tenant architecture with full data isolation
- AI Copilot via Cmd+K natural language commands
- 100+ integration layer (Gmail, Slack, WhatsApp, Stripe)
- Real-time subscriptions across deal lifecycle events
 
</td>
<td width="50%" valign="top">
 
### 🟩 [DueVault](https://aiops-delta.vercel.app/)
**AI-Powered Pharma Compliance Platform**
 
Co-founded with Dr. Balaji Ommurugan (15+ yrs Novartis/Organon). Built the entire technical stack.
 
Continuous compliance monitoring that scans your systems every hour, maps evidence to regulatory controls (21 CFR Part 11, ICH Q10, EU GMP, HIPAA and 6 more), and generates audit packages before the auditor calls.
 
`Next.js` `TypeScript` `Supabase` `Azure OpenAI`
 
**What's under the hood:**
- 4 specialized AI agents (Validation, Compliance, QA, Knowledge)
- RAG over SOPs — returns answers with exact citations
- Immutable audit trail — compliant even with expired licenses
- AES-256 + RLS + Zero-trust architecture + on-premise ready
 
</td>
</tr>
</table>
 
---
 
## Selected Projects
 
### ⚡ NEXUS — Prediction Market Quantitative Trading Engine
`Rust` `Tokio` `REST/WebSocket APIs`
 
8-crate Rust workspace scanning all live Polymarket contracts for alpha across three layers:
 
| Layer | Signal | Method |
|---|---|---|
| 1 | Zero-risk completeness arbitrage | YES + NO < $1 detection |
| 2 | Crypto lag detection | Log-normal GBM: P(ST > K) = N(d₂) vs live Coinbase |
| 3 | Longshot bias exploitation | 60%+ documented overpricing on sub-$0.08 contracts |
 
Implemented from scratch in pure Rust: **GARCH(1,1)** volatility forecasting, **VPIN** informed-flow detection, **Avellaneda-Stoikov** optimal market-making, **half-Kelly** position sizing — all operating in log-odds space for bounded [0,1] market prices. Scanner produces 15–20 ranked signals per cycle with execution instructions.
 
Architecture: `core` · `signals` · `backtest` · `risk` · `sentiment` · `execution` · `data` · `runner` — async Tokio runtime, zero-copy serde deserialization.
 
---
 
### 🏦 AlphaSentiment — Multi-Agent AI Signal Pipeline
`Python` `FastAPI` `PostgreSQL` `Docker`
 
Multi-step AI pipeline feeding signals into execution engines. Per-step latency monitoring, structured logging, validation, retries, and cost-aware rate scheduling. Containerized for reproducible production deployment.
 
---
 
### 🔐 TeamSync — Multi-Tenant SaaS Backend
`Node.js` `TypeScript` `PostgreSQL` `Redis` `Docker`
 
Production-grade multi-tenant infrastructure: tenant isolation, RBAC, API key management, rate limiting, background jobs, audit logging, and partition strategies for high-throughput query performance.
 
---
 
## Work Experience
 
**Software Engineer — Encurex** *(2025 – Present)*
*Cybersecurity · Enterprise IAM Platform*
 
Building a full-stack Identity & Access Management platform with 15+ modular services for enterprise customers. Highlights:
- Engineered breach monitoring via HIBP API + Redis caching → **95% fewer API calls**
- Implemented zero-runtime type-safe API client from OpenAPI schema via codegen — eliminated all manual API code
- Immutable audit log infrastructure for all permission events (actor, target, IP, session, delta)
- Multi-stage access review workflows with automatic approval routing and recurring compliance sign-off
 
---
 
**Quant / Systems Engineer — Orgax LLC** *(Nov 2024 – Jan 2025)*
*U.S. Algorithmic Trading Startup*
 
Re-architected production trading bots (Gold futures + BTC) from Python/C++ hybrid to **pure Rust + C++ stack** — eliminating interpreter overhead, cutting order-placement latency materially. Designed the full hot path: tick ingestion → signal computation → order dispatch. Profiled with flamegraphs + perf, replaced bottlenecks with zero-copy Rust via FFI. Contributed to ML signal integration while maintaining deterministic latency bounds.
 
---
 
**Software Engineer — The Linux Foundation (LFX'25)** *(Jun – Nov 2025)*
*Open Source · Hyperledger Labs*
 
Built REST APIs and Java SDKs for edX, Moodle, and Canvas LMS platforms. **Reduced API latency 40%** through profiling, caching, and algorithmic optimization. Implemented DLT (blockchain) integration with deterministic audit logging for high-traffic systems.
 
---
 
**Full-Stack Engineer — Quantummosaic** *(2024 – 2025)*
*U.S. Private Capital Firm*
 
Shipped a production platform (React + TypeScript + FastAPI + Node.js) end-to-end — dev through staging to production with rollback support. Optimized PostgreSQL queries, implemented caching layers, owned full deployment lifecycle.
 
---
 
## Tech Stack
 
**Core**
 
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++17/20-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
 
**Data & Infrastructure**
 
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
 
**AI / LLM**
 
![OpenAI](https://img.shields.io/badge/Azure_OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
`RAG · Embeddings · Prompt Engineering · Agentic Workflows`
 
**Quant / Systems**
 
`GARCH(1,1)` `VPIN` `Avellaneda-Stoikov` `Kelly Criterion` `Log-normal GBM` `CLOB Order Books` `Lock-free Data Structures` `Low-latency Design` `Tokio async` `FFI`
 
**Product & Compliance**
 
`Multi-Tenancy` `RBAC` `Audit Trail Design` `21 CFR Part 11` `GxP` `HIPAA` `SOC 2` `OpenAPI Codegen` `CI/CD` `Playwright E2E` `TanStack Query`
 
---
 
## Education
 
| | Institution | Degree | GPA |
|---|---|---|---|
| 🎓 | **University of Mumbai** | B.E. Electronics & Communication | **8.45 / 10** |
| 🎓 | **IIT Madras** | B.S. Data Science & Applications | **7.0 / 10** |
 
---
 
## Recognition
 
🏆 **Winner — Cognitia'25** &nbsp;·&nbsp; ⭐ **GSEA Finalist** &nbsp;·&nbsp; ⭐ **Eureka Semi-Finalist**
🥈 **MindShift Runner-Up** &nbsp;·&nbsp; 🎖️ **Microsoft Learn Student Ambassador** &nbsp;·&nbsp; 🔧 **Technical Officer — ISTE VESIT**
 
---
 
<div align="center">
 
**Open to founding-team roles, high-conviction early-stage companies, and interesting hard problems.**
 
[haiomdhage@gmail.com](mailto:haiomdhage@gmail.com) · +91-8080283122
 
</div>
