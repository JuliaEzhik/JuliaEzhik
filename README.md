<h1 align="center">Julia Zhuravleva</h1>
<h3 align="center">Senior Data Engineer — data systems, BI and analytics in Munich</h3>

<p align="center">
Data Engineer with 6+ years of experience designing, building and operating production data systems
and scalable ETL/ELT pipelines. I work with engineering and business stakeholders to turn complex
requirements into reliable, maintainable data solutions.
</p>

<p align="center">
📍 Munich, Germany · 🎓 M.Sc. Statistical Modelling and Actuarial Science, HSE (2021)
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/julia-zhuravleva-8669b2236/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/JuliaEzhik/llm-leaderboard-elt"><img src="https://img.shields.io/badge/Flagship-LLM_Leaderboard_ELT-181717?style=for-the-badge&logo=github&logoColor=white" alt="Flagship project"></a>
  <a href="https://github.com/JuliaEzhik/julia-zhuravleva-portfolio"><img src="https://img.shields.io/badge/Portfolio-181717?style=for-the-badge&logo=github&logoColor=white" alt="Portfolio"></a>
</p>

---

## What I solve for companies

- **Production ETL/ELT pipelines.** End-to-end data workflows with Python, SQL, Apache Spark, dbt and Airflow — built to run reliably, not as one-off scripts.
- **Data modeling, quality and monitoring.** Clear definitions, tests and automation so stakeholders can trust the numbers. Hands-on with Great Expectations and test automation.
- **Cloud-native data architecture on GCP.** Warehouses and services with BigQuery, PostgreSQL, Cloud Functions and Terraform.
- **Analytics that support decisions.** KPI dashboards and reporting, from requirement-gathering with the business to delivery.
- **Event-driven tracking and serverless processing.** Capture and process user interactions, then automate the workflows behind them.

## Proof, not promises

- **24%** lower system load and waiting time after leading the analytical evaluation of a reconciliation-system redesign (UniCredit, via Convolut).
- An **AI agent** for regulatory documentation and reporting that cut template completion time by **43%**.
- Monitoring of **100+** data sources automated with Python, reducing manual validation effort by **78%** (Raiffeisen Bank).
- **16%** higher credit-scoring model precision by building the path from the data lake and Greenplum into scoring data marts (Glowbyte).
- Payment-notification automation that reduced payment delays by **70%** (RESO-Guarantee).

## Featured projects

### 📊 [LLM Leaderboard ELT](https://github.com/JuliaEzhik/llm-leaderboard-elt) — daily snapshots, contracts and pipeline health

<a href="https://github.com/JuliaEzhik/llm-leaderboard-elt"><img src="https://raw.githubusercontent.com/JuliaEzhik/llm-leaderboard-elt/main/docs/screenshots/01-best-model-now.png" width="760" alt="LLM Leaderboard ELT dashboard: best model now"></a>

A daily batch pipeline that snapshots an LLM leaderboard, keeps history the source does not keep, and answers which model to use now and how the ranking changed. Built to show what matters after the first successful run: **schema contracts, incremental loads, data tests, and a check for what failed and what is late**.

- Airflow DAG: extract → contract check → dbt build → health check
- Landing, curated and mart layers on DuckDB, plus a Streamlit dashboard
- Demo source is synthetic; the same pipeline can read a live API

`Airflow` `dbt` `DuckDB` `Python` `Streamlit`

### 📈 [Performance Analytics Dashboard](https://github.com/JuliaEzhik/performance-analytics-dashboard) — marketing and sales analytics

<a href="https://github.com/JuliaEzhik/performance-analytics-dashboard"><img src="https://raw.githubusercontent.com/JuliaEzhik/performance-analytics-dashboard/main/docs/screenshots/01-overview.png" width="760" alt="Performance analytics dashboard overview"></a>

Raw web events and bookings are modelled with **dbt** (bronze → silver → gold) on **DuckDB** and served in a bilingual (EN/DE) **Streamlit** dashboard. **All data is synthetic.**

- Traffic channels, conversion, CPL/ROAS, booking funnel and a data-quality tab
- **89 dbt data tests**, including reconciliation and funnel checks
- Sessionisation, channel grouping, and quality flags that stay auditable

`dbt` `DuckDB` `Streamlit` `Python` `pandas` `Plotly`

### 🍊 [Spanish Citrus Export Analytics](https://github.com/JuliaEzhik/spanish-citrus-export-analytics) — trade markets, competition and forecasts

<a href="https://github.com/JuliaEzhik/spanish-citrus-export-analytics"><img src="https://raw.githubusercontent.com/JuliaEzhik/spanish-citrus-export-analytics/main/docs/screenshots/01-overview.png" width="760" alt="Spanish citrus export destination heatmap"></a>

EU COMEXT trade flows modelled with **dbt** on **DuckDB**, explored in a **Streamlit** dashboard with maps, competition views and revenue forecasts.

- Destination demand, Spain’s EU share and top trade flows
- Competition by market and an export-revenue forecast
- Runs locally or with Docker

`dbt` `DuckDB` `Streamlit` `Plotly` `Docker`

### 🔗 [Airflow + dbt Data Vault](https://github.com/JuliaEzhik/airflow-dbt-data-vault) — orders to hubs, links, satellites and a mart

A small end-to-end demo of **Apache Airflow** orchestrating **dbt** models that build a **Data Vault** and a simple mart on Postgres from an online-store `raw.orders` stream.

- Hourly DAG: new orders → staging → hubs / link / satellite → `dm.stat_orders`
- Airflow 2.9 (LocalExecutor) and Postgres, started with Docker Compose
- dbt tests on the mart rebuild

`Airflow` `dbt` `PostgreSQL` `Docker` `Data Vault`

## Tech stack

| | |
|---|---|
| **Languages & data** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=sqlite&logoColor=white) ![Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) |
| **Warehousing & modeling** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white) ![Great Expectations](https://img.shields.io/badge/Great_Expectations-FF4510?style=flat-square) |
| **Orchestration & cloud** | ![Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white) ![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |
| **Analytics & apps** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![HTML](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white) |
| **Quality & AI tools** | ![pytest](https://img.shields.io/badge/Test_automation-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=claude&logoColor=white) |

## GitHub stats

<p align="center">
  <img height="180" src="https://github-readme-stats.vercel.app/api?username=JuliaEzhik&show_icons=true&hide_border=true&include_all_commits=true" alt="JuliaEzhik GitHub stats">
  <img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JuliaEzhik&layout=compact&hide_border=true" alt="Top languages">
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com/?user=JuliaEzhik&hide_border=true" alt="GitHub streak">
</p>

## Background

I have worked as a Data Engineer and Data Analyst in banking, consulting and product teams — most recently as Production System Owner at Svango in Munich, and before that at Convolut (UniCredit), Raiffeisen Bank, Glowbyte Consulting and RESO-Guarantee.

**Education:** M.Sc. in Statistical Modelling and Actuarial Science, HSE (2021) · B.Sc. in Applied Mathematics, Bauman MSTU (2019)

**Languages:** English — Fluent · German — Proficient · Russian — Native

---

<p align="center"><sub>Data systems · ETL/ELT · Analytics — built to run in production</sub></p>
