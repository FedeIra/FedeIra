# Propuesta de README para `FedeIra/My-Profile`

> Versión ajustada tras feedback: especialización más amplia ("integración y conciliación de datos a escala")
> en vez de "especialista en conciliación de pagos", para no leer como cerrado solo a fintech.
> Pendientes marcados abajo — copiar todo lo que sigue a la línea de guiones en el `README.md` del repo.

---

### Federico Irarrázaval
**Senior Backend Engineer · Systems Integration & Data Reconciliation at Scale · Node.js · TypeScript · AWS · MCP & LLM Integrations**

Buenos Aires, Argentina · English C2 · [LinkedIn](https://linkedin.com/in/federico-irarrazaval) · [Portfolio](https://portfolio-fedeira.vercel.app) · fedeirar@gmail.com

---

I'm a backend engineer specialized in **integrating systems and reconciling data at scale** — sales, payments, inventory, orders — across e-commerce and fintech. Currently I design and maintain the reconciliation & promotions platform at **nubceo**, a fintech processing **1M+ transactions/week**; before that, I integrated ERPs with e-commerce platforms at ITGlobers. The problems repeat across domains: idempotency, eventual consistency, conflicting sources of truth, volume.

Before code, I spent 7 years as a senior attorney at Baker McKenzie leading teams of lawyers and paralegals — which is why I end up owning specs, talking to stakeholders, and driving delivery even without a "lead" title.

Lately I've been building **production AI tooling**: an MCP server shipped to production and dual Claude/Gemini integrations solving the same problem two different ways.

---

#### What I've built

- 🏦 **Payment reconciliation engine** — 97% automatic reconciliation rate, 95% reduction in manual resolution time, across a multi-tenant architecture with per-client rules (chart of accounts, tax treatment, payment providers).
- 🤖 **MCP server in production** (TypeScript, official SDK) — tools, prompts and resources exposing an internal API over stdio and streamable HTTP, running multi-tenant and authenticated on ECS. *(I built the server logic — auth and infra deploy were owned by others on the team.)*
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

`Node.js` `TypeScript` `PostgreSQL` `AWS (Lambda, DynamoDB, SQS, ECS, API Gateway, RDS, X-Ray)` `Fastify` `Express` `Serverless Framework` · `Model Context Protocol` `Claude API` `Gemini API`

#### Certifications

Anthropic — MCP · MCP Advanced &nbsp;|&nbsp; Platzi — Claude AI (×2)

#### Pinned

- [`Project-Personal-Services`](https://github.com/FedeIra/Project-Personal-Services) — serverless microservices platform (8 Lambdas, DynamoDB w/ GSIs, SQS FIFO + DLQs, least-privilege IAM, X-Ray)
- `Project-MCP-...` *(pending rename, task 3.2.2)* — production-style MCP server: tools, prompts, resources
- [`Project-Backend-Movie`](https://github.com/FedeIra/Project-Backend-Movie) — Fastify + TypeScript + Zod REST API

---

📫 Open to Senior Backend / Tech Lead roles — reach out at fedeirar@gmail.com

---

## Notas para vos (no van en el README)

1. **`[DECIDIR]` grafía del apellido** — usé "Irarrázaval" con tilde. Si en el resto de las superficies eligen sin tilde, es find-replace acá también (decisión 8 del plan).
2. **Fecha de inicio en ITGlobers** — usé Abr 2022 (mayoría: LinkedIn + portfolio). Sigue pendiente contra Jun 2022 (decisión 7).
3. **Límite de atribución del MCP respetado** — el paréntesis "auth e infra las hicieron otros" es intencional, no lo borres.
4. **El repo de MCP sigue sin link real** porque hoy es `MCP-Server-Client-Learning` con TODOs sin implementar (tarea 3.2.1). Cuando esté renombrado y terminado, cambiá la línea de "Pinned" por el link real.
5. **`fedeira.xyz` no está** — sigue marcado para deprecar (tarea U.3 / 1.9), no lo agregues.
