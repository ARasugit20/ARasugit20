# Aditya Ranjan

Builder focused on **data pipelines**, **ML with honest evaluation**, and **full-stack systems** where the README matches what is in the repo.

---

## Award-Winning Project

### Redreemer

**State Farm Track Winner — Innovation Hacks 2.0**

Hackathon-winning **caseworker console and marketing site** (React, Vite, shadcn/ui) for a financial-independence concept aimed at caseworkers supporting unhoused and re-entry clients.

What ships today: dashboard UI with hardcoded `MOCK_CLIENTS`, landing pages, and Vitest coverage on the frontend — **not wired to a live backend or outbound messaging**.

[![Repo](https://img.shields.io/badge/Repo-redreemer--path--forward-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/redreemer-path-forward)

---

## Featured Projects

Projects below are written to survive a click-through. Each claim maps to code in the linked repo.

### eventLedger

Idempotent event-ingestion API: Redis `SET NX` fast dedupe, Postgres `UNIQUE(idempotency_key)` durable dedupe, Redis Streams workers, and a Postgres-backed DLQ after max delivery attempts.

Hard part: concurrency proof — 50 parallel POSTs with the same idempotency key yield exactly one persisted event (`tests/test_concurrency.py`).

[![Repo](https://img.shields.io/badge/Repo-eventLedger-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/eventLedger)

### CreditRisk_

Credit default modeling with an explicit leakage story: dbt-DuckDB warehouse → feature mart → temporal holdout XGBoost with post-origination columns stripped via `LEAKAGE_COLUMNS` and enforced in `tests/test_no_leakage.py`.

Hard part: temporal ROC AUC **0.707** on held-out vintages (`results/temporal_metrics.json`) — not the ~0.99 figures that appear only in narrative docs without a paired before-metrics artifact.

[![Repo](https://img.shields.io/badge/Repo-CreditRisk_-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/CreditRisk_)

### Model-Lineage-Guard

DataHub-aware CLI that scans ML lineage for schema drift, PII exposure, feature leakage, and related production risks; writes audit tags back and exits **code 3** for CI gating with `--fail-on`.

Hard part: live CI boots DataHub, seeds demo lineage, runs scan + write-back verification (`.github/workflows/ci.yml`).

[![Repo](https://img.shields.io/badge/Repo-Model--Lineage--Guard-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Model-Lineage-Guard)

### Civilian

**Governance & Collaboration Track Winner — HackASU 2026 (sole winner in track)**

Shipped civic web app: compose a complaint → Claude analysis with web search → formal letter → InsForge persistence → echo/forum/map views. Translation via Claude for 72 compose languages.

Hard part: end-to-end flow under hackathon constraints; forum still merges static demo threads with live DB posts (`lib/civicData.js`).

[![Live Demo](https://img.shields.io/badge/Live%20Demo-gocivilian.org-22c55e?style=for-the-badge)](https://www.gocivilian.org)
[![Repo](https://img.shields.io/badge/Repo-Civilian-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Civilian)

### Chronos

Event-driven quant research stack (FastAPI, Celery, PostgreSQL, Redis, React dashboard): ingest events, score with LightGBM + isotonic calibration, size with half-Kelly caps.

Hard part: committed fixture `resolved_predictions.json` reports **Brier 0.2167 on n=28** resolved decisions (`docs/outcomes.md`) — **mock price track**, calibration quality not trading P&L; default deploy uses mock news and mock prices.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-chronos--frontend.onrender.com-22c55e?style=for-the-badge)](https://chronos-frontend.onrender.com)
[![Repo](https://img.shields.io/badge/Repo-Chronos-181717?style=for-the-badge&logo=github)](https://github.com/ARasugit20/Chronos)

---

## Tech

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

---

## GitHub Stats

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=ARasugit20&theme=radical" alt="GitHub stats" width="49%" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=ARasugit20&theme=radical" alt="Top languages" width="49%" />
</p>

---

## Connect

- LinkedIn: [linkedin.com/in/aditya-ranjan-b9954730a](https://linkedin.com/in/aditya-ranjan-b9954730a)
- Email: [anola268@asu.edu](mailto:anola268@asu.edu)
