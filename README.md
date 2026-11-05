# Hi, I'm Rudresh 👋

**AI/ML Engineer | LLM Agents & GenAI Systems | Python | AWS, Azure | 8+ Years Shipping Production ML**

📍 Atlanta, GA · [LinkedIn](https://www.linkedin.com/in/rudreshwar-toutam-8253251b9/) · [Portfolio](https://rudhrestam.github.io)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat&logo=apachespark&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)

## About me

I'm an AI/ML and data engineer with 8+ years of experience building production systems at enterprise scale — the kind where a wrong answer or a missed check has a real cost. My recent work centers on LLM agents and retrieval systems for operations teams, large-scale data pipelines, and automation frameworks that replace manual, error-prone processes. I care about the parts of AI that don't show up in demos: guardrails, validation, and measuring whether the system is still working a month after launch.

Currently a Database Automation Engineer at Morgan Stanley, working on AI tooling and infrastructure automation.

## Core skills

- **Languages:** Python, SQL, Scala, Shell scripting
- **ML / AI:** LLM agents, retrieval systems, scikit-learn, churn & predictive modeling, NLP
- **Data Engineering:** Apache Spark, Kafka, Airflow, ETL/ELT pipelines, data quality & validation frameworks
- **Cloud / DevOps:** AWS (Lambda, Glue, S3, EC2, SNS, CloudWatch), Azure, Redshift, Snowflake, Jenkins, CI/CD, ControlM

## Featured projects

Open-source demos of the patterns behind my production work — original code, sample data only:

### 🔎 [LLM Knowledge Retrieval Agent](https://github.com/rudhrestam/llm-knowledge-retrieval-agent)
A retrieval agent (Python + scikit-learn) that answers questions from runbooks and documentation with citations — and refuses rather than guessing when nothing supports an answer. Demo of the pattern behind the operations knowledge agent I built at Morgan Stanley, which the whole ops team adopted.

### 🩺 [Server Health Verification Framework](https://github.com/rudhrestam/server-health-verification-framework)
Parallel health-check automation with per-check validation, a summary report, and an audit log. The production version verifies 1,800 servers after OS patching — checks run 20 at a time — and eliminated ~800 manual hours per quarter, with zero missed checks since launch.

### 📊 [Customer Churn Prediction](https://github.com/rudhrestam/customer-churn-prediction)
Customer-360 style churn modeling on synthetic data: transaction, engagement, and feedback-sentiment features feeding a classifier and a daily-insights summary. Based on the McDonald's platform that combined nightly data from 18,000+ restaurants with sentiment and clickstream signals — models at 70–90% accuracy.

### 🔄 [Global ETL Data Pipeline](https://github.com/rudhrestam/global-etl-data-pipeline)
Batch ETL with a data-quality layer that reverts and quarantines bad files instead of loading them. Based on the McDonald's pipeline that moved 30+ GB/day from 6+ global markets (AWS, Kafka, Airflow) inside a strict 3-hour SLA.

### ☀️ [Solar Grid Efficiency AI](https://github.com/rudhrestam/solar-grid-efficiency-ai)
A personal project exploring AI in energy systems: a simulated solar plant (100% synthetic data) that tracks the full loss chain between generation and grid export — soiling, degradation, downtime, inverter and wiring losses, curtailment — then uses ML to forecast generation, flag underperforming strings, and rank which losses are worth fixing. In the demo run, 16.2% of generated energy never reaches the grid, and the detector finds the two planted faults exactly.

### 🏥 [Healthcare Claims Intelligence](https://github.com/rudhrestam/healthcare-claims-intelligence)
Denial prediction on 5,930 synthetic claims: a GradientBoosting model (ROC-AUC 0.795) scores denial risk before submission, and the analysis ranks the drivers — missing prior authorisation (63.9% denied vs 16.2% without) and coding mismatches lead — plus an estimate of the denied dollars recoverable by fixing the top one. Synthetic data only; a standalone demo of the claims-analytics pattern.

### 🛡️ [Regulatory Reporting Data Quality](https://github.com/rudhrestam/regulatory-reporting-data-quality)
A pre-submission data-quality framework for financial reporting extracts: 14 named checks across schema, completeness, validity, uniqueness, consistency, and reconciliation against a control file. In the demo, all 295 planted defects in 5,040 synthetic records are caught and quarantined — a 94.15% DQ score, with the reconciliation deltas explained.

### 🍽️ [Restaurant Demand Forecasting](https://github.com/rudhrestam/restaurant-demand-forecasting)
Daily demand forecasting for 8 synthetic restaurants: a RandomForest over day-of-week, holidays, weather, promotions, events, and feedback sentiment forecasts orders with test MAE 28.0 (R² 0.832), beating a same-weekday-last-week baseline by 22.6% — then turns next week's forecast into prep and staffing tiers per location.

### 🖥️ [Server Log Anomaly Detection](https://github.com/rudhrestam/server-log-anomaly-detection)
A generic log-anomaly demo over ~190K synthetic log lines from 10 hosts: logs are parsed into per-host 30-minute windows and scored two ways — IsolationForest and per-host z-score baselines. Between them they catch 42 of 46 planted anomaly windows (an error burst, a latency spike, and one host failing slowly), with the false positives discussed honestly.

### 🧱 [dbt Analytics Engineering](https://github.com/rudhrestam/dbt-analytics-engineering)
A full dbt project on synthetic commerce data: staging, intermediate, and mart models with 31 tests — `dbt build` passes 39/39, and the data-quality mart catches all 19 planted order-total mismatches plus 12 empty orders, reconciling $158,019.67 of revenue across 3,304 completed orders. Built to demonstrate the analytics-engineering patterns behind production pipeline work.

### 🦜 [LangChain RAG Agent](https://github.com/rudhrestam/langchain-rag-agent)
A LangChain retrieval agent over a small operations-runbook corpus with MiniLM embeddings and a distance-based guardrail: in evaluation it answers 13/13 test questions with the correct source at rank 1, and refuses all 3 off-corpus questions instead of hallucinating. A companion to the LLM Knowledge Retrieval Agent above, built with the framework stack.

### ☸️ [Docker & Kubernetes ML Service](https://github.com/rudhrestam/docker-kubernetes-ml-service)
A small ML model (ROC-AUC 0.7964) packaged as a containerized FastAPI-style service with Kubernetes deployment and service manifests: a 60-prediction smoke test runs at p95 latency 63.9 ms. All manifests validated locally; the build sandbox had no Docker daemon, so the image build itself is documented rather than claimed.

## Experience

I started out as a Python developer and data engineer at Iplace Software Solutions, building ETL for medical-device and healthcare data, then moved to BlueCross BlueShield, where I automated multi-source healthcare claims processing with Spark and Kafka — 300 claims in parallel, ~45% faster processing, and 10–15% fewer rejections. From there I joined E*TRADE as a Python developer and data engineer, leading a Python 2.7 → 3.8+ migration of a legacy automation codebase to 80% test coverage and automating quarterly SEC regulatory data submissions, and spent time at GE Aviation building multi-source ingestion and data-quality workflows feeding analytics.

At McDonald's, as a senior Python developer and data engineer, I ran a global data pipeline moving 30+ GB/day from 6+ markets inside a 3-hour SLA and built the Customer 360 churn platform over nightly data from 18,000+ restaurants — models at 70–90% accuracy, with insights delivered daily. Today I'm a Database Automation Engineer at Morgan Stanley, where I build LLM retrieval tooling for the operations team and large-scale automation, including a post-reboot verification framework that checks 1,800 servers and eliminated ~800 manual hours per quarter.

## Education & certification

- 🎓 Master's Degree, Computer Science — Texas A&M University-Kingsville
- ☁️ AWS Certified Data Engineer – Associate — Amazon Web Services

## Get in touch

- LinkedIn: [linkedin.com/in/rudreshwar-toutam-8253251b9](https://www.linkedin.com/in/rudreshwar-toutam-8253251b9/)
- Portfolio: [rudhrestam.github.io](https://rudhrestam.github.io)
- Email: rudhrestam@gmail.com
