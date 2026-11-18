# Kaan Kara

**Full-Stack Software Engineer** &nbsp;·&nbsp; Java &nbsp;·&nbsp; Spring Boot &nbsp;·&nbsp; Angular &nbsp;·&nbsp; React Native

I build web and mobile applications end to end: the data model, the backend logic, the UI and the deployment. I care about clear architecture, decisions that are written down, and code I fully understand.

🌍 Hannover, Germany &nbsp;·&nbsp; Open to Java / Spring Boot roles across Germany

<p>
  <a href="https://kaandroids.dev"><img src="https://img.shields.io/badge/Website-kaandroids.dev-1F2937?style=flat&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/kaan-kara-0a720439b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:kaan403@icloud.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

## 🏋️ Benchbite — workouts and nutrition in one app

> A mobile app that builds a training and nutrition plan from a few questions, logs workouts on the phone and the Apple Watch, and comes with **Bite**, an AI coach that proposes changes the user applies or undoes. **In development**, no release yet.

<table align="center">
  <tr>
    <td><img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/onboarding.gif" width="240" alt="Benchbite onboarding: a few questions, then a plan with daily targets and weekly workouts" /></td>
    <td><img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/workout-create.gif" width="240" alt="Creating a workout in Benchbite" /></td>
  </tr>
  <tr>
    <td align="center"><em>The onboarding</em></td>
    <td align="center"><em>Making a workout</em></td>
  </tr>
</table>

<p align="center">
  <img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/today.png" width="150" alt="Today screen" />
  <img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/nutrition.png" width="150" alt="Nutrition screen" />
  <img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/bite-proposal.png" width="150" alt="Bite proposing a change to a workout" />
  <img src="https://raw.githubusercontent.com/Kaandroids/benchbite/main/docs/media/workout-active.png" width="150" alt="A workout in progress" />
</p>

**How it is built**

- 🗄️ **No backend server.** The app talks to Supabase directly. Row level security on every table decides what each user may read and write; anything atomic or multi-table runs in Postgres functions, triggers and `pg_cron`.
- 📝 **Every decision written down.** 140+ Architecture Decision Records, from the stack to how chat photos are purged. Schema changes only through migrations, tested with pgTAP.
- 🤖 **AI that proposes, the user decides.** Bite runs in Deno Edge Functions behind an own model interface, with per-user and monthly spend limits enforced on the server. Changes to workouts, targets and the food log come as cards the user applies or undoes.
- ⌚ **Native where it matters.** A SwiftUI Apple Watch app follows the workout started on the phone; workouts, steps, weight and heart rate sync with Apple Health and Health Connect.
- ✅ **Checked on every pull request.** Types, lint, unit tests, database tests, Edge Function checks, Watch tests on a Mac and end-to-end journeys with Maestro.

<p>
  <img src="https://img.shields.io/badge/Expo-SDK_58-000020?logo=expo&logoColor=white" alt="Expo SDK 58" />
  <img src="https://img.shields.io/badge/React_Native-0.88-61DAFB?logo=react&logoColor=black" alt="React Native" />
  <img src="https://img.shields.io/badge/TypeScript-strict-3178C6?logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Supabase-Postgres-3ECF8E?logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/SwiftUI-watchOS-F05138?logo=swift&logoColor=white" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/Gemini-AI-4285F4?logo=google&logoColor=white" alt="Gemini" />
</p>

**[📂 Source &amp; Architecture Decision Records](https://github.com/Kaandroids/benchbite)**

---

## 🧾 Harper — invoice and bookkeeping automation for German accounting

> Turns a raw invoice PDF into a booking-ready accounting record: AI extraction, SKR account classification, tax code and statutory checks before anything reaches a human for review.

```
PDF / ZUGFeRD ─► AI extraction ─► HyDE ─► embeddings ─► pgvector top-10 ─► LLM picks the SKR account ─► §14 UStG + plausibility checks ─► review
```

- 🔍 **RAG for account classification.** Each line item is first expanded by HyDE into a hypothetical product description (asset, service, consumable…), embedded and matched against the SKR03/SKR04 chart of accounts with pgvector. The LLM then only chooses among the retrieved candidates instead of guessing an account number.
- ⚖️ **Rules where the law is exact.** 11 §14 UStG mandatory-field checks and 7 plausibility checks are plain Java, no AI. Depreciation (AfA), GWG and the VAT pre-registration follow German tax rules.
- 🏢 **Built for tax advisors.** Kanzlei ↔ Mandant tenancy with RBAC, bank-statement reconciliation, and a hash-chained, verifiable audit log.
- ✅ **Tested.** 90% line-coverage gate, integration tests against real PostgreSQL and Redis via Testcontainers, Playwright end-to-end tests.

<p>
  <img src="https://img.shields.io/badge/Java-21-ED8B00?logo=openjdk&logoColor=white" alt="Java 21" />
  <img src="https://img.shields.io/badge/Spring_Boot-3.5-6DB33F?logo=springboot&logoColor=white" alt="Spring Boot 3.5" />
  <img src="https://img.shields.io/badge/Angular-21-DD0031?logo=angular&logoColor=white" alt="Angular 21" />
  <img src="https://img.shields.io/badge/PostgreSQL-17_+_pgvector-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL 17 + pgvector" />
  <img src="https://img.shields.io/badge/Gemini-AI-4285F4?logo=google&logoColor=white" alt="Gemini" />
</p>

**[📂 Source &amp; Docs](https://github.com/Kaandroids/AutoFin)**

---

## ✉️ Postwerk — visual, AI-driven email automation

> Drag-and-drop workflows that classify, extract, reply to and forward emails, built with an AI assistant. **Live at [postwerk.io](https://postwerk.io)**, no longer in active development.

<p align="center">
  <a href="https://github.com/Kaandroids/Postwerk">
    <img src="https://raw.githubusercontent.com/Kaandroids/Postwerk/main/doc/screenshots/demo.gif" width="100%" alt="Postwerk: building an email automation with the AI assistant" />
  </a>
</p>

- ⚙️ **DAG automation engine.** Automations are graphs of 15 typed nodes run by a single executor, with dry-run tracing per node and reusable sub-flows.
- 🔍 **Hybrid search.** pgvector similarity fused with Postgres full-text search via reciprocal rank fusion.
- 🔐 **Multi-tenant SaaS on GCP.** Org-scoped queries, RBAC + JWT, Terraform, and keyless CI/CD with Workload Identity Federation and health-gated rollback.

<p>
  <img src="https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white" alt="Java 21" />
  <img src="https://img.shields.io/badge/Spring_Boot-3.4-6DB33F?logo=springboot&logoColor=white" alt="Spring Boot 3.4" />
  <img src="https://img.shields.io/badge/Angular-19-DD0031?logo=angular&logoColor=white" alt="Angular 19" />
  <img src="https://img.shields.io/badge/Terraform-IaC-7B42BC?logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/GCP-Cloud-4285F4?logo=googlecloud&logoColor=white" alt="GCP" />
</p>

**[🌐 Live](https://postwerk.io)** &nbsp;·&nbsp; **[📂 Source &amp; Docs](https://github.com/Kaandroids/Postwerk)**

---

## 🛠️ Other Projects

| Project | Description | Stack | Links |
| :--- | :--- | :--- | :--- |
| **Algoraph** | Interactive graph-algorithm learning platform with its own pseudocode language (lexer → parser → interpreter) and a step debugger on a live graph. | Angular · TypeScript | [Live](https://kaandroids.github.io/algoraph/) · [Code](https://github.com/Kaandroids/algoraph) |
| **Brief-Fix** | DIN 5008-compliant German letter generator with AI-assisted writing and PDF output for window envelopes. | Spring Boot · Angular · Gemini | [Frontend](https://github.com/Kaandroids/Brieffix-Frontend) · [Backend](https://github.com/Kaandroids/Brieffix-Backend) |
| **2Do** | Task management with JWT auth, Redis-backed token blacklisting and rate limiting. | Spring Boot · Angular · Redis | [Frontend](https://github.com/Kaandroids/2Do-frontend) · [Backend](https://github.com/Kaandroids/2Do-backend) |
| **Legacy MauMau** | My first app (2021): a card game, 100% human-made, from my second semester at Uni Hannover. | Java | [Code](https://github.com/Kaandroids/Legacy-MauMau-CardGame) |

---

## 🧰 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Backend** | Java 21 · Spring Boot 3 (Web, Data JPA, Security) · JWT · Flyway · MapStruct |
| **Frontend** | Angular 21 (standalone, signals) · TypeScript · RxJS · SCSS |
| **Mobile** | React Native · Expo · TanStack Query · SwiftUI (watchOS) |
| **Data** | PostgreSQL 17 · pgvector · Redis 7 · Supabase (RLS, Postgres functions, pg_cron) |
| **AI** | Gemini · RAG (HyDE, embeddings, vector search) · Claude Code |
| **Cloud &amp; DevOps** | GCP · Azure · Docker · Terraform · GitHub Actions · Supabase Edge Functions (Deno) |
| **Testing** | JUnit 5 · Testcontainers · pgTAP · Jest · Vitest · Playwright · Maestro |

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
  <a href="https://kaandroids.dev"><img src="https://img.shields.io/badge/Website-kaandroids.dev-1F2937?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/kaan-kara-0a720439b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:kaan403@icloud.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>
