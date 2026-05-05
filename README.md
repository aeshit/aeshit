## Shipping.

Building AI-native SaaS products, solo.

---

### Live

#### [dpdpscore.in](https://dpdpscore.in) — DPDP Score

India's first public compliance rating platform for the Digital Personal Data Protection Act. The CRISIL of privacy.

- Proactively scans Indian company websites and publishes public grades (A+ to F) — not a GRC tool, not a cookie banner. Companies discover their public grade, then buy the audit.
- **270+ Indian companies scored and indexed.**
- 3-phase consent crawl via Playwright — captures pre-consent, post-consent, and post-withdrawal state for every domain.
- LLM-assisted policy analysis (Gemini 2.5 Flash) grades 5 required disclosure fields against the privacy policy.
- GeoIP lookup on every third-party destination flags unannounced cross-border transfers.
- 4-category weighted score: Consent 30% · Notice 25% · Security 20% · Data Handling 25%. 220+ rules across DPDP, CERT-In, SOC 2, ISO 27001.
- HITL-gated scan pipeline: BullMQ + Redis on a self-hosted Mac, bi-weekly automated rescans via GitHub Actions, delta hold + policy hold gates before publish.

`TypeScript` · `Next.js 15` · `Fastify` · `tRPC` · `PostgreSQL` · `TimescaleDB` · `Redis` · `BullMQ` · `Playwright` · `Gemini` · `Razorpay` · `Supabase Auth` · `Turborepo` · `Vercel`

#### [builtlike.app](https://builtlike.app) — BuiltLike

Calendar-first fitness app built around multi-personality sport benchmarks.

- Pick one or two sport profiles, schedule workouts on a calendar, every saved set derives PRs into an immutable benchmark history.
- **19 sport profiles across 5 sports** — football, combat, cricket, track, strength — with 5 generalists and 14 role specializations.
- Each profile defines 5–10 metrics with concrete targets in real units (kg, reps, seconds, cm) — sourced from public sport-science benchmarks, not celebrity programs.
- Tier system: Rookie / Athlete / Pro / Elite based on gap-to-target.
- **Smart-fill** rule-based scheduler populates the calendar from goals + equipment + experience level.
- 200+ exercises with auto-looping video demos, plate math for barbell work, recency-weighted body map, GitHub-style contribution grid for streaks.
- 14-day reverse trial — full premium, **no card required**.
- BOGO referral: every first-time payer gets a single-use code that grants matching premium tier to one friend.
- Web live, Android awaiting Play Store approval. Razorpay-only checkout — no IAP cut.

`React Native` · `Expo SDK 55` · `TypeScript` · `NativeWind` · `Supabase` · `PostgreSQL` · `Edge Functions` · `Razorpay` · `Zustand` · `TanStack Query`

---

### Building

#### Finance — three tools, one shared market data layer

- **PortfolioBot** — Telegram bot for Indian equities. 9:05 AM morning briefings (portfolio health, macro, picks). Intraday scans every 30 min, only pings on confluence (RSI + MACD + VWAP + EMA, ≥2 breaches simultaneous). FIFO lot tracking with full STCG/LTCG/STT/GST tax math. 7 RSS news feeds with urgency classification + 4-hour fingerprint dedup. Dashboard on Vercel. Costs ₹7/month to run. `Python · Gemini · FastAPI · SQLite · APScheduler · Next.js`
- **EquityResearcher** — multi-agent equity research pipeline. One ticker in, structured research report out. `Python · Claude · Gemini · SQLite`
- **AlphaEngine** — strategy backtesting lab. 8 strategies, walk-forward validation, multi-strategy composition, execution runtime that can talk to a live order book. `Python · FastAPI · NumPy · pandas`

#### subBuddy

Embedded Shopify app for Indian D2C subscription commerce. Built around Razorpay UPI Autopay and RBI e-mandate — undercutting the USD pricing of Recharge and Skio for stores that can't justify it. Plan builder, subscription lifecycle, customer portal, smart dunning for failed recurring payments.

`Node.js` · `Razorpay` · `Shopify App Bridge` · `PostgreSQL` · `BullMQ`

#### OutreachPro

Autonomous AI sales agent. 10-step pipeline: discovers companies, finds decision-makers, scores leads 0–100, writes personalized cold emails across 12 templates × 8 verticals, verifies deliverability via SMTP handshake, validates SPF/DKIM/DMARC. Pluggable research nodes for domain-specific qualification. Nothing sends without inbox review.

`Next.js` · `FastAPI` · `Claude` · `Gemini` · `Celery` · `Redis` · `PostgreSQL` · `Hunter.io`

---

### Slop

- **Editr** — AI resume tailor. Paste a JD, get a tailored single-page PDF out via Typst. `Next.js · Gemini · Typst · Supabase`
- **theConclave** — SaaS idea discovery engine. Gemini researches (web-grounded), Claude evaluates. 7-phase scan across 14 verticals, 5-axis composite scoring, deep-research dossiers. `TypeScript · Gemini · Claude · SQLite`
- **Forgekit** — multi-agent dev orchestrator. Atlas (architect) + Dev (implementer) + Charon (reviewer) coordinate via Slack to ship production apps from a text prompt. Parallel execution via git worktrees, code review before merge, multi-round discovery. Predates the Claude Agent SDK. `Python · asyncio · Claude SDK · Slack · SQLAlchemy`
- **Reels** — real-time 3D companion for Claude Code. File operations rendered as glowing nodes in a Three.js scene, hooked into Claude Code transcripts via SSE. Predates Claude's own companion view. `TypeScript · Three.js · SSE · Express`
