# Hi, I'm Shirley Landon 👋

## Data & Operations Analyst | SQL · Python · Power BI · Excel

I turn messy business data into clear answers that people can act on.

I spent 15 years inside the operations that analysts report on: supporting investment teams, executives, and legal practices at The Carlyle Group, Goldman Sachs, Barclays, Viking Global Investors, and Kirkland & Ellis. I've maintained the CRM records, reconciled the expenses, tracked the pipelines, and produced the reports. I know where business data breaks, because I've worked downstream of it.

Now I build the analysis myself: defining the business question, validating the data, modeling it, and explaining what it means for the decision.

**Open to remote roles:** Data Analyst · Business Data Analyst · Operations Analyst · Reporting Analyst · Data Quality Analyst · Business Intelligence (BI) Analyst

📅 [Book an intro call](https://calendly.com/shirleymlandon/intro-meeting) · 💼 [LinkedIn](https://www.linkedin.com/in/shirleylandon/)

---

## 📊 Featured Analytics Projects

| Project | Business question | Tools |
|---|---|---|
| 🔮 **[Customer Churn Predictive Modeling](https://github.com/shirleylandondata/Customer-Churn-Predictive-Modeling)** | Which retail-banking customers are most likely to leave, and where should retention effort go? | Python · pandas · scikit-learn · Matplotlib · Seaborn |
| 📈 **[Executive KPI Command Center](https://github.com/shirleylandondata/Executive-KPI-Command-Center)** *(in progress)* | How can leadership get one trusted view of revenue, customers, sales, and support? | Python · DuckDB/SQL · Data Modeling · Power BI |
| 💳 **[Payment Funnel Analysis — FinTech](https://github.com/shirleylandondata/payment-funnel-analysis-fintech)** | Where do payments drop off, and which methods fail most often? | SQL · DuckDB · Hex |
| 🔄 **[AI-Enhanced ETL Pipeline](https://github.com/shirleylandondata/ai-enhanced-etl-pipeline)** | Can structured business data be extracted automatically from free-text customer reviews? | Python · spaCy · NLP |

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

### 📈 Executive KPI Command Center *(in progress)*

A fictional B2B SaaS company has customer, billing, sales, product, marketing, and support data spread across separate systems. Leadership can't answer basic questions from one trusted source.

**Completed so far:**
- Translated executive questions into KPI definitions across revenue, customers, sales, product, marketing, support, and customer success
- Designed a star-schema dimensional model spanning 7 business processes, with a field dictionary and ERD
- Built a seeded, reproducible Python data generator
- Ran data-quality checks on generated data: uniqueness, referential integrity, date logic, and non-negative revenue across **128,977 revenue transactions**, with zero duplicate or missing customer IDs

**Next:** SQL warehouse build in DuckDB, KPI layer, executive dashboard, and written findings.

➡️ [View project](https://github.com/shirleylandondata/Executive-KPI-Command-Center)

---

### 💳 Payment Funnel Analysis — FinTech

Analyzed a 5,000-order simulated payments dataset in SQL/DuckDB to measure conversion at each payment stage, step-to-step conversion, and where transactions drop off, including the effect of fraud and authentication checks.

➡️ [View project](https://github.com/shirleylandondata/payment-funnel-analysis-fintech)

---

### 🔄 AI-Enhanced ETL Pipeline

Traditional ETL handles structured databases well but struggles with free text. This workflow uses Python and spaCy Named Entity Recognition to pull products, dates, organizations, and people out of customer reviews and aggregate them into structured output.

➡️ [View project](https://github.com/shirleylandondata/ai-enhanced-etl-pipeline)

---

## ⚙️ Operations Reporting & Systems

I've also built hands-on labs in IT operations. Each one includes reporting and monitoring work:

- **[ServiceNow ITSM Change Management Lab](https://github.com/shirleylandondata/ServiceNow-ITSM-Change-Management-Lab):** incident and change workflows, approvals, SLA tracking, and operational reporting
- **[Splunk Monitoring Lab](https://github.com/shirleylandondata/Azure-Splunk-Security-Monitoring-Lab):** log ingestion, SPL queries, and dashboards tracking failed logins, lockouts, and operational KPIs
- **[AI Automation Consultant](https://github.com/shirleylandondata/ai-automation-consultant):** a Python/LLM tool that runs structured, multi-turn discovery to identify workflow automation opportunities for small businesses
- Azure, Active Directory, Terraform, and network analysis labs are also in my [repositories](https://github.com/shirleylandondata?tab=repositories)

---

## 🛠️ Toolkit

**Data & Analysis:** SQL · DuckDB · Python (pandas, NumPy, scikit-learn) · Excel · Data Modeling · Data Validation · ETL
**Visualization & BI:** Power BI · Tableau · Matplotlib · Seaborn · Hex
**Business Systems:** DealCloud CRM · ServiceNow · Splunk · Microsoft 365
**Workflow:** Git/GitHub · VS Code · Jupyter / Google Colab · Draw.io

---

## 🎓 Education

- **B.S. Data Analytics & Cloud Computing**, Purdue University Global (expected June 2027) · GPA 3.89
- **MBA, Marketing Focus**, Keller Graduate School of Management
- **BBA, Corporate Organizational Studies**, University of Connecticut

---

## 📬 Let's Connect

💼 [LinkedIn](https://www.linkedin.com/in/shirleylandon/) · 📧 Shirleymlandon@gmail.com · 📍 Fairfield, CT (remote)

📅 **[Book an intro call with me](https://calendly.com/shirleymlandon/intro-meeting)**
