<h1 align="center">Dmitry Grebenshchikov</h1>
<h3 align="center">Tech Lead · Engineering Manager · Python Backend Architect</h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=2E9EF7&center=true&vCenter=true&width=650&lines=17%2B+years+shipping+backend+systems+at+scale;Built+and+led+engineering+teams+from+0+to+12;FastAPI+%C2%B7+Kubernetes+%C2%B7+event-driven+architecture;AI-native+engineering+with+Claude+Code+%2B+spec-driven+dev" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/grebenshchikov/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://career.habr.com/mtizima"><img src="https://img.shields.io/badge/Habr%20Career-65A3BE?style=for-the-badge" alt="Habr Career"></a>
  <a href="https://t.me/mtizima"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"></a>
  <a href="mailto:meathmc@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<p align="center"><sub>🇷🇺 Резюме на русском: <a href="https://career.habr.com/mtizima">career.habr.com/mtizima</a></sub></p>

---

## About

Backend engineer and engineering leader with **17+ years of experience**, the last 5 as **Tech Lead / Engineering Manager** for FemTech and FinTech products serving **200K-500K+ active users**. I design event-driven, horizontally scalable systems, build engineering teams from zero, and ship infrastructure that stays fast under real production load.

- 🏗️ **Architecture:** event-driven microservices, hexagonal architecture, zero-downtime Kubernetes migrations, monoliths when that's the correct call
- 👥 **Leadership:** hired and mentored teams up to 12 engineers across 4 time zones, grew 4 Middle engineers to Senior on my last team
- ⚡ **Impact:** cut API latency 200ms → 120ms, doubled delivery velocity, sped up release cadence 30%, shipped real-time analytics for 200K+ users
- 🤖 **AI-native engineering:** spec-driven development with Claude Code, production LangChain/LangGraph agent workflows

---

## Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,django,flask,postgres,redis,kafka,docker,kubernetes,aws,azure,grafana,prometheus,elasticsearch,git,go,nodejs,terraform" alt="Skills" />
</p>

| | |
|---|---|
| **Languages & Runtime** | Python (asyncio), Go, Node.js |
| **Backend & APIs** | FastAPI, Django, Flask, aiohttp, aiogram, REST |
| **Data & Messaging** | PostgreSQL, ClickHouse, MongoDB, Redis, Kafka, RabbitMQ, NATS JetStream, SQLAlchemy, Elasticsearch |
| **Infrastructure** | Kubernetes, Docker, Terraform, Ansible, AWS, Azure, GitLab CI, Prometheus, Grafana |
| **AI / LLM Tooling** | Claude Code, LangChain, LangGraph, OpenAI API, spec-driven development |

---

## Featured Work

### TaskAI: AI-native Telegram task management platform
**Founder & Fullstack Engineer** · 2026-present · [task24.online](https://task24.online)

A production SaaS built on one idea: **one Telegram supergroup = one team, one topic = one task**. Tasks are created by voice message, transcribed, reformatted, and titled through an LLM pipeline, with automatic topic creation, a closed-task archive, weekly AI-generated performance summaries, and recurring billing via Telegram Stars, bank cards, and SBP.

- Event-driven architecture: the API publishes to **NATS JetStream**; isolated **FastStream** workers run the full voice-to-task pipeline
- Analytics subsystem built on atomic incremental SQL instead of ORM read-modify-write, with materialized views and a log-based fallback recompute
- Application-level **envelope encryption (AES-256-GCM)** for user content, applied transparently via a SQLAlchemy `TypeDecorator`
- Recurring Telegram Stars billing and a rate-limited broadcast pipeline built around Bot API limits
- Built iteratively with **Claude Code** as a pair-engineering partner: spec first, reviewed, then shipped

`Python 3.12` `FastAPI` `aiogram 3` `FastStream` `NATS JetStream` `PostgreSQL 16` `SQLAlchemy 2.0` `Redis` `Docker` `OpenAI Whisper`

<sub>Private repository. Architecture walkthrough available on request.</sub>

### Cashier & Kitchen Ordering Bot
**Backend Engineer (independent)** · Telegram-based POS for food service

An order-lifecycle system for a food business: cashiers place orders from Telegram, kitchen staff get real-time notifications, and the product catalog imports from CSV. Built end-to-end with **Claude Code**, from spec and implementation plan through production deploy and bug fixes.

- Order lifecycle service (create → ready → issued) with per-recipient notification isolation, so one unreachable chat never blocks the rest of the kitchen
- SQLAlchemy models for products and orders, CSV catalog ingestion with validation
- Deployed on Render with managed Postgres

`Python` `aiogram` `SQLAlchemy` `PostgreSQL` `Render`

<sub>Private repository. Architecture walkthrough available on request.</sub>

### Womanly: FemTech Wellness Platform
**Tech Lead** · Python, Flutter, FastAPI · 200K+ active users

- Led a zero-downtime migration to **Kubernetes**, raising platform availability from 60% to 80%
- Migrated **Sanic → FastAPI**, cutting p50 response time 200ms → 120ms while doubling delivery speed
- Integrated **PowerBI + Grafana** for real-time analytics across 200K+ active users
- Restructured code review and CI/CD, increasing release velocity by 30%

### amma family: Pregnancy Tracker
**Head of Python Development → Tech Lead** · scaled to 500K+ users

- Designed a scalable architecture for medical data processing on Django + FastAPI, lifting throughput 50%
- Built a backend team from scratch: hired, onboarded, and mentored engineers to Senior level
- Promoted to Tech Lead for an international 12-person team (mobile, QA, DevOps, backend) across 4 time zones
- Rebuilt the backend on Django + Redis microservices, tripling throughput

### Litres: Digital Books Platform
**Head of Python Development** · 2021 · [litres.ru](https://www.litres.ru)

- Led the migration from a legacy Perl monolith to a Python microservices architecture
- Introduced hexagonal architecture to decouple domain logic from delivery and infrastructure concerns
- Built integration services for 15+ partners
- Sped up catalog search 50% across a 1M+ book catalog using Elasticsearch

`Python` `FastAPI` `MySQL` `ClickHouse` `Kafka` `Elasticsearch` `Kubernetes`

### Anna Money: UK FinTech, Business Banking
**Senior Python Developer** · 2018-2021 · [anna.money](https://anna.money)

- Led a team of 5 building antifraud and AML (anti-money-laundering) services for live transaction flows
- Coordinated integrations with external providers including Global Processing Services and Dow Jones
- Owned technical design end-to-end on asyncio/aiohttp, Kubernetes/Mesos, and RabbitMQ messaging

`Python` `asyncio` `aiohttp` `PostgreSQL` `Kubernetes` `RabbitMQ` `MongoDB`

---

## Open Source

**[adjust-client](https://github.com/mtizima/adjust-client)**: Python client for the Adjust.com server-to-server (S2S) event API.

---

## GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats-git-master-rickstaa.vercel.app/api?username=mtizima&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
  <img height="165" src="https://streak-stats.demolab.com?user=mtizima&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

---

<p align="center"><i>Open to Tech Lead / Staff Engineer roles, remote-first, worldwide.</i></p>
