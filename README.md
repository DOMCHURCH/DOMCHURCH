<div align="center">

<img src="assets/header.svg" width="880" alt="Dominique Church — public-data finance systems">

<!-- Pixel art agent: commit the image to this repo as assets/agent-pixel.png (or push it to
     DOMCHURCH/Gnosis under docs/ and swap in the raw.githubusercontent URL), then uncomment: -->
<!-- <img src="assets/agent-pixel.png" width="420" alt="Gnosis pixel art agent"> -->

[![Typing](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3200&pause=800&color=58A6FF&center=true&width=620&lines=Geopolitical+risk+%C2%B7+equity+research+%C2%B7+SEC+data;FastAPI+%C2%B7+React+%C2%B7+DuckDB+%C2%B7+Postgres+%C2%B7+real+public+data;Eight+web+properties+live+in+production)](https://git.io/typing-svg)

</div>

---

### Live in production

I build self-contained data systems: scheduled ingestion from free public sources (SEC EDGAR, GDELT, World Bank, FRED, OFAC), typed storage, a scoring or valuation model on top, and a UI that shows the result at full resolution. Everything below is deployed and running on real data — no mocks, no paywalled feeds.

Current flagship: BalanceProof — reconciled SEC balance sheet data, live at [balanceproof.dev](https://balanceproof.dev).

#### 🤖 [Gnosis](https://github.com/DOMCHURCH/Gnosis) — terminal coding agent
Open-source terminal coding agent (TypeScript + Ink) with a browser UI (`dom serve`) and a live Three.js 3D office floor where sub-agents animate between zones as they work. Provider-agnostic via OpenRouter — switch models mid-session with the conversation intact, automatic fallback to the cheapest paid model on upstream errors. MCP client, Obsidian-backed long-term memory, local Kokoro TTS voice overlay, Electron desktop build with notify-only auto-updater, token-bucket rate limiting and host-allowlisted server with timing-safe auth. **150+ verify suites** run on every CI push (Windows + Playwright). MIT.

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2?style=flat-square)

#### 🌍 [Sovereign](https://sovereign-production-0351.up.railway.app) — geopolitical risk intelligence
Continuously ingests public data across ~75 countries, fuses it into a typed `Country` ontology in DuckDB, and runs a NetworkX contagion model over the resulting graph. Outputs a composite **0–100 risk score** per country, a history/delta series, and cross-border spillover alerts weighted by financial correlation, trade openness and regional adjacency. A **GDELT bulk-event ingestor** parses the 15-minute export files, filters to violent CAMEO codes, deduplicates and cross-corroborates sources, and renders ~700 geolocated incidents/day onto a WebGL globe (NASA Blue Marble textures, real sun position) with click-through to the source article. Connectors are free and keyless: World Bank WDI/WGI, FRED, OFAC SDN, country-proxy ETFs, VADER-scored news from 11 outlets, GDELT, Open-Meteo. APScheduler drives a 15-minute fast cycle and a 6-hour full cycle on a Railway persistent volume; an LLM analyst chat sits over the same store.

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![NetworkX](https://img.shields.io/badge/networkx-2C5364?style=flat-square)

#### 📈 [Axiom](https://axiom-mu-ten.vercel.app) — institutional-style equity research
Ticker in, fully priced research note out. Resolves the ticker to a CIK against SEC's company_tickers file, pulls five years of XBRL company facts from `data.sec.gov`, derives margins and Piotroski F-score inputs, runs an LLM analysis pass, and renders a complete note — **DCF, comparables, bull/bear thesis, risk score, recommendation** — exportable to PDF. Handles the 60s/30s function caps with retry and backoff.

![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Neon Postgres](https://img.shields.io/badge/Neon%20Postgres-336791?style=flat-square&logo=postgresql&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=flat-square)
![Groq](https://img.shields.io/badge/Groq%20llama--3.3--70b-F55036?style=flat-square)

#### ⚖️ [BalanceProof](https://balanceproof.dev) — reconciled balance sheets at true proportion
Every US public company's balance sheet, drawn at real scale from SEC filings. A bank, a retailer and a software company produce visibly different shapes. Three views per company: what it owns and who has a claim on it, where each dollar of revenue goes, and how its annual sales compare to national GDP.

The hard part was selection: SEC reports the same figure many times per filing, split by segment, geography and legal entity. JPMorgan files "total assets" 23 separate times, and exactly one row is the consolidated company. Every filing is reconciled against the accounting identity (Assets = Liabilities + Equity) before it is stored. 6,224 companies covered. 4,912 reconcile directly. 215 flagged with a specific reason. 0 hidden.

Live: https://balanceproof.dev

API: https://balanceproof.dev/api

Repo: https://github.com/DOMCHURCH/AlphaCode

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)

---

### Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)

---

<div align="center">
<table>
<tr>
<td align="center" valign="middle">
<a href="https://domchurch.github.io/DOMCHURCH/" title="Open the interactive version — the hole follows your cursor"><img src="assets/portrait.png" width="380" alt="ASCII portrait"></a>
</td>
<td align="center" valign="middle">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake.svg" />
  <img alt="contribution snake" width="520" src="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake.svg" />
</picture>
</td>
</tr>
</table>

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=DOMCHURCH&show_icons=true&theme=dark&hide_border=true)](https://github.com/DOMCHURCH)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=DOMCHURCH&layout=compact&theme=dark&hide_border=true)](https://github.com/DOMCHURCH)

</div>

---

<div align="center">
Ottawa · Public data, real systems · 2026 · balanceproof.dev
</div>