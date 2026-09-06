<div align="center">

# Sammeyak Wankhade
### Software Development Engineer — Full-Stack

<a href="mailto:wankhadesammeyak@gmail.com"><img src="https://img.shields.io/badge/Email-wankhadesammeyak%40gmail.com-333333?style=flat-square&logo=gmail&logoColor=white" /></a>
<a href="https://linkedin.com/in/sammeyak-wankhade"><img src="https://img.shields.io/badge/LinkedIn-Sammeyak%20Wankhade-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
<a href="https://github.com/Sammeyak797"><img src="https://img.shields.io/badge/GitHub-Sammeyak797-181717?style=flat-square&logo=github&logoColor=white" /></a>
<a href="https://portfolio-ebon-two-89.vercel.app"><img src="https://img.shields.io/badge/Portfolio-Visit-000000?style=flat-square&logo=vercel&logoColor=white" /></a>

</div>

<br/>

## About

Full-stack engineer building production backend systems and the APIs/UIs on top of them. Currently at **Cooee**, working across the stack — from API design and database migrations to query optimization at scale. Comfortable owning a problem end-to-end: customer-facing UI, backend services, and the infrastructure underneath.

- 🔧 Backend & distributed systems: Node.js/NestJS, PostgreSQL, MongoDB, ClickHouse, Redis, Kafka, BullMQ
- 🎨 Frontend: React, Angular, TypeScript
- 📍 Based in Pune, India
- 🎓 B.E. Information Technology, Sinhgad College of Engineering (CGPA 8.60/10, 2026)

<br/>

## Experience

**Software Development Engineer (Full-Stack) — Cooee** · *Feb 2026 – Present*

- Owned a Shopify app feature (customer- and admin-facing) that injects global CSS into the document head to dynamically restyle native storefront elements for on-site conversion optimization.
- Migrated the analytics data store from **MongoDB to ClickHouse** — rewrote Mongo queries into ClickHouse SQL and consolidated three separate API calls into a single endpoint backed by one query.
- Diagnosed an **N+1 query issue** in the subscription module (~120 queries/request, ~800ms avg latency); replaced it with a MongoDB aggregation pipeline (`$lookup`), cutting response time to ~480ms (**40% faster**).
- Optimized a GraphQL flow fetching a single product's data through multiple redundant queries, consolidating it into one batched query and cutting unnecessary network round-trips.
- Root-caused a production incident where retried payment webhooks were processed twice and corrupted subscription state; fixed with **idempotency keys and transactional updates**, eliminating recurrence.

<br/>

## Tech Stack

<div align="center">

**Languages**
<br/>
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Backend & APIs**
<br/>
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)

**Frontend**
<br/>
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Data & Messaging**
<br/>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge&logo=clickhouse&logoColor=black)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Infra & Observability**
<br/>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**Testing & Security**
<br/>
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

</div>

<br/>

## Featured Projects

### [Distributed Job Processing & Notification Platform](https://github.com/Sammeyak797)
`NestJS` `BullMQ` `PostgreSQL` `Redis` `Docker`
- Built durable job execution using BullMQ + Redis with concurrency-based workers, cutting processing time **~60%** vs. synchronous execution; failed jobs auto-retry up to 4 times with exponential backoff before moving to a dead-letter queue.
- Designed the full job lifecycle (API → PostgreSQL → BullMQ/Redis → worker → status update), simulating failures to validate retry/DLQ handling; containerized with Docker Compose, deployed to AWS EC2, monitored throughput and failure rates with Prometheus.

### [Subscription & Billing Service](https://github.com/Sammeyak797)
`NestJS` `React` `TypeScript` `PostgreSQL` `Redis` `BullMQ`
- Architected a multi-tenant billing system (plans, invoices, proration, webhook-driven payment transitions) using idempotency keys and PostgreSQL transactions to prevent duplicate charges and guarantee atomicity.
- Built a React/TypeScript admin dashboard — MRR, active-subscription, and plan-distribution charts (Recharts), a searchable/paginated customer list, and an upgrade/downgrade flow validated with React Hook Form + Zod, kept fresh via TanStack Query.

### [Real-Time Analytics & Event Pipeline](https://github.com/Sammeyak797)
`NestJS` `WebSockets` `Kafka` `MongoDB` `Redis` `Docker`
- Built a real-time event pipeline tracking page-view, purchase, and signup events end-to-end: ingested via Kafka topics for durable, partitioned storage across multiple consumers, persisted raw events in MongoDB, and maintained live aggregate counters in Redis.
- Benchmarked ingestion with a custom Node.js/TypeScript load generator (5,000 requests, 50 concurrent/batch), sustaining **~1.16K req/sec** at 100% success and ~25ms avg latency; built a live dashboard (Socket.IO) broadcasting metric updates with no page refresh.

<details>
<summary><b>Other Projects</b></summary>
<br/>

| Project | Stack |
|---|---|
| [Scalable URL Shortener with Analytics](https://github.com/Sammeyak797/url-shortener) | Flask, MongoDB, Redis, JWT |
| [Smart CNC Predictive Maintenance](https://github.com/Sammeyak797/smart-cnc-predictive-maintenance) | Python, IoT, Data Processing |
| [Plant Disease Detection System](https://github.com/Sammeyak797/Plant-Disease-Detection-System-for-Sustainable-Agriculture) | TensorFlow, Keras, OpenCV, Streamlit |

</details>

<br/>

## Achievements

- 🧩 Solved **500+ DSA problems** across coding platforms, primarily LeetCode
- 🏆 **Top 10**, Smart India Hackathon — University-level round
- 📈 **GATE 2026 (CS)** — AIR 15,000

<br/>

## GitHub Stats

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Sammeyak797&show_icons=true&theme=default&hide_border=true&count_private=true&rank_icon=github" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sammeyak797&layout=compact&hide_border=true&langs_count=8" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=Sammeyak797&hide_border=true" />
</div>

<br/>

<div align="center">

📫 **Open to full-time SDE / Backend Engineer roles** — reach out at [wankhadesammeyak@gmail.com](mailto:wankhadesammeyak@gmail.com)

</div>
