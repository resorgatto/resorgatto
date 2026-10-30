<div align="center">

# Renato Sorgatto

**Backend Engineer**

Backends built to hold up in production. Multi-tenant SaaS, auth, async pipelines. Security enthusiast.

<a href="https://www.sorgatto.dev"><img src="https://img.shields.io/badge/sorgatto.dev-111111?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/renato-sorgatto/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:renatosorgatto@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

---

## About

Backend engineer at Carvion, building Orquestra360 and the products that run on it. Orquestra360 is a multi-tenant platform: one auth, billing and tenancy core shared by every product under the Bravend brand. My work is the server side of it: schema-per-tenant isolation on PostgreSQL, SSO with RS256 JWTs, Celery pipelines and LLM features that run for real users. I build the Next.js frontend too.

I am a security enthusiast, and it shows in how I design an API. What I study and practice most now is system design: capacity, failure modes, idempotency, backpressure. The things that decide whether a system survives growth.

## How I work

- **Design for the failure first.** Before the happy path, I write down what happens when the queue backs up, the pool runs dry or a webhook arrives twice. Idempotency keys, timeouts and retries with backoff go into the design, not into a hotfix.
- **Isolation by construction.** Schema per tenant on PostgreSQL. A cross-tenant leak is impossible by construction, not by code review.
- **Security as the default.** RS256 tokens, secrets encrypted at rest, least privilege on every integration, secret scanning in CI. I read my own APIs the way an attacker would.
- **Async by default.** Heavy work goes to Celery and queues. The request stays fast, and a slow third party cannot take the API down with it.

## Stack

| Layer | Tools |
| :--- | :--- |
| Backend | Python, Django, DRF, Django Ninja, FastAPI, Celery, Node.js |
| Data | PostgreSQL, Redis, Prisma, SQLAlchemy, MinIO / S3 |
| AI | OpenAI, Anthropic, Whisper, with a cost and latency budget |
| DevOps | Linux, Docker, GitHub Actions, Vultr, Vercel, Sentry |
| Frontend | TypeScript, React, Next.js |

## Work

Day job: the Orquestra360 ecosystem at Carvion. Beyond it: products of my own and open source. Case studies for all of them at [sorgatto.dev](https://www.sorgatto.dev).

**Orquestra360 ecosystem (Carvion)**

| Project | What it is | Stack |
| :--- | :--- | :--- |
| [Orquestra360](https://orquestra360.com.br) | The hub: SSO (JWT RS256), schema-per-tenant multi-tenancy, white-label branding and a central credit wallet shared by every product | Django, DRF, Next.js, PostgreSQL, Redis |
| Siv360 | AI sales simulator: hybrid AI plus human scoring, spoken answers transcribed live with Whisper | Django, OpenAI, Whisper, Celery |
| Assessments360 | 360 assessments, DISC, PDI and competency management, with reports per person and per team | Django, Next.js, Recharts |
| Learning360 | Gamified LMS: learning paths, courses, certificates and forums | Django, Next.js |
| [Fala T&D](https://falatd.bravend.com.br) | Offline-first PWA for live events: QR check-in without signal, ICP scoring, CRM webhooks with retry | FastAPI, Next.js, IndexedDB |
| LAB.AIx | Touchscreen kiosk that turns a recorded voice diagnosis into an ADDIE learning blueprint | Next.js, Prisma, Claude, Whisper |
| Vinvolve | Standalone course and membership hub with auth and transactional email | React, Vite, Express, Drizzle |

**Own products and open source**

| Project | What it is | Stack |
| :--- | :--- | :--- |
| SEAM | Webhook integration hub: per-workflow ingest URLs that answer 202 at once, Celery delivery with exponential backoff and a dead-letter queue, tenant-isolated workspaces, credentials encrypted with Fernet. First module of SGT Systems | Django, Django Ninja, Celery, PostgreSQL, Redis |
| Hub4Makers | Real margin per piece for people who sell 3D prints on marketplaces: filament, energy by state tariff, packaging, failed prints and fees in one place | Django, Next.js, PostgreSQL, Redis |
| [Chariot](https://github.com/resorgatto/Chariot) | Open-source fleet and delivery management: coverage areas validated on PostGIS, Celery notifications, React PWA with Leaflet maps and push. MIT | Django, DRF, PostGIS, Celery, React |
| [SmartPortfolio](https://github.com/resorgatto/SmartPortfolio) | Scheduled stock purchases: consolidates monthly orders, splits standard and fractional lots, keeps average price and withholding tax per client. Clean Architecture, Kafka events, B3 COTAHIST parser | C#, .NET 8, MySQL, Kafka |

---

<details>
<summary>Versão em português</summary>

<br/>

**Engenheiro Backend.** Backends feitos para aguentar a produção. SaaS multi-tenant, autenticação, pipelines assíncronos. Entusiasta de segurança.

Engenheiro backend na Carvion, onde construo o Orquestra360 e os produtos que rodam sobre ele. O Orquestra360 é uma plataforma multi-tenant: um núcleo único de autenticação, cobrança e tenancy compartilhado por todos os produtos da marca Bravend. Meu trabalho é o lado do servidor: isolamento schema-per-tenant no PostgreSQL, SSO com JWT RS256, pipelines em Celery e funcionalidades com LLM rodando para usuários reais. Também faço o frontend em Next.js.

Sou entusiasta de segurança, e isso aparece na forma como desenho uma API. O que mais estudo e pratico hoje é system design: capacidade, modos de falha, idempotência, backpressure. As coisas que decidem se um sistema sobrevive ao crescimento.

**Como eu trabalho**

- **Projetar a falha primeiro.** Antes do caminho feliz, escrevo o que acontece quando a fila enche, o pool esgota ou um webhook chega duas vezes. Chaves de idempotência, timeouts e retry com backoff entram no desenho, não no hotfix.
- **Isolamento por construção.** Schema por tenant no PostgreSQL. Um vazamento entre tenants é impossível por construção, não por code review.
- **Segurança como padrão.** Tokens RS256, segredos criptografados em repouso, privilégio mínimo em cada integração, secret scanning no CI. Leio minhas próprias APIs como um atacante leria.
- **Assíncrono por padrão.** Trabalho pesado vai para Celery e filas. A requisição continua rápida, e um terceiro lento não derruba a API junto.

Os cases de todos os projetos estão em [sorgatto.dev](https://www.sorgatto.dev/pt).

</details>
