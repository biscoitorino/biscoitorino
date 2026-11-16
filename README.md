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

### Projects

**[poly-gamer](https://github.com/biscoitorino/poly-gamer)** — Systematic trading platform in Python

Full lifecycle in one system: market discovery, real-time data ingestion over WebSockets, strategy logic, risk controls, order execution and a monitoring dashboard. Includes a tick-replay backtesting engine (P&L, win rate, profit factor, drawdown) and a parameter optimizer running grid search on GPU via OpenCL, with CPU fallback.

The part I care most about is the failure handling. It trades real money, so the dangerous state isn't a crash — it's a system that looks healthy while acting on stale prices. Every tick is timestamped and checked; positions that no longer match live market state get flagged; a daily loss cap and cooldown windows halt trading entirely; and a dry-run mode exercises the full pipeline without placing orders.

`Python` · `SQLite` · `WebSockets` · `OpenCL` · `REST API`

**[StreamVault](https://github.com/biscoitorino/StreamVault)** — Streaming archive extraction for Windows

Downloads and extracts archives at the same time, so you never need disk space for both the compressed file and its contents. Supports ZIP, TAR and single-volume RAR through HTTP range requests, with a graceful fallback for formats that can't be streamed.

`Python` · `PySide6` · `pytest` · `GitHub Actions` · `PyInstaller`

---

### Previously

**ScARF** (Pixlog, 2021–2026) — A computer vision system that replaced manual timber measurement with real-time measurement from a phone camera. No depth sensor, no specialized hardware. I architected it in C# and Unity, wrote the detection algorithms and the screen-to-metric coordinate math, and integrated ML models to run fully on-device so it worked offline in the field for 3–4 continuous hours. It shipped to industrial clients and ran in production for years.

---

B.Sc. Computer Science, Universidade Federal do Paraná (UFPR)

[LinkedIn](https://www.linkedin.com/in/matheus-de-almeida-arseno-5122131ba) · matheu.arseno@gmail.com
