# Monitoring & Evaluation Project — DHQ Hospitals

## Revamping of Non-Teaching DHQ Hospitals in Khyber Pakhtunkhwa

An end-to-end **Monitoring & Evaluation (M&E) and Data Analysis project** focused on analyzing the progress, achievement, budget utilization, and activity status of non-teaching District Headquarters (DHQ) hospitals across Khyber Pakhtunkhwa.

The project uses **SQL, Python, and Microsoft Excel** to transform raw activity-level data into meaningful analysis and decision-ready reporting.

---

## 📌 Project Overview

This project analyzes data related to the revamping of **32 DHQ hospitals across Khyber Pakhtunkhwa**.

The analysis focuses on:

* Physical target vs. achievement
* Budget allocation and utilization
* District-wise performance
* Category-wise performance
* Quarterly progress
* Activity status and delays
* Data quality and consistency
* Relationship between budget utilization and achievement

### Project Scope

| Metric                |              Value |
| --------------------- | -----------------: |
| Districts             |                 32 |
| DHQ Hospitals         |                 32 |
| Activity Records      |                885 |
| Investment Categories |                  4 |
| Quarters              |                  8 |
| Data Fields           |                14+ |
| Tools Used            | SQL, Python, Excel |

---

## 🎯 Project Objectives

1. Monitor physical progress against planned targets.
2. Analyze financial performance through budget utilization.
3. Identify delayed activities and areas requiring follow-up.
4. Compare performance across districts and investment categories.
5. Validate and clean the project dataset.
6. Develop an accessible dashboard for M&E reporting and decision-making.

---

## 🛠️ Tools & Technologies

* **MySQL** — Database creation, data import, cleaning, validation, and analytical queries
* **Python / Pandas** — Exploratory data analysis and statistical analysis
* **Microsoft Excel** — Pivot-based summaries, dashboard, and reporting
* **Matplotlib** — Data visualization

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
SQL — Data Import & Cleaning
     ↓
Data Quality Validation
     ↓
Python — Exploratory & Statistical Analysis
     ↓
Excel — Dashboard & Reporting
     ↓
Key Findings & Recommendations
```

---

# 1. SQL — Data Collection & Cleaning

The SQL stage focused on creating the database, importing the raw dataset, cleaning the data, and performing quality checks.

### Key Activities

* Created MySQL database: `dhq_hospital_project`
* Created and populated the `raw_data` table
* Imported **885 activity records**
* Cleaned percentage values containing `%` signs
* Removed comma separators from financial values
* Converted cleaned fields to appropriate numeric data types
* Checked missing values
* Checked duplicate Activity IDs
* Performed range and consistency checks
* Generated district, category, quarter, and agency-level summaries

### Data Quality Results

* **885 / 885** records had no missing values
* **0** duplicate Activity IDs detected
* **93** records had Budget Utilized greater than Budget Allocated
* **160** records had Achievement greater than Target
* **37** activities were flagged as delayed

The logical-check records were retained for further analysis rather than automatically deleted.

### SQL File

`dhq_hospital_project_queries.sql`

This file contains the database setup, cleaning queries, validation checks, and analytical queries used in the project.

---

# 2. Python — Exploratory & Statistical Analysis

The cleaned dataset was analyzed using Python and Pandas to explore performance patterns and relationships within the data.

### Analysis Performed

* Dataset structure and data-type inspection
* Descriptive statistics
* Missing-value validation
* Duplicate checking
* District-wise achievement analysis
* Category-wise analysis
* Quarterly trend analysis
* Budget allocation vs. utilization analysis
* Activity status analysis
* District-wise budget utilization
* Correlation analysis

### Key Statistical Finding

The Pearson correlation between **Budget Utilized** and **Achievement** was approximately:

**-0.44**

This indicates a weak negative relationship within this dataset and suggests that higher spending alone did not necessarily correspond to higher achievement.

---

# 3. Excel — Dashboard & Reporting

The Excel stage converted the analyzed data into a decision-ready reporting dashboard.

The dashboard includes:

* Overall achievement KPI
* Budget utilization KPI
* District summary
* Category summary
* Quarterly progress
* Hospital-level summary
* Activity status
* Implementing agency analysis
* Budget allocation and utilization charts

---

# 📊 Key Findings

### Overall Performance

* **83.5%** overall achievement against target
* **76.9%** overall budget utilization
* **885** activities analyzed

### District Performance

The analysis identified variation in achievement across the 32 districts.

* Highest reported average achievement: **Shangla — 92.4%**
* Lowest reported average achievement: **Kohat — 78.0%**

### Category Performance

| Category                 | Achievement | Budget Used |
| ------------------------ | ----------: | ----------: |
| Medicines & Disposables  |       86.1% |       77.4% |
| Medical Equipment        |       84.7% |       75.7% |
| Furniture & IT           |       84.5% |       78.3% |
| Renovation & Civil Works |       69.8% |       77.3% |

Renovation & Civil Works represented the largest budget share while recording the lowest achievement rate among the four categories.

### Delayed Activities

**37 out of 885 activities (4.2%)** were flagged as delayed.

The delays were distributed across multiple districts rather than being concentrated in a single district.

---

# 👤 Team & Contributions

### Muhammad Abrar — SQL & Data Collection

* Database setup
* Data import
* SQL data cleaning
* Data validation
* Quality checks
* Analytical SQL queries
* District/category/quarter-level summaries

### Shayan Khan — Python Analysis

* Exploratory data analysis
* Statistical analysis
* Correlation analysis
* Data visualization
* Python-based validation

### Saad & Farhan — Excel Dashboard

* Pivot-based summaries
* Dashboard development
* KPI reporting
* Charts and reporting views

---

# 📁 Repository Contents

```text
DHQ-Hospitals-ME-Project/
│
├── README.md
│
├── dhq_hospital_project_queries.sql
│
└── DHQ_Hospitals_ME_Presentation_FINAL.pptx
```

---

# 💡 Recommendations

Based on the analysis, the project recommends:

* Increased M&E follow-up for **Renovation & Civil Works**
* Early review of districts with lower achievement levels
* Standardized formatting of source datasets before future imports
* Monitoring budget utilization and physical achievement together
* Continued validation of activities where achievement exceeds targets or expenditure exceeds allocation

---

## 📚 Skills Demonstrated

**Monitoring & Evaluation**

* Data Collection
* Data Cleaning
* Data Validation
* Performance Monitoring
* Progress Reporting
* KPI Analysis
* Means of Verification concepts

**Data Analytics**

* SQL
* MySQL
* Python
* Pandas
* Data Visualization
* Statistical Analysis
* Correlation Analysis
* Excel
* Pivot Tables
* Dashboard Development

---

## 📌 Project Type

**Data Analyst Course Project | Monitoring & Evaluation | Healthcare Infrastructure | SQL + Python + Excel**

*Dataset and project scenario are based on a real KP healthcare infrastructure initiative and are used here for educational and analytical purposes.*
