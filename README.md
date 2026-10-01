### Federico Irarrázaval
**Senior Backend Engineer · Systems Integration & Data Reconciliation at Scale (Fintech & E-commerce) · Node.js · TypeScript · AWS · MCP & LLM Integrations**

Buenos Aires, Argentina · English C2 · [LinkedIn](https://linkedin.com/in/federico-irarrazaval) · [Portfolio](https://portfolio-fedeira.vercel.app) · fedeirar@gmail.com

---

I'm a backend engineer specialized in **integrating systems and reconciling data at scale** — sales, payments, inventory, orders — across e-commerce and fintech. Currently I co-led the build of the reconciliation platform at **nubceo** and now lead all new development on it, plus the promotions platform, a fintech processing **1M+ transactions/week**; before that, I integrated ERPs with e-commerce platforms at ITGlobers. The problems repeat across domains: idempotency, eventual consistency, conflicting sources of truth, volume.

Before code, I spent 7 years as a senior attorney at Baker McKenzie leading teams of lawyers and paralegals — which is why I end up owning specs, talking to stakeholders, and driving delivery even without a "lead" title.

Lately I've been building **production AI tooling**: an MCP server shipped to production and dual Claude/Gemini integrations solving the same problem two different ways.

---

#### Some of what I've worked on

- 🏦 **Payment reconciliation engine** — 97% automatic reconciliation rate, 95% reduction in manual resolution time, across a multi-tenant architecture with per-client rules (chart of accounts, tax treatment, payment providers).
- 🏷️ **End-to-end promotions platform** — full CRUD for promotion structures, PDF-to-JSON structuring via two different paradigms (direct Claude integration and MCP tool — see next bullet), and an **asynchronous matching engine** that tags every transaction ingested from clients' ERPs with the promotion that applied to it. That tagging is what powers the ROI and pricing-optimization dashboards downstream.
- 🤖 **MCP server in production** (TypeScript) — tools, prompts and resources exposing an internal API over stdio and streamable HTTP, running multi-tenant and authenticated on ECS. *(Co-built — I owned the server logic; auth and infra deploy were owned by others on the team.)*
- 🔀 **The same problem, two paradigms:** a promotion PDF → structured JSON, solved once as a direct Claude API integration (backend drives the Q&A) and once as an MCP tool (the user's own LLM drives it). Same outcome, opposite control model — happy to walk through the trade-offs.
- 🧠 **LLM-assisted reconciliation** — for the ~3% of transactions the deterministic engine can't close automatically, a Claude-powered endpoint suggests a reconciliation sequence for a human to review and approve. The model proposes, a person decides — no non-deterministic step touches the ledger directly.
- 🔌 4+ years integrating external systems and reconciling two sources of truth that never quite agree — ERPs ↔ VTEX (ITGlobers) and sales ↔ payment providers (nubceo). Same muscles, two domains.

#### Experience

**Senior Backend Engineer — nubceo** · Aug 2024 – Present · Remote
Fintech · payment & sales reconciliation (1M+ tx/week) · multi-tenant serverless on AWS · MCP server + Claude/Gemini integrations in production.

**Backend Engineer — ITGlobers** · Apr 2022 – Aug 2024 · Remote
E-commerce/marketplace integrations — VTEX IO, order status, inventory, payment platforms, bulk catalog loads.

**Senior Attorney — Baker McKenzie** · Aug 2015 – Feb 2022
Led teams of lawyers and paralegals in labor law. The reason "senior" with 4 years of code holds up: 11 years of professional seniority, not 4.

#### Stack

`Node.js` `TypeScript` `PostgreSQL` `AWS (Lambda, DynamoDB, SQS, ECS, API Gateway, RDS, X-Ray)` `Fastify` `Express` `Koa.js` `Serverless Framework` · `Model Context Protocol` `Claude API` `Gemini API` · `VTEX IO`

#### Selected certifications

Anthropic — MCP · MCP Advanced &nbsp;|&nbsp; DeepLearning.AI — MCP: Build Rich-Context AI Apps with Anthropic &nbsp;|&nbsp; Platzi — Claude AI · Claude Code

#### Pinned

- [`Project-Personal-Services`](https://github.com/FedeIra/Project-Personal-Services) — serverless microservices platform (8 Lambdas, DynamoDB w/ GSIs, SQS FIFO + DLQs, least-privilege IAM, X-Ray)
- [`MCP-Server-Client-Learning`](https://github.com/FedeIra/MCP-Server-Client-Learning) — MCP server & client: tools, prompts, resources over stdio + streamable HTTP
- [`Project-Backend-Movie`](https://github.com/FedeIra/Project-Backend-Movie) — Fastify + TypeScript + Zod REST API
- [`Project-Portfolio`](https://github.com/FedeIra/Project-Portfolio) — personal portfolio site, source available

---

📫 Open to Senior Backend / Product Engineer / Tech Lead roles — reach out at fedeirar@gmail.com

---
