## Matheus de Almeida Arseno

Software engineer based in Curitiba, Brazil. I build backend systems in **C#/.NET** and **Python**, and I've spent the last few years taking products from first prototype to running in production.

I started as an AR engineer at Pixlog, became Head of Augmented Reality in about a year, and later Technical Lead — leading a team of four while still writing code daily. These days I'm building open source.

**What I work on**

- Backend systems, REST APIs and system integration — C#, .NET, Python, Node.js
- Computer vision and on-device ML inference
- Real-time data pipelines: WebSocket ingestion, stale-state detection, failure recovery
- PostgreSQL, SQL Server, MongoDB — schema design and query optimization
- AI coding agents as part of my daily workflow, with every generated line reviewed before it ships

---

### Skills

**Languages**

![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge)

**Backend & frameworks**

![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST%20APIs-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=for-the-badge&logo=socketdotio&logoColor=white)
![Qt](https://img.shields.io/badge/PySide6%20%2F%20Qt-41CD52?style=for-the-badge&logo=qt&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

**Computer vision & ML**

![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white)
![AR](https://img.shields.io/badge/Augmented%20Reality-FF4F00?style=for-the-badge)
![On-device ML](https://img.shields.io/badge/On--device%20ML-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![OpenCL](https://img.shields.io/badge/OpenCL%20%2F%20GPU-ED1C24?style=for-the-badge&logo=amd&logoColor=white)

**Tooling & delivery**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Claude Code](https://img.shields.io/badge/AI%20coding%20agents-D97757?style=for-the-badge&logo=anthropic&logoColor=white)

---

### Projects

**[poly-gamer](https://github.com/biscoitorino/poly-gamer)** — Systematic trading platform in Python

Full lifecycle in one system: market discovery, real-time data ingestion over WebSockets, strategy logic, risk controls, order execution and a monitoring dashboard. Includes a tick-replay backtesting engine (P&L, win rate, profit factor, drawdown) and a parameter optimizer running grid search on GPU via OpenCL, with CPU fallback.

The part I care most about is the failure handling. It trades real money, so the dangerous state isn't a crash — it's a system that looks healthy while acting on stale prices. Every tick is timestamped and checked; positions that no longer match live market state get flagged; a daily loss cap and cooldown windows halt trading entirely; and a dry-run mode exercises the full pipeline without placing orders.

`Python` · `SQLite` · `WebSockets` · `OpenCL` · `REST API`

**[StreamVault](https://github.com/biscoitorino/StreamVault)** — Streaming archive extraction for Windows

Downloads and extracts archives at the same time, so you never need disk space for both the compressed file and its contents. Supports ZIP, TAR and single-volume RAR through HTTP range requests, with a graceful fallback for formats that can't be streamed.

`Python` · `PySide6` · `pytest` · `GitHub Actions` · `PyInstaller`

**[Crafting-Materials-Checker](https://github.com/biscoitorino/Crafting-Materials-Checker)** — Market-aware crafting cost and profit tool for FFXIV

Prices all 13,892 crafting recipes against live market data from the Universalis API. Since listings can only be bought as whole stacks, the cheapest price per unit isn't necessarily the cheapest buy. So for each material it finds the set of listings that covers the quantity needed at the lowest total cost, and compares that against NPC vendor prices. Prices use the week's median sale capped at the cheapest live listing, so outlier sales can't inflate the estimates. A profit finder ranks everything a player can craft by margin and weekly sales volume. It ships as a single Windows executable (Node.js single-executable application) with no install required.

`Node.js` · `Fastify` · `REST API` · `esbuild` · `Optimization`

---

### Previously

**ScARF** (Pixlog, 2021–2026) — A computer vision system that replaced manual timber measurement with real-time measurement from a phone camera. No depth sensor, no specialized hardware. I architected it in C# and Unity, wrote the detection algorithms and the screen-to-metric coordinate math, and integrated ML models to run fully on-device so it worked offline in the field for 3–4 continuous hours. It shipped to industrial clients and ran in production for years.

---

B.Sc. Computer Science, Universidade Federal do Paraná (UFPR)

[LinkedIn](https://www.linkedin.com/in/matheus-de-almeida-arseno-5122131ba) · matheu.arseno@gmail.com
