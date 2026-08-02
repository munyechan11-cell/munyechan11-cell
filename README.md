## Yechan Mun — Product Manager & Forward Deployed Engineer

I go to the site, measure what is actually broken, and build the smallest thing that survives there.

**The rule that repeats across everything below: AI drafts. Humans and servers confirm.**
Every AI feature I ship has a fallback, and every irreversible action is decided by a server or a person — never by a model.

---

### Why most repositories here are private

Four of these products are running with real users — a client's factory safety team, a local children's welfare center, two pilot stores. Their repositories hold client data models, partner terms and credentials, so they stay private until each owner agrees otherwise.

**Everything below is live and clickable instead.** If you need to read code for an evaluation, ask me and I will arrange access to a specific repository.

---

### What I have shipped

**Multilingual Frontline Safety Platform** — Product Manager & sole developer
*Live: [aimake-tbm.onrender.com](https://aimake-tbm.onrender.com) · Android/iOS app in pilot since 27 Jul 2026*

On-site I counted 103 of 104 registered workers as untrained — a 1% completion rate. Competing tools stopped at "translate and deliver", so I reframed the product to *verify comprehension*: you pass a quiz in your own language or you are not marked as trained.

* 3-layer localization for 11 languages — base dictionary → 98 pre-translated domain terms → runtime AI translation
* Offline-first. A cache miss returns a network error, never "no training today" — that single false display is what turns into an incident
* Fallbacks on all 12 AI-backed features, so the product works with no API key at all
* Deploy aborts and keeps the previous version on any destructive schema change

`NestJS` `Prisma` `PostgreSQL` `Capacitor` `PWA` — 143 API routes · 29 data models · 72 tests · 254 commits, all single-author

---

**Evidence-Based Credentialing System** — Product Owner & lead developer
*Live: [skillprint-student.vercel.app](https://skillprint-student.vercel.app)*

Turning a research finding — that employers want narrative context, not digital badges — into a working system.

* Deliberately **no LLM**. This document is used in hiring, so it runs on a rule-based narrative engine with a source field on every sentence, traceable back to the exact input
* Found a forgery vector in my own build (approval badges could be faked through an unsigned link) and added Web Crypto ECDSA P-256 signatures — while stating in the UI that a signature proves integrity, not identity
* A permanent 5-axis self-verification tab, so anyone can check the output

937 tests passing · rubric of 6 competencies × 4 levels

---

**Care-Service Operations + Assistant Chatbot** — sole developer
*Live: [dolbom-sangdam.vercel.app](https://dolbom-sangdam.vercel.app)*

* Scored 3 architectures (54/55/41) before committing, and chose the one that survives network and API outages
* Built risk detection as a 33-term rule lexicon rather than an LLM, and wrote *the judgment is human* into the code. I claim high sensitivity and low precision, not accuracy
* Anonymized by default — records stored under codes only, raw utterances excluded from the UI and from backups

---

**Retail Operations Cloud (POS · CRM · ERP · AI)** — founder, sole developer
*Live: [theta-sepia.vercel.app](https://theta-sepia.vercel.app) · [source](https://github.com/munyechan11-cell/gyeol)*

* Re-defined the anonymous QR visitor as a customer identifier, so returning customers are recognized with zero signup drop-off
* Automatic RFM classification into 6 grades, driving tiered messaging
* An approval gate with an audit log: AI writes the draft, the server confirms the booking
* HMAC-SHA256 verification on payment webhooks; a 4-stage route guard (login → role → attendance → grade)

Validated in 2 pilot stores on a pay-after-results model I negotiated with the owner directly.

---

**Local ESG Gamification Platform** — sole developer
*Live: [esg-sul.vercel.app](https://esg-sul.vercel.app)*

A 5-step mission (intro → quiz → GPS geofence → AI receipt verification → limited reward) that completes with **zero operator intervention**. 50+ active users; 3 partner cafés signed in person.

---

**Restaurant Operations ERP — AI/OCR domain** *(team project; my scope is the AI/OCR domain)*
Released on Google Play. I designed 3 pipelines that pull daily and hourly revenue out of receipt and POS screenshots, so an owner records sales from one photo. I treated the output schema and the verification layer as the real problem, not the prompt — health-check endpoint, a 422 reproduction test that isolated a UOM field type mismatch, and a verify script.

---

**Short-Term Investing Assistant** — sole developer
*[github.com/munyechan11-cell/invest](https://github.com/munyechan11-cell/invest)*

One poll per symbol broadcast to all clients, removing duplicate external API calls, plus a 6-source fallback chain for quotes so a single provider outage never stops a lookup.

---

### How I work

* The workaround people already use — the spreadsheet, the group chat, the paper log — is the real spec
* I name what a product cannot do before I demo what it can
* I do not report a pilot as a success until the adoption number comes back

---

### Stack

`TypeScript` `Python` `NestJS` `FastAPI` `React` `Prisma` `PostgreSQL` `Firebase` `Capacitor` `PWA` · LLM applications, schema-forced outputs, fallback design

Handong Global University, 2026– · Vice President, IMC Technology Management Society

**[LinkedIn](https://www.linkedin.com/in/munyechan11/)**

**[LinkedIn](https://www.linkedin.com/in/munyechan11/)**
## Hi there 👋
