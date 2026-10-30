# Aditya Ranjan

**CS @ Arizona State University (May 2027) · 3× Hackathon Winner · Open to Summer 2027 SWE / AI engineering internships**

I build AI systems and backend infrastructure for real users, with safety, privacy, and reliability designed in from the start: multi-agent products, LLM pipelines with guardrails, and idempotent event systems. Sports analytics and ML are a side interest.

---

## Award-Winning Projects

### Civilian

**Governance & Collaboration Track Winner — HackASU 2026 (sole winner in track)**

AI civic platform that turns a resident's complaint in any of 70+ languages into a formal government request with ordinance citations and automated follow-up.

Hard part: Claude-powered authority routing plus TinyFish agents that monitor silence and escalate when officials don't respond.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-gocivilian.org-22c55e?style=for-the-badge)](https://www.gocivilian.org)
[![Repo](https://img.shields.io/badge/Repo-Civilian-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Civilian)

### Redreemer

**State Farm Track Winner — Innovation Hacks 2.0**

SMS-based financial empowerment for people without smartphones, bank accounts, or stable addresses — an 8-step guided path from survival to financial independence.

Hard part: a 20-layer detection pipeline that routes crisis, scam, and benefits messages before Gemini ever responds.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-redreemer.vercel.app-22c55e?style=for-the-badge)](https://redreemer.vercel.app/)
[![Repo](https://img.shields.io/badge/Repo-redreemer--path--forward-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/redreemer-path-forward)

### Hirearchy

**Track 2 Winner — Cubbie Hackathon (Oct 2026)**

Multi-agent networking for student job hunts: each student has a personal AI agent, a broker sees only anonymized listings, and agents negotiate prep sessions and share interview intel, revealing names only after everyone consents. Deterministic code makes every decision; the LLM only words messages.

Built with Sumedha Gupta. I owned the Find, Ask, Pipeline, and Intel features plus the Discord and LLM integrations.

Hard part: privacy enforced in the data layer, not just the UI — company pipeline stats stay hidden until 3+ independent reports, interview reports are scrubbed of emails, phones, handles, and exact dates, and a sabotage suite plants identity leaks and fails if any slip through (357 tests across my suites).

[![Live Demo](https://img.shields.io/badge/Live%20Demo-hirearchy--agents.vercel.app-22c55e?style=for-the-badge)](https://hirearchy-agents.vercel.app)
[![Repo](https://img.shields.io/badge/Repo-sgupt354%2Fhirearchy--agents-181717?style=for-the-badge&logo=github)](https://github.com/sgupt354/hirearchy-agents)

---

## Featured Projects

### EventLedger

Idempotent event ingestion for retry-heavy order, claims, and webhook workflows: a retried request never creates a second durable event or runs the handler twice.

Hard part: layered dedup — a Postgres lookup for committed keys, Redis `SET NX` for in-flight requests, a `UNIQUE(idempotency_key)` constraint as the final race arbiter, and an atomic `received → processing` claim so only one worker owns an event. CI runs Postgres-backed integration tests via testcontainers; an AWS companion runs the same design on SQS + DynamoDB + Lambda.

[![Repo](https://img.shields.io/badge/Repo-eventLedger-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/eventLedger)
[![AWS Version](https://img.shields.io/badge/AWS%20Version-eventledger--aws-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://github.com/ARasugit20/eventledger-aws)

### Model Lineage Guard

DataHub-aware CLI agent with 9 risk checks (schema-hash drift, PII exposure, PII column classification, stale data, freshness SLA, missing owner, feature leakage, performance regression, deploy-config drift). Outputs JSON/HTML/Markdown reports and a `--fail-on` CI gate that blocks risky merges. Offline demo surfaces 11 findings in ~1.2s. Built for the DataHub Agent Hackathon.

Hard part: policy-gated write-back (irreversible tags need human review), deterministic finding IDs for risk diffing, and CI proof that dry-run never mutates.

[![Repo](https://img.shields.io/badge/Repo-Model--Lineage--Guard-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Model-Lineage-Guard)
[![View Sample Report](https://img.shields.io/badge/Sample%20Report-examples%2Fsample_report.html-blue?style=for-the-badge)](https://github.com/ARasugit20/Model-Lineage-Guard/blob/main/examples/sample_report.html)

---

## Also Built

### PlayerVec

PyTorch autoencoder that compresses World Cup player stats into 32-dim embeddings and rolls them into team style DNA for fixture matchup diagnosis.

Hard part: unsupervised player clustering without position labels, then minute-weighted squad fingerprints and FAISS search at scale.

[![Repo](https://img.shields.io/badge/Repo-PlayerVec-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/PlayerVec)

### Chronos

Event-driven quant research agent that ingests news and macro events, maps them to ticker themes, scores probability, and sizes positions with Kelly caps.

Hard part: end-to-end pipeline with Celery workers, Redis + Postgres dedup, calibration stubs, and half-Kelly risk controls — built on FastAPI, Celery, Redis, PostgreSQL, React, Docker, and Prometheus.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-chronos--frontend.onrender.com-22c55e?style=for-the-badge)](https://chronos-frontend.onrender.com)
[![Repo](https://img.shields.io/badge/Repo-Chronos-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Chronos)

### Career Signal

Role intelligence engine for CS students — pick a company and role, get a Signal Report with project ideas, JD keywords, and interview framing.

Hard part: static report generation from structured company/role data with optional Claude-backed AI mode and shareable report URLs.

[![Repo](https://img.shields.io/badge/Repo-Career--signal-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Career-signal)

---

## Tech

**Languages:** Python, TypeScript, Java, C/C++, SQL<br>
**Backend & data:** FastAPI, Node.js, PostgreSQL, Redis, Celery, Supabase<br>
**Frontend:** React, Next.js<br>
**AI/ML:** PyTorch, LLM APIs (Claude, Gemini), agent orchestration<br>
**Infra:** Docker, GitHub Actions, GCP, AWS (Lambda, SQS, DynamoDB)

---

## GitHub Activity

<p align="center">
  <img src="https://raw.githubusercontent.com/ARasugit20/ARasugit20/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake" width="90%" />
</p>

---

## Connect

- LinkedIn: [linkedin.com/in/aditya-ranjan-b9954730a](https://linkedin.com/in/aditya-ranjan-b9954730a)
- Email: [anola268@asu.edu](mailto:anola268@asu.edu)
