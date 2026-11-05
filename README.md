<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./img/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./img/banner-light.svg">
  <img alt="James Kinyua, Data and AI Engineering, Nairobi, Kenya" src="./img/banner-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://linkedin.com/in/james-kinyua00"><b>LinkedIn</b></a> &nbsp;·&nbsp;
  <a href="mailto:jameskinyua190@gmail.com"><b>Email</b></a> &nbsp;·&nbsp;
  <a href="#data-engineering"><b>Data</b></a> &nbsp;·&nbsp;
  <a href="#ai-engineering"><b>AI</b></a> &nbsp;·&nbsp;
  <a href="#live-production-systems"><b>Live systems</b></a>
</p>

I build data pipelines, streaming services and LLM applications. My focus is data and AI engineering, backed by 7+ years shipping production software for a national financial regulator, the Nairobi Securities Exchange, SACCOs and international health organisations.

As a Lead Full Stack Developer at Agile Business Solutions, I lead a team of 10 and stay hands-on in the code. That means I treat pipelines and AI features like any other production system: tested, monitored and able to handle failure.

<table>
  <tr>
    <td align="center" width="25%"><h3>28,463</h3>food price records modelled in my Airflow and PostgreSQL warehouse</td>
    <td align="center" width="25%"><h3>~0.2%</h3>dropped live market feed packets after the Go rewrite I led</td>
    <td align="center" width="25%"><h3>10,000+</h3>student users on NSE Virtual Trader, about 2,000 active daily</td>
    <td align="center" width="25%"><h3>~300</h3>SACCOs onboarded to the regulator's supervisory system</td>
  </tr>
</table>

## Data engineering

| Project | What it does | Stack |
|---|---|---|
| **[Kenya Food Prices and Inflation Platform](https://github.com/jimkinyua/kenya-food-market-analytics)** | Tracks food prices across Kenya's 47 counties to detect regional inflation. A five-task Airflow DAG checks the source, downloads WFP market data with integrity checks, cleans it in pandas and loads PostgreSQL. It converts bag prices to per-kg prices, maps old districts to current counties and models 51 commodities across 226 markets since 2006 in a Kimball star schema, with six automated quality checks and Grafana geomaps. | Python, pandas, Airflow, PostgreSQL, Grafana |
| **[JobRadar](https://github.com/jimkinyua/JobRadar)** | Pulls job listings from APIs, RSS feeds and scrapers into Bronze, Silver and Gold PostgreSQL tables, resolves duplicates across sources, scores each role against several career profiles and sends Telegram alerts. It also syncs application status with Notion. | Python, PostgreSQL, Pydantic, pytest |
| **[Weather and Crypto ETL Pipeline](https://github.com/jimkinyua/etl-pipeline)** | Extracts weather data from OpenWeather and ticker data from Binance, normalizes units and timestamps and loads the results into both a relational store and a wide-column store. | Python, PostgreSQL, Cassandra |

## AI engineering

| Project | What it does | Stack |
|---|---|---|
| **[DocuHelp](https://github.com/jimkinyua/DocuHelp)** | RAG service for PDF, DOCX and TXT files. It splits documents into overlapping chunks, stores their embeddings in a vector database and answers questions using only the uploaded content, with a choice of LLM provider. | FastAPI, ChromaDB, sentence-transformers, Groq, OpenAI, Gemini |
| **[JobRadar AI layer](https://github.com/jimkinyua/JobRadar)** | Uses an LLM for fallback data extraction and career-fit analysis, with schema-checked outputs and a keyword fallback so the pipeline keeps working when the model fails. | Gemini, Pydantic |

**Private tools in use (code not public):**

- **CV parsing and shortlisting:** a RAG tool that turns unstructured CVs into structured data.
- **User stories to developer tasks:** an internal LLM tool in daily use that converts user stories into developer-ready tasks.
- **Workflow automation over MCP:** a tool that creates sprint tasks and moves issues through workflow states based on commit messages.
- **Local models:** moved AI workloads from the OpenAI API to locally hosted models on Ollama for cost and privacy.

## Live production systems

Systems I built or helped build. Most sit behind a login, so the links open the sign-in or landing page.

| System | What it does |
|---|---|
| **[NSE Virtual Trader / SOKO PLAY](https://academy.nse.co.ke)** | Investor-education trading platform for the Nairobi Securities Exchange, built with TradingView as a partner on the upgraded version. It streams live market data while handling orders and student payments. Its market feed runs on a Go rewrite using Kafka. |
| **[SASRA Risk-Based Supervisory System](https://sacco.sasra.go.ke)** | Kenya's SACCO regulator uses it for supervisory reporting. SACCOs submit data through APIs. The platform validates it, scores risk on liquidity, governance and capital adequacy and feeds supervisory dashboards. It runs as microservices over Kafka and issues tax-compliant invoices and credit notes through KRA eTIMS. |
| **[NSE Quotations Board](https://bondsquotations.nse.co.ke)** | Ingests, validates and publishes government and corporate bond quotes reported by banks for the secondary market. |
| **[Britam Pension Member Portal](https://pensionmembers.britam.com)** | Lets pension members sign in with their national ID or passport number and access their pension accounts online. |
| **[Mhasibu SACCO Member Portal](https://members.mhasibusacco.com)** | Lets members manage accounts, apply for loans and transact online, with M-Pesa and PayPal payments, CRB checks and IPRS identity verification. |
| **[Ushuru SACCO Member Portal](https://webportal.ushurusacco.com:8060/site/login)** | Gives members access to balances, statements, loan services and personal details online, integrated with Microsoft Business Central. |

**Also delivered (internal staff systems, not public):** Employee Self-Service portals on Dynamics 365 Business Central for AMREF Health Africa, IITA Nigeria, The Global Fund Indonesia and KEMRI Wellcome Trust Research Programme.

**More public code:** [Mini Ticket Tracker](https://github.com/jimkinyua/LodwarServices) (TypeScript, Express, Prisma, React) and [Social Assistance Information System](https://github.com/jimkinyua/SAIS) (ASP.NET Core, EF Core, SQL Server).

## What I work with

<table>
  <tr><td><b>Data</b></td><td><code>Airflow</code> <code>Kafka</code> <code>pandas</code> <code>ETL/ELT</code> <code>Star schemas</code> <code>Medallion architecture</code> <code>Data quality checks</code> <code>Grafana</code></td></tr>
  <tr><td><b>AI</b></td><td><code>RAG</code> <code>Embeddings</code> <code>ChromaDB</code> <code>Ollama</code> <code>Gemini</code> <code>OpenAI</code> <code>Groq</code> <code>MCP</code></td></tr>
  <tr><td><b>Databases</b></td><td><code>PostgreSQL</code> <code>SQL Server</code> <code>MySQL</code> <code>Azure SQL</code> <code>Cassandra</code></td></tr>
  <tr><td><b>Languages</b></td><td><code>Python</code> <code>SQL</code> <code>Go</code> <code>C#</code> <code>PHP</code> <code>TypeScript</code> <code>JavaScript</code></td></tr>
  <tr><td><b>Frameworks</b></td><td><code>FastAPI</code> <code>Django</code> <code>Flask</code> <code>ASP.NET Core</code> <code>Laravel</code> <code>React</code> <code>Angular</code></td></tr>
  <tr><td><b>Cloud and delivery</b></td><td><code>Azure</code> <code>Azure DevOps</code> <code>Docker</code> <code>Git flow</code> <code>Key Vault</code> <code>Entra ID</code></td></tr>
  <tr><td><b>Testing</b></td><td><code>TDD</code> <code>pytest</code> <code>xUnit</code> <code>Playwright</code> <code>Postman</code> <code>k6</code> <code>JMeter</code></td></tr>
</table>

## How I build

- **Check the data, don't trust it.** Pipelines get integrity checks and automated quality assertions before anything reaches a dashboard.
- **Plan for model failure.** LLM outputs get schema checks and a non-AI fallback.
- **Tests first.** I practise test-driven development and back releases with automated tests.
- **Assume integrations fail.** Payment integrations get idempotency, retries, timeouts and circuit breakers.

## Get in touch

Reach me at **[jameskinyua190@gmail.com](mailto:jameskinyua190@gmail.com)** or on **[LinkedIn](https://linkedin.com/in/james-kinyua00)**.

Outside work, I play piano and sing in a choir.
