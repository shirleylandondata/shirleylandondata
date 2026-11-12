# Hi, I'm Shirley Landon 👋

## Data & Operations Analyst | SQL · Python · Power BI · Excel

### I turn messy business data into clear answers that people can act on.

I spent 15 years inside the operations that analysts report on: supporting investment teams, executives, and legal practices at The Carlyle Group, Goldman Sachs, Barclays, Viking Global Investors, and Kirkland & Ellis. I've maintained the CRM records, reconciled the expenses, tracked the pipelines, and produced the reports. I know where business data breaks, because I've worked downstream of it.

Now I build the analysis myself: defining the business question, validating the data, modeling it, and explaining what it means for the decision.

**Open to remote roles**: Business Systems Analyst · Data Analyst · Business Data Analyst · Operations Analyst · Reporting Analyst · Data Quality Analyst · Business Intelligence (BI) Analystt

📅 [Book an intro call](https://calendly.com/shirleymlandon/intro-meeting) · 💼 [LinkedIn](https://www.linkedin.com/in/shirleylandon/)

---

## ⭐ Spotlight: Payment Funnel Analysis — FinTech

**Where do payments fail on a digital payments platform, why do they fail, and how much order value is at stake?**

I analyzed **5,000 orders** in SQL across a five-stage payment funnel, classified **561 payment failures** by root cause, and compared six payment methods.

<img src="https://raw.githubusercontent.com/shirleylandondata/payment-funnel-analysis-fintech/main/images/funnel_conversion.png" alt="Payment funnel conversion by stage" width="720">

**What I found:**
- **Authorization is the bottleneck:** 662 orders (15.95%) are lost between Payment Attempted and Payment Authorized, the largest drop in the funnel.
- **Failures split evenly:** bank/processing issues (36.90%) and customer/payment-method issues (35.83%) cause nearly the same share of failures.
- **Volume isn't risk:** Card has the most failures only because it has the most orders. **Bank Transfer has the highest failure rate (12.60%)** and the lowest paid rate.
- **Every order reconciles:** 2,923 paid + 157 refunded + 86 chargebacks = 3,166 captured payments.

**Checking my own work:** comparing the failure categories against the raw decline reasons showed that 58 address (AVS) mismatches had been left unclassified. Fixing the rule changed the finding from "processing problems dominate" to "an even split between processor and customer causes."

**SQL:** CTEs · window functions (`LAG`, `FIRST_VALUE`) · `CASE` classification · `FILTER` aggregates · reconciliation queries

➡️ [View project](https://github.com/shirleylandondata/payment-funnel-analysis-fintech) · [See the SQL](https://github.com/shirleylandondata/payment-funnel-analysis-fintech/tree/main/sql)

---

## 📊 Featured Analytics Projects

| Project | Business question | Tools |
|---|---|---|
| 💳 **[Payment Funnel Analysis — FinTech](https://github.com/shirleylandondata/payment-funnel-analysis-fintech)** | Where do payments fail, why, and how much order value is at stake? | SQL · DuckDB · Hex |
| 📊 **[Sales Performance Dashboard](https://github.com/shirleylandondata/Sales-Performance-Dashboard)** | Which products, states, and categories drive revenue and profit across 1M transactions? | Power BI · Tableau · Excel |
| 🧹 **[Customer Data Cleaning & Validation](https://github.com/shirleylandondata/Customer-Data-Cleaning_Validation)** | Can 500K customer records with corrupted dates and codes be made trustworthy, and how do you prove it? | Power Query · Tableau · Excel |
| 🔮 **[Customer Churn Predictive Modeling](https://github.com/shirleylandondata/Customer-Churn-Predictive-Modeling)** | Which retail-banking customers are most likely to leave, and where should retention effort go? | Python · pandas · scikit-learn · Matplotlib · Seaborn |
| 📈 **[Executive KPI Command Center](https://github.com/shirleylandondata/Executive-KPI-Command-Center)** *(v1.0 released)* | How can leadership get one trusted view of revenue, customers, sales, product usage, and customer health? | Python · pandas · Data Modeling · Data Quality · DuckDB/SQL (V2) |
| 🔄 **[AI-Enhanced ETL Pipeline](https://github.com/shirleylandondata/ai-enhanced-etl-pipeline)** | Can structured business data be extracted automatically from free-text customer reviews? | Python · spaCy · NLP |

---

### 📊 Sales Performance Dashboard

Executive dashboards for a computer hardware and software retailer, built from **1,000,000 sales transactions** in Power BI, Tableau, and Excel.

**What I found:**
- **Software earns about twice hardware's margin** (≈24.7% vs. ≈11.7%). It's 20% of revenue but about 34% of profit.
- **Internet Security is the margin outlier** at 18%, while every other software category earns about 26%.
- **California, New York, and Texas lead profit,** and the top 10 products drive about 27% of the $43.39B in revenue.
- **Validated across tools:** Excel sub-category totals reconcile exactly to the $43.39B revenue shown in Power BI and Tableau.

➡️ [View project](https://github.com/shirleylandondata/Sales-Performance-Dashboard) · [Interactive Tableau dashboard](https://public.tableau.com/views/IN302_ShirleyGLandon_U9/CoXYZSalesPDashboard)

---

### 🧹 Customer Data Cleaning & Validation

Cleaned **500,000 customer records** using the same rules in Tableau, Power BI (Power Query), and Excel. I fixed birthdates recorded in the 1700s, future join dates, invalid gender codes, and inconsistent ZIP codes, then derived Age and tenure fields.

**Why it matters:** reconciling chart totals back to the 500,000-row source showed that about 46 records still had future join dates after the first cleaning rule. Cross-checking caught what a single tool missed, and the project documents the stronger rule and validation checks.

➡️ [View project](https://github.com/shirleylandondata/Customer-Data-Cleaning_Validation)

---

### 🔮 Customer Churn Predictive Modeling

A retail bank wants to focus retention resources on the customers most likely to leave. Using 10,000 customer records (20.4% churn rate), I compared four classification models: Logistic Regression, SVM, Decision Tree, and Random Forest.

**What I found:**
- **Accuracy alone was misleading.** Logistic Regression scored 80.5% accuracy but caught only 14.7% of customers who actually churned.
- **Random Forest gave the best balance:** 85.95% test accuracy, 0.847 ROC-AUC, and the most churners identified (168 of 407).
- **Age and number of products** drove about 57% of the model's predictive weight. Number of products showed only a weak correlation during exploration, so the relationship is likely nonlinear.

**Recommendation:** use model output as a churn risk score to prioritize outreach, not to automate decisions about customers.

➡️ [View project](https://github.com/shirleylandondata/Customer-Churn-Predictive-Modeling)

---

### 📈 Executive KPI Command Center · [v1.0 released](https://github.com/shirleylandondata/Executive-KPI-Command-Center/releases/tag/v1.0)

A fictional B2B SaaS company has its billing, sales, product, and customer success data spread across separate systems, and leadership can't answer basic questions from one trusted source. V1 builds the data foundation: business requirements, a star-schema model, a reproducible data pipeline, and validated monthly KPIs.

**V1 KPI snapshot (Jan 2024 → Jul 2026):**
- **MRR grew 44.6%,** from $3.46M to $5.01M ($60.1M ARR), on 2,677 → 3,822 active subscriptions
- **Monthly churn averaged 0.33%,** and **collection rate averaged 95.0%**
- **Every KPI ties back to source data:** monthly transactions match active subscriptions in all 31 months

**Checking my own work:** every row-level check passed, but billed revenue sat flat at $5.45M every month while subscriptions grew. Reconciling revenue against subscriptions traced the cause to a billing calendar that only ran for 3 subscriptions. After the fix, 106,112 transactions show 0 billed before start, 0 billed after cancellation, and 0 where collected exceeds billed.

**Also in V1:** a KPI dictionary with owners and decisions, a KPI-to-data mapping that flags which KPIs the data can't support yet (NRR and GRR need expansion/contraction history), and 29 documented data quality rules.

**Next (V2):** SQL KPI layer in DuckDB, executive dashboard, and written findings.

➡️ [View project](https://github.com/shirleylandondata/Executive-KPI-Command-Center) · [Data quality rules](https://github.com/shirleylandondata/Executive-KPI-Command-Center/blob/main/docs/data_quality_rules.md) · [KPI mapping](https://github.com/shirleylandondata/Executive-KPI-Command-Center/blob/main/docs/kpi_data_mapping.md)

---

### 🔄 AI-Enhanced ETL Pipeline

Traditional ETL handles structured databases well but struggles with free text. This workflow uses Python and spaCy Named Entity Recognition to pull products, dates, organizations, and people out of customer reviews and aggregate them into structured output.

➡️ [View project](https://github.com/shirleylandondata/ai-enhanced-etl-pipeline)

---

## ⚙️ Operations Reporting & Systems

### I've also built hands-on labs in IT operations. Each one includes reporting and monitoring work:

- **[ServiceNow ITSM Change Management Lab](https://github.com/shirleylandondata/ServiceNow-ITSM-Change-Management-Lab):** incident and change workflows, approvals, SLA tracking, and operational reporting
- **[Splunk Monitoring Lab](https://github.com/shirleylandondata/Azure-Splunk-Security-Monitoring-Lab):** log ingestion, SPL queries, and dashboards tracking failed logins, lockouts, and operational KPIs
- **[AI Automation Consultant](https://github.com/shirleylandondata/ai-automation-consultant):** a Python/LLM tool that runs structured, multi-turn discovery to identify workflow automation opportunities for small businesses
- Azure, Active Directory, Terraform, and network analysis labs are also in my [repositories](https://github.com/shirleylandondata?tab=repositories)

---

## 🛠️ Toolkit

**Data & Analysis:** SQL · DuckDB · Python (pandas, NumPy, scikit-learn) · Excel (PivotTables) · Power Query · Data Modeling · Data Cleaning · Data Validation · ETL
**Visualization & BI:** Power BI · Tableau · Matplotlib · Seaborn · Hex
**Business Systems:** DealCloud CRM · ServiceNow · Splunk · Microsoft 365
**Workflow:** Git/GitHub · VS Code · Jupyter / Google Colab · Draw.io

---

## 🎓 Education

- **B.S. in Analytics – Cloud Computing**, Purdue University Global (expected 2027) · GPA 3.89 · Micro-credential: Data Intelligence
- **MBA, Marketing Focus**, Keller Graduate School of Management
- **BBA, Corporate Organizational Studies**, University of Connecticut

---

## 📬 Let's Connect

💼 [LinkedIn](https://www.linkedin.com/in/shirleylandon/) · 📧 Shirleymlandon@gmail.com · 📍 Fairfield, CT (remote)

📅 **[Book an intro call with me](https://calendly.com/shirleymlandon/intro-meeting)**
