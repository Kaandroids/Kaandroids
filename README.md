<h1 align="center">Kaan Kara</h1>

<p align="center">
  <strong>Full-Stack Software Engineer</strong> &nbsp;·&nbsp; Java &nbsp;·&nbsp; Spring Boot &nbsp;·&nbsp; Angular
</p>

<p align="center">
  I design and ship production-grade web applications end to end — from the data model and<br/>
  execution engine on the backend to the reactive UI and the cloud deployment I own myself.<br/>
  I care about clean architecture, multi-tenant isolation, observability, and infrastructure-as-code.
</p>

<p align="center">
  🚀 Building <a href="https://postwerk.io"><strong>Postwerk</strong></a> — an AI-driven email automation platform &nbsp;·&nbsp; 🌍 Germany
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/kaan-kara-0a720439b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:kaan403@icloud.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://postwerk.io"><img src="https://img.shields.io/badge/Website-postwerk.io-1F88C0?style=flat&logo=googlechrome&logoColor=white" alt="Website" /></a>
</p>

---

## 🚀 Featured Project — Postwerk

> **AI-Powered Email Automation Platform.** Build visual, drag-and-drop workflows that classify, extract, reply, forward, and act on your emails — powered by Google Gemini. Live in open beta at **[postwerk.io](https://postwerk.io)**.

<p align="center">
  <a href="https://github.com/Kaandroids/Postwerk">
    <img src="https://raw.githubusercontent.com/Kaandroids/Postwerk/main/doc/screenshots/demo.gif" width="100%" alt="Postwerk — building an email automation with the AI assistant" />
  </a>
</p>
<p align="center"><em>Building &amp; running an email automation with the AI assistant — no code.</em></p>

**Engineering highlights**

- ⚙️ **DAG automation engine** — automations are graphs of 15 typed node types run by a single executor (not a giant switch), with supervised execution (`AUTO` / `REVIEW` / `OFF`), dry-run per-node tracing, and recursive reusable sub-flows.
- 🤖 **Conversational AI builder** — a typed tool registry exposed to Gemini behind an `OPEN → PLANNING → BUILDING` phase machine, so the assistant safely modifies a live automation from natural language.
- 🔍 **Hybrid semantic search** — pgvector cosine similarity fused with Postgres full-text via **reciprocal rank fusion**, gated by an LLM match-judge.
- 🏢 **Multi-tenant SaaS** — organizations as tenants, org-scoped at the query level, RBAC + JWT, plan-based AI quotas, GDPR data retention &amp; audit logging.
- 🔐 **Keyless CI/CD** — GitHub Actions builds each image once and ships to GCP on merge with **zero long-lived credentials** (Workload Identity Federation / OIDC, IAP-tunnelled SSH, health-gated auto-rollback).

<p>
  <img src="https://img.shields.io/badge/Spring_Boot-3.4-6DB33F?logo=springboot&logoColor=white" alt="Spring Boot 3.4" />
  <img src="https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white" alt="Java 21" />
  <img src="https://img.shields.io/badge/Angular-19-DD0031?logo=angular&logoColor=white" alt="Angular 19" />
  <img src="https://img.shields.io/badge/PostgreSQL-17_+_pgvector-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL 17 + pgvector" />
  <img src="https://img.shields.io/badge/Redis-7-DC382D?logo=redis&logoColor=white" alt="Redis 7" />
  <img src="https://img.shields.io/badge/Gemini-AI-4285F4?logo=google&logoColor=white" alt="Google Gemini" />
  <img src="https://img.shields.io/badge/Terraform-IaC-7B42BC?logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/GCP-Cloud-4285F4?logo=googlecloud&logoColor=white" alt="GCP" />
</p>

**[🌐 Live Demo](https://postwerk.io)** &nbsp;·&nbsp; **[📂 Source &amp; Full Docs](https://github.com/Kaandroids/Postwerk)**

---

## 🧰 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Backend** | ![Java](https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.4-6DB33F?logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-JWT-6DB33F?logo=springsecurity&logoColor=white) ![Resilience4j](https://img.shields.io/badge/Resilience4j-Circuit_Breaker-orange) |
| **Frontend** | ![Angular](https://img.shields.io/badge/Angular-19-DD0031?logo=angular&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white) ![RxJS](https://img.shields.io/badge/RxJS-Reactive-B7178C?logo=reactivex&logoColor=white) ![SCSS](https://img.shields.io/badge/SCSS-Styling-CC6699?logo=sass&logoColor=white) |
| **Data &amp; Cache** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-4169E1?logo=postgresql&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-Embeddings-4169E1) ![Redis](https://img.shields.io/badge/Redis-7-DC382D?logo=redis&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-Migrations-CC0000?logo=flyway&logoColor=white) |
| **AI** | ![Gemini](https://img.shields.io/badge/Google_Gemini-2.5-4285F4?logo=google&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude_Code-CLI-black?logo=anthropic&logoColor=white) |
| **Cloud &amp; DevOps** | ![GCP](https://img.shields.io/badge/GCP-Compute_Engine-4285F4?logo=googlecloud&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-Cloud-0089D6?logo=microsoftazure&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-IaC-7B42BC?logo=terraform&logoColor=white) ![Caddy](https://img.shields.io/badge/Caddy-Auto_HTTPS-1F88C0?logo=caddy&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/CI/CD-Actions-2088FF?logo=githubactions&logoColor=white) |
| **Observability** | ![Prometheus](https://img.shields.io/badge/Prometheus-Metrics-E6522C?logo=prometheus&logoColor=white) ![Micrometer](https://img.shields.io/badge/Micrometer-Tracing-117A8B) ![Actuator](https://img.shields.io/badge/Spring_Actuator-Health-6DB33F?logo=springboot&logoColor=white) |
| **Testing** | ![JUnit5](https://img.shields.io/badge/JUnit5-25A162?logo=junit5&logoColor=white) ![Testcontainers](https://img.shields.io/badge/Testcontainers-Integration-291A3A?logo=testcontainers&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-E2E-2EAD33?logo=playwright&logoColor=white) ![Vitest](https://img.shields.io/badge/Vitest-Unit-6E9F18?logo=vitest&logoColor=white) |

---

## 🛠️ Other Projects

| Project | Description | Stack | Links |
| :--- | :--- | :--- | :--- |
| **Brief-Fix** | DIN 5008-compliant German letter generator with AI-assisted composition and window-envelope-ready PDF rendering. | Spring Boot · Angular · Gemini · Cloud Run | [Live](https://www.brief-fix.de/) · [Frontend](https://github.com/Kaandroids/Brieffix-Frontend) · [Backend](https://github.com/Kaandroids/Brieffix-Backend) |
| **2Do** | Cloud-native task management with Redis-backed JWT blacklisting, rate limiting, and Azure deployment. | Spring Boot · Angular · Redis · Azure | [Live](https://gentle-cliff-06c31ee03.6.azurestaticapps.net/) · [Frontend](https://github.com/kaandroids/2Do-frontend) · [Backend](https://github.com/kaandroids/2Do-backend) |
| **Legacy MauMau** | My first app (2021) — a 100% human-made card game, zero AI, lots of late-night debugging at Uni Hannover. | Java | [Code](https://github.com/Kaandroids/Legacy-MauMau-CardGame) |

---

## 🤖 On Using AI Tools

I use **Claude Code** and **Gemini** as part of my daily workflow — not as autopilots, but as tools I direct with intent.

- I own the architecture. Every structural and design decision is mine.
- I review all AI-generated code before it goes anywhere near a codebase.
- No vibe coding. I understand what I ship.

AI accelerates the work. It doesn't replace the thinking.

---

## 📬 Connect

<p>
  <a href="https://www.linkedin.com/in/kaan-kara-0a720439b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:kaan403@icloud.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://postwerk.io"><img src="https://img.shields.io/badge/Postwerk-1F88C0?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Postwerk" /></a>
</p>
