<div align="center">

<img src="https://raw.githubusercontent.com/Ameya79/Ameya79/main/ChatGPT Image Aug 3, 2026, 08_35_36 PM (1).png" width="100%" alt="banner" />

<br/>

# Ameya Kulkarni

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=15&pause=1200&color=8B9EC7&center=true&vCenter=true&width=520&lines=Python+Developer+%26+Open-Source+Builder;Maintainer+%40+Mustel+%C2%B7+4%2C400%2B+PyPI+Downloads;AI+Systems+Evaluation+%40+AirDawg+Labs;TCET+Information+Technology+%2728)](https://github.com/Ameya79)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ameya-kulkarni-a31b74246)
&nbsp;
[![PyPI](https://img.shields.io/badge/PyPI-3775A9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/mustel)
&nbsp;
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:ameyakulkarnialt@gmail.com)
&nbsp;
[![The Free University](https://img.shields.io/badge/The_Free_University-000000?style=flat-square&logo=vercel&logoColor=white)](https://thefreeuniversity.space)

</div>

<br/>

```
currently: building in public, shipping real tools, two internships deep
```

<br/>

## what's going on

- Building a Next.js AI Literacy Portal at TCET Centre of Excellence and internal automation tools in Python (May 2026)
- AI Systems Evaluation Intern at AirDawg Labs on Project Terminus-2nd-Edition by Snorkel AI, reviewing and submitting benchmark tasks used to train frontier models for OpenAI and Anthropic (Jun 2026)
- Maintaining **[Mustel](https://pypi.org/project/mustel)**, a Python CLI and MCP server with 4,400+ PyPI downloads
- Founded **[The Free University](https://thefreeuniversity.space)** with 90,000+ lifetime visits and 1,000+ LinkedIn followers

<br/>

## featured work

<br/>

### [Mustel](https://mustel.vercel.app) · `pip install mustel` · [PyPI](https://pypi.org/project/mustel) · [repo](https://github.com/mustel-py/mustel)

Non-AI static analysis layer for AI coding agents (Cursor, Claude Code, Windsurf). Deterministic scanning, no model calls, no hallucinated findings.

[![Python](https://img.shields.io/badge/Python_3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![PyPI](https://img.shields.io/pypi/v/mustel?style=flat-square&color=3775A9)](https://pypi.org/project/mustel)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://github.com/mustel-py/mustel/blob/main/LICENSE)

- Orchestrates three engines (Ruff, Bandit, pip-audit) plus 20 custom YAML pattern files covering `subprocess`, `requests`, `flask`, `django`, `pickle`, `asyncio`, and more
- Normalizes everything into a schema-versioned JSON report, with a precomputed `agent_prompt` field so an AI agent can act on it without parsing the raw output
- Ships an MCP server (`mustel serve`) exposing `review`, `review_file`, `env`, and `check_package` tools for direct IDE and agent integration
- Benchmarked at 100% recall across 14 planted bugs in 4 test projects, 0 false positives on a clean baseline

```bash
mustel review        # scan current directory, outputs JSON
mustel serve          # run as an MCP server for AI IDEs
```

<br/>

### [Driftwood](https://driftwood-docs.vercel.app/docs) · [repo](https://github.com/Ameya79/Driftwood)

Stateless Monte Carlo simulation API for stock price paths, built on Geometric Brownian Motion (GBM).

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)](https://nextjs.org)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)

- FastAPI backend, fully stateless, no auth keys required, single `POST /v1/simulate` endpoint
- Vectorized NumPy computation returns 1,000 simulated paths in milliseconds
- Returns p10/p50/p90 percentile price envelopes along with annualized volatility and probability-of-profit
- Rate limited at both the Nginx layer (20 r/s, burst 30) and the app layer (100 requests per 5s per IP)
- Full stack runs via Docker Compose: FastAPI backend, Next.js frontend, Nginx reverse proxy

<br/>

### [rollit](https://rollit-website.vercel.app) · `pip install rollit` · [repo](https://github.com/Ameya79/rollit) · [PyPI](https://pypi.org/project/rollit/)

Rolling window statistics for NumPy arrays, without pulling in pandas.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org)
[![PyPI Version](https://img.shields.io/pypi/v/rollit?style=flat-square&color=3775A9)](https://pypi.org/project/rollit)
[![CI](https://github.com/Ameya79/rollit/actions/workflows/ci.yml/badge.svg)](https://github.com/Ameya79/rollit/actions/workflows/ci.yml)

- `mean`, `std`, `sum`, `min`, `max`, `zscore`, `normalize`, `apply`, all under one consistent function signature
- Uses `numpy.lib.stride_tricks.as_strided` for zero-copy windowing, and locks the returned views read-only to avoid segfault-prone manual stride math
- Supports `min_periods` to mask incomplete windows instead of failing on them
- 700+ monthly PyPI downloads, CI on every push via GitHub Actions

<br/>

### [Squeezy](https://squeezy-image-compressor.onrender.com) · [repo](https://github.com/Ameya79/Squeezy-Image-Compressor)

Flask app for image compression, resizing, and image-to-PDF merging, all done in memory.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Pillow](https://img.shields.io/badge/Pillow-3776AB?style=flat-square&logo=python&logoColor=white)](https://python-pillow.org)

- `BytesIO`-based processing, no files touch disk beyond the request lifecycle
- Resize by percentage, adjustable JPEG/PNG compression quality
- Merges multiple uploaded images into a single PDF
- Files auto-delete 5 seconds after generation, no logging, no stored metadata

<br/>

### [The Free University](https://thefreeuniversity.space)

A free course and certification aggregator I founded and grew from scratch. It manually vets free courses and certifications from providers like Google, Harvard, IBM, Cisco, and freeCodeCamp, and runs interactive in-browser learning spaces (including a Python zero-to-production track with live code execution) plus instant Python and web compilers, so people can learn without wading through paywalled content.

- 90,000+ lifetime visits, 1,000+ LinkedIn followers
- 117+ certifications listed, all manually reviewed
- Built and SEO-optimized from scratch, zero paid promotion

<br/>

## internships

<br/>

**AI Systems Evaluation Intern · AirDawg Labs** &nbsp;`Jun 2026 – Present`

Working on Project Terminus-2nd-Edition by Snorkel AI. Reviews AI coding agent benchmark tasks for instruction clarity, test alignment, rubric quality, metadata correctness, Docker/base image compliance, and solution leakage risks. Evaluates full task submissions by inspecting task environments, verifier reports, Dockerfiles, `task.toml`, and oracle solutions before making Accept / Needs Revision decisions. Also contributed as a task submitter before moving to the reviewer side. Ubuntu / WSL, Docker, Python.

**Software Intern · TCET Centre of Excellence** &nbsp;`May 2026 – Present`

Contributing to a Next.js web portal for AI literacy training. Building Python-based internal automation tools.

**Research Analyst → Associate Data Analyst · CoreLayer Labs (Review.AI)** &nbsp;`Oct 2024 – Feb 2025`

Built an LLM-powered product-page scraper cutting manual review time by 75%. Built a real-time Streamlit dashboard integrated with Google Sheets for team workload tracking. Researched and documented 50+ AI tools.

<br/>

## activity

<div align="center">

<img src="https://streak-stats.demolab.com?user=Ameya79&theme=tokyonight&hide_border=true&fire=8B9EC7&currStreakLabel=8B9EC7" height="160" alt="github streak stats" />

<br/><br/>

<img src="https://skillicons.dev/icons?i=python,fastapi,flask,nextjs,docker,git,mysql&theme=dark" height="50" alt="tech icons" />

</div>

<br/>

## highlights

- **Problem Setter · Shastra Coding Club, TCET.** Designs and validates test cases for T&P coding assessments
- **Mumbai Hacks 2025.** Built LifeLink (AI organ donation platform), qualified for Round 2 offline of India's largest agentic AI hackathon (HealthTech track)
- **CGPA 9.21 / 10** · B.E. Information Technology, Mumbai University

<br/>

*Mumbai · open to opportunities*

</div>
