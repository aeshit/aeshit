<h2>Shipping.</h2>

<h3>Building AI-native SaaS products, solo.</h3>

<p>
  <a href="https://github.com/aeshit">GitHub</a> ·
  <a href="#live">Live</a> ·
  <a href="#building">Building Now</a> ·
  <a href="#markets">Markets</a> ·
  <a href="#utilities">Utilities</a> ·
  <a href="#scooped">Scooped</a>
</p>

---

<h3 id="live">Live</h3>

### [builtlike.app](https://builtlike.app) &nbsp;·&nbsp; **BuiltLike**

Train like your heroes. Gamified fitness app — nine celebrity programs and a library of 200+ exercises with video demos. Web is live; Android awaiting Play Store approval; iOS next.

`React Native` · `Expo` · `TypeScript` · `Supabase` · `NativeWind` · `Razorpay`

### [dpdpscore.in](https://dpdpscore.in) &nbsp;·&nbsp; **DPDP Score**

India's public DPDP compliance index. An external crawl engine audits websites against the DPDP Act, captures consent states across the full user lifecycle (pre-consent, post-consent, withdrawal), and publishes a comparable score. **270+ Indian companies already scored and indexed.**

`TypeScript` · `Next.js` · `Fastify` · `tRPC` · `PostgreSQL` · `TimescaleDB` · `Redis` · `BullMQ` · `Playwright` · `mitmproxy` · `Razorpay`

---

<h3 id="building">Building Now</h3>

In flight.

### **subBuddy** — *Subscription commerce for Indian Shopify stores.*

Embedded Shopify app built around Razorpay UPI Autopay and RBI e-mandate. Plan builder, subscription lifecycle, customer portal, and smart dunning for failed recurring payments — without the USD pricing of foreign alternatives.

`Remix` · `TypeScript` · `Prisma` · `PostgreSQL` · `BullMQ` · `Razorpay` · `Shopify App Bridge`

### **OutreachPro**

Autonomous AI sales agent. Finds its own leads, researches decision-makers, writes personalized cold emails across 12 templates × 8 verticals, and tracks ROI attribution back to USD. Nothing sends without inbox review.

`Next.js` · `TypeScript` · `FastAPI` · `Python` · `PostgreSQL` · `Redis` · `Celery` · `Claude` · `Gemini`

---

<h3 id="markets">Markets</h3>

From a morning Telegram ping to a backtesting lab. Listed newest first.

### **AlphaEngine**

Standalone strategy lab and backtester. Walk-forward validation against historical tape, multi-strategy composition, and an execution runtime that can talk to a live order book.

`Python` · `FastAPI` · `NumPy` · `pandas` · `Jupyter`

### **AlphaFlow**

A normalized financial data engine. Aggregates regulatory filings (SEC EDGAR, SEBI, NSE) and market data across US and Indian markets — normalizes tape, fundamentals, filings, and sentiment into a strict `ContextPacket` schema. Ships with a 4-factor alpha scoring engine that produces a composite score with an AI-generated narrative.

`Python` · `FastAPI` · `Pydantic` · `Gemini` · `Firecrawl` · `sec-parser`

### **PortfolioBot** — *Wakes me up at 9:05 every morning.*

Telegram bot for Indian equities. Pre-market briefing covers portfolio health, macro context, and picks. Scans NSE tape every 30 minutes during market hours but only pings when two or more technicals breach simultaneously. FIFO lot tracking with full STCG/LTCG/STT tax math.

`Python` · `FastAPI` · `Gemini` · `Next.js` · `SQLAlchemy` · `Vercel`

---

<h3 id="utilities">Utilities</h3>

### **[Editr](https://github.com/aeshit/editr)** — *Got tired of tailoring resumes by hand.*

Parses a JD, researches the company, suggests card-based edits I refine in plain English. Outputs a single-page PDF via Typst.

`Python` · `Flask` · `Gemini` · `Typst`

### **[theConclave](https://github.com/aeshit/theConclave)** — *Two AIs walk into a room and argue about SaaS ideas.*

Gemini researches, Claude judges. 7-phase scan across 14 verticals with deep-research dossiers and cross-run learning.

`TypeScript` · `Gemini` · `Claude` · `React`

---

<h3 id="scooped">Scooped</h3>

Built these to solve my own problems. Watched the big labs build theirs around the same time. Moved on.

### **AI Software House** — *Multi-agent dev orchestrator.*

Three agents — Atlas (architect), Dev (implementer), Charon (reviewer) — coordinate through Slack to build production apps from a text prompt. Parallel execution via git worktrees, code review before merge, multi-round discovery. Predates Claude Agent SDK and ChatGPT Agents.

`Python` · `asyncio` · `Claude SDK` · `Slack` · `SQLAlchemy`

### **Reels** — *A live 3D companion for Claude Code.*

File operations rendered as glowing nodes in a Three.js scene with HUD overlay and bloom post-processing — hooked directly into Claude Code transcripts. Predates Claude's own companion view.

`TypeScript` · `Three.js` · `SSE`
