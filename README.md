<div align="center">

<img src="assets/ascii-burn.svg" width="880" alt="ASCII portrait with a hole burning through it">

![header](https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Dominique%20Church&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Solo%20founder%20%C2%B7%20shipping%20live%20products&descSize=18&descAlignY=60)

[![Typing](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3200&pause=800&color=58A6FF&center=true&width=620&lines=Geopolitical+risk+%C2%B7+equity+research+%C2%B7+SEC+data;FastAPI+%C2%B7+React+%C2%B7+real+public+data%2C+no+paywalls;Eight+web+properties+live+in+production)](https://git.io/typing-svg)

</div>

---

### Live in production

I build self-contained systems that ingest real public data and turn it into something you can actually make decisions with. Three of the most substantial below.

#### 🌍 [Sovereign](https://sovereign-rust-two.vercel.app) — geopolitical risk intelligence
Continuously ingests live public data across ~75 countries, fuses it into a typed `Country` ontology, runs a contagion model over the resulting graph, and exposes it through a dashboard with a natural-language LLM analyst chat. Outputs a composite **0–100 risk score** per country plus cross-border spillover alerts modelled on financial correlation, trade openness and regional adjacency. Free, no-paywall connectors only: World Bank WDI/WGI, FRED, OFAC SDN, country-proxy ETFs, VADER-scored news from 11 outlets, GDELT, Open-Meteo. 15-minute fast cycle, 6-hour full cycle.

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

#### ⚖️ [To Scale](https://alphacode-production.up.railway.app) — balance sheets at true proportion
Every US public company's balance sheet rendered at real scale from SEC filings, so a bank, a retailer and a software company produce visibly different shapes. Nothing estimated: where a company doesn't report a line item, the page says so. Built on **1.24M as-reported facts across 5,944 companies and seven quarters**, loaded from SEC bulk datasets. The hard part was selection — JPMorgan reports total assets 23 times in one filing and exactly one row is consolidated; mapping noncontrolling interests and bank-specific tags raised the accounting-identity pass rate from 78.6% to **99.9%** (`assets = liabilities + equity` within 1%).

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

![stats](https://github-readme-stats.vercel.app/api?username=DOMCHURCH&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true)
![langs](https://github-readme-stats.vercel.app/api/top-langs/?username=DOMCHURCH&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

</div>

---

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/DOMCHURCH/DOMCHURCH/output/github-snake.svg" />
</picture>
</div>
