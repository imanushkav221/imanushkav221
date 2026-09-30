## Anushka Verma

**Data Lead. Data engineering and analytics engineering.**

I build the pipelines, stores and checks that research and trading teams run on. Five years on energy and commodity market data at Bloomberg and Wood Mackenzie: sourcing it, validating it before it loads, orchestrating the runs, and owning the models and client-facing datasets on top.

Right now I take fractional data engineering work with early-stage teams, and I am open to the right full-time lead data engineering/ CTO role.

Delhi, India. Open to remote, hybrid and relocation.

[LinkedIn](https://www.linkedin.com/in/anushka-the-data-girl) &nbsp;&middot;&nbsp; [Resume](https://github.com/imanushkav221/imanushkav221/blob/main/Anushka_Verma_Resume.pdf) &nbsp;&middot;&nbsp; imanushkav221@gmail.com

---

### What I work with, by pipeline layer

One pipeline per dataset, always the same shape: ingestion, transformation, a check layer, then publish to the main store.

| Layer | What I use, and how I think about it |
| --- | --- |
| **Ingestion** | Exchange and vendor files, REST and websocket APIs, news feeds, web scraping, analyst hand-off forms. Mostly trigger and event based rather than scheduled. Cursors and high-water marks with an overlap window, dedupe at commit. |
| **Transformation** | Python, Pandas, NumPy, SQL, dbt, Spark. Contract roll and back-adjustment, point-in-time reference data so a backtest sees only what was known then. |
| **Checks** | Data contracts with cross-field rules, quarantine rather than a half-loaded table, blocking asset checks that stop a bad run before anything downstream sees it. |
| **Storage** | Snowflake, QuestDB, Postgres, Trino over a lake. Partitioning and ordering chosen for the query the desk actually runs, not for whatever is convenient to write. |
| **Orchestration** | Airflow, Dagster. Software-defined assets, retries and backfills, trading and publication calendars so a closed market is not mistaken for a late file. |
| **Serving** | Enterprise data APIs and client-facing portals. Schema design, release management, and being the person clients escalate to. |
| **Monitoring** | Prometheus, Grafana, Alertmanager. Deadline-relative staleness, freshness and completeness alerts that stay quiet when the market is shut. |
| **Modelling** | scikit-learn, time-series forecasting, scenario modelling, walk-forward validation with purge and embargo. Power BI, Tableau, Sisense for the visuals on top. |
| **LLM work** | Tool-calling agents for collection and extraction, RAG with embeddings and vector search, evaluation and fine-tuning. Claude Code and Cursor in the build loop. |

---

### Experience

**Bloomberg** &nbsp;&middot;&nbsp; Data Lead &nbsp;&middot;&nbsp; Jun 2024 to Sep 2026

Python and SQL pipelines behind the New Energy Outlook, orchestrated with Airflow and dbt and loading into Snowflake. Owned the Data Viewer and the Enterprise Data API end to end: schema design, release management and client support. Built the shipping and aviation datasets and their modelling frameworks from nothing. Moved four legacy Excel models into Python and took per-model runtime from about a week to four or five minutes, which is what made parallel runs possible. Maintained global datasets of over a million data points across power, transport, industry and buildings. Built LLM agents for automated collection and extraction. Supported more than ten analysts.

**Wood Mackenzie** &nbsp;&middot;&nbsp; Jul 2021 to Jun 2024

*Data Analyst, Data Processing Team Lead &nbsp;&middot;&nbsp; Nov 2023 to Jun 2024.* CI/CD pipelines for Lens on AWS SageMaker, with Spark behind the heavy processing. Led a team of ten and shipped more than seventy recurring automated workflows a year in place of manual reports and legacy tools. Owned the customer-facing Power and Renewables portal, built in Sisense over more than a hundred predictive models. Added automated ArcGIS validation to the hydrogen, ammonia and methanol datasets, where there had been none.

*Senior Data Associate, Data Optimization Lead &nbsp;&middot;&nbsp; Nov 2022 to Nov 2023.* Took global upstream M&A ingestion from people watching their inboxes and pasting deals into Excel to an automated feed end to end: tracking, ingestion, orchestration and load. Built demand forecasting models for global oil and gas.

*Data Associate &nbsp;&middot;&nbsp; Jul 2021 to Nov 2022.* First member of the Commodity Analytics team in India. It was twelve or thirteen people by the time I left.

---

### Selected projects

| Project | What it is | Why it is here |
| --- | --- | --- |
| **[market-data-platform-for-hft](https://github.com/imanushkav221/market-data-platform-for-hft)** | Commodity and crypto market data taken from where it is published to where a researcher can query it. QuestDB store built for as-of joins, Dagster orchestration with blocking asset checks, data contracts enforced before load, deadline-aware monitoring in Prometheus and Grafana, and a walk-forward forecasting model on top. | The one to read. It is a whole platform rather than a notebook, and the design decisions are written down with the benchmarks behind them. |
| **EV Infrastructure Intelligence** | Python pipelines collecting and standardising EV charging infrastructure data across India, with extraction, cleaning and validation automated off public sources. | Building a dataset that did not exist from sources that were never meant to be joined. Code not public. |
| **LLM Shopping Assistant** | A Claude-based assistant with tool calling that answers shopper questions in Instagram and Facebook DMs from a store's live Shopify catalogue. Multi-language replies, GDPR double opt-in, multi-tenant routing. TypeScript and Postgres. | Agents wired to a live system with real tenants, not a demo. Code not public. |
| [guesstimate1](https://github.com/imanushkav221/guesstimate1) | Guesstimating the number of internships offered in India every year. | Older. Structuring an estimate when there is no dataset to query. |
| [stanfordopenpolicing](https://github.com/imanushkav221/stanfordopenpolicing) | Exploratory analysis of the Stanford Open Policing dataset. | Older. Notebook work from when I was moving into data. |
| [gamestatistics](https://github.com/imanushkav221/gamestatistics) | Statistics on game data. | Older. Same. |

---

### Education and certifications

B.Sc. Mathematics and Statistics, University of Lucknow, 2017 to 2020.

Data Analyst Career Track using Python (DataCamp) &nbsp;&middot;&nbsp; Data Visualization with Tableau Specialization (UC Davis) &nbsp;&middot;&nbsp; Google Kick Start Round A, rank 206 &nbsp;&middot;&nbsp; HackerRank SQL silver badge.
