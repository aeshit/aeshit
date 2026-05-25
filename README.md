## Laboratory

---

### Live

#### [dpdpscore.in](https://dpdpscore.in) — DPDP Score

India's first public compliance rating platform for the Digital Personal Data Protection Act. Proactively scans company websites and publishes grades from A+ to F — not a GRC tool, not a cookie banner. Companies discover their public grade, then buy the audit.

- 270+ Indian companies scored and indexed.
- 3-phase consent crawl via headless Playwright — captures pre-consent, post-consent, and post-withdrawal state for every domain.
- LLM-assisted policy analysis grades required disclosure fields against the actual privacy policy text.
- GeoIP lookup on every third-party destination flags unannounced cross-border transfers.
- 4-category weighted scoring engine across 220+ DPDP-specific rules.
- HITL-gated scan pipeline: BullMQ job queue on a self-hosted runner, bi-weekly automated rescans via GitHub Actions, delta hold and policy hold gates before publish.

`Next.js 15 · Fastify · tRPC · Drizzle ORM · PostgreSQL · TimescaleDB · Redis · BullMQ · Playwright · Razorpay · Supabase Auth · Turborepo · Vercel`

#### [builtlike.app](https://builtlike.app) — BuiltLike

Calendar-first fitness app built around multi-personality sport benchmarks. Pick a sport profile, schedule workouts on a calendar, and every saved set auto-derives PRs into an immutable benchmark history.

- 19 sport profiles across 5 sports — football, combat, cricket, track, strength — with 5 generalists and 14 role specializations, each defining metrics with concrete targets in real units sourced from sport-science benchmarks.
- Rule-based smart-fill scheduler that populates the calendar from goals, equipment, and experience level.
- 200+ exercises with auto-looping video demos, plate math for barbell work, recency-weighted body map, and a contribution grid for streaks.
- Tier progression system (Rookie → Athlete → Pro → Elite) derived from gap-to-target across benchmarks.

`React Native · Expo SDK 55 · TypeScript · NativeWind · Supabase · PostgreSQL · Edge Functions · Razorpay · Zustand · TanStack Query · Reanimated`

---

### The Trading Desk

Three tools built on a shared SQLite market data layer — daily OHLCV candles for Nifty 200 back to 2006, NSE bhavcopy with delivery data, quarterly SEBI shareholding patterns, fundamentals, and a tagged news archive.

**PortfolioBot** — Telegram bot for Indian equities. Morning briefings at market open with portfolio health, sector rotation, and actionable picks. Intraday scans every 30 minutes — only surfaces signals on technical confluence across RSI, MACD, VWAP, and EMA crossovers. FIFO lot tracking with full STCG/LTCG/STT/GST tax computation. 7 RSS news feeds with urgency classification and 4-hour fingerprint dedup. Vercel-hosted dashboard for historical scan and briefing data. Built on FastAPI with APScheduler driving the scan loop.

**AlphaEngine** — Strategy backtesting lab for NSE/BSE. 8 strategies with walk-forward calibration windows, DuckDB-accelerated parallel execution across the full universe, multi-strategy portfolio composition, and a web dashboard for browsing results. Reads candles and delivery data from the shared market data layer.

**EquityResearcher** — Multi-agent equity research pipeline. One ticker in, structured investment report out. 8-phase pipeline: data collection, thesis formation, adversarial challenger, gap-filling research, parallel specialist analysis (technicals, valuation, catalysts), synthesis with entry/exit zones and scenario modelling, section writing, and final assembly with a quality gate.

---

### Completed Quests

- **[Forgekit](https://github.com/aeshit/ai-software-house)** — Three-agent dev orchestrator. Architect, implementer, and reviewer coordinate through Slack to ship apps from a text prompt. Parallel execution via git worktrees, code review before merge, multi-round discovery. Built on asyncio with SQLAlchemy. Predates the Claude Agent SDK.
- **theConclave** — AI-powered competitive intelligence engine. Runs web-grounded deep research across 14 verticals, evaluates market gaps through a 7-phase analytical pipeline, and produces scored dossiers with a 5-axis composite rating covering market size, competition density, technical feasibility, defensibility, and monetisation potential.
- **Editr** — Resume tailoring tool. Paste a job description, get back a single-page PDF restructured and rewritten for the role. Typst handles typesetting, Supabase handles state.
- **[Reels](https://github.com/aeshit/reels)** — Real-time 3D companion for Claude Code. File operations rendered as glowing nodes in a Three.js force graph via SSE. Predates Claude's own companion view.
- **[ap-excise-anomaly](https://github.com/aeshit/ap-excise-anomaly)** — Anomaly detection on Andhra Pradesh excise department data.
- **[MeetingScheduler](https://github.com/aeshit/MeetingScheduler)** — Python meeting scheduler implementation.
