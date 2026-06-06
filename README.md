# 🎓 Placement Intelligence Analysis | Power BI Dashboard

> **Analyzing placement outcomes, salary drivers, and skill impact for 9,000 engineering students using Power BI and DAX — designed to surface actionable insights for academic institutions and HR/Talent teams.**


## 📌 Project Overview

This end-to-end Business Intelligence project analyzes campus placement data for **9,000 engineering students** across six branches, three college tiers, and four company types. The Power BI dashboard — titled **"Placement Intelligence Analysis"** — translates raw student profile data into strategic insights, helping institutions understand what drives placement success and salary outcomes.

The project demonstrates proficiency in **data modeling, DAX measures, KPI design, resume-category segmentation, and visual storytelling** — core skills for Data Analyst, HR Analyst, and Reporting Analyst roles.

---

## 🧩 Business Problem

Campus placement teams and academic institutions often lack visibility into:

- Which student attributes (skills, CGPA, internships) most influence placement success
- How resume quality and skill diversity affect hiring probability
- Which risk indicators signal low employability early
- What strategic interventions can improve student placement outcomes at scale

**This dashboard answers these questions using data** — enabling institutions to target interventions, counsel students proactively, and benchmark cohort performance.

---

## 📂 Dataset Overview

| Attribute | Details |
|---|---|
| **Source** | Synthetic academic placement dataset |
| **File** | `student_placement_salary_elite_v2.csv` |
| **Records** | 9,000 students |
| **Columns** | 20 features |
| **Target Variables** | `placed` (binary), `salary_lpa` (continuous) |

### Key Columns

| Column | Description |
|---|---|
| `cgpa` | Cumulative GPA (5.0–10.0) |
| `branch` | Engineering branch (CSE, IT, ECE, EEE, Mechanical, Civil) |
| `college_tier` | Institution tier (1 = Top, 2 = Mid, 3 = Lower) |
| `python_skill`, `dsa_skill`, `ml_skill`, `web_dev_skill` | Binary skill flags (1 = Yes, 0 = No) |
| `coding_score`, `aptitude_score`, `communication_score` | Continuous assessment scores |
| `internships` | Number of internships completed (0–3) |
| `projects` | Number of academic/personal projects |
| `backlogs` | Number of academic backlogs |
| `resume_score` | Resume quality score (categorized into 6 tiers) |
| `skill_score` | Composite skill diversity score (0–4) |
| `placed` | Placement status (1 = Placed, 0 = Not Placed) |
| `company_type` | MNC / Mid-size / Startup / Top Tech |
| `job_role` | Software Engineer / Data Scientist / Web Developer / Analyst |
| `salary_lpa` | Annual salary offered (Lakhs Per Annum) |

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, data modeling, DAX measures |
| **Power Query (M)** | Data transformation, resume category segmentation, cleaning |
| **DAX** | KPI calculations, conditional measures, placement rate aggregations |
| **Microsoft Excel** | Initial data exploration and validation |

---

## 📊 Dashboard Features

### Dashboard Title: *Placement Intelligence Analysis*
*"Analysis of placement drivers among technical students using Power BI and DAX"*

---

### KPI Cards (Header Row)
| Metric | Value |
|---|---|
| Placement Rate | **85.6%** |
| Average CGPA | **7.5** |
| Avg Salary (LPA) | **64.7** |
| Placement % with Internship | **90.3%** |

---

### Visual 1 — Placement Rate & Number of Internships *(Scatter Plot)*
Plots placement rate against internship count (0–3), showing a clear upward trajectory. Students with 3 internships cluster near the 97%+ placement mark.

### Visual 2 — Placement Rate & Skill Score *(Column Chart)*
Displays placement rate at each skill score level (0–4) with exact data labels:

| Skill Score | Placement Rate |
|---|---|
| 0 | 57.63% |
| 1 | 76.74% |
| 2 | 89.02% |
| 3 | 96.12% |
| 4 | 98.65% |

### Visual 3 — Placement Rate by Resume Category *(Horizontal Bar Chart)*
Six resume quality tiers with placement rates:

| Resume Category | Placement Rate |
|---|---|
| Best | 100.00% |
| Good | 98.84% |
| Medium | 95.13% |
| Alert | 89.07% |
| Alarming | 72.29% |
| Worse | 40.37% |

### Insight Panels (Built Directly in Dashboard)

**Key Insights panel** summarizes major findings from the data, including internship impact, resume quality premium, and backlog risk.

**Major Placement Drivers panel** flags: Internship Experience · Communication Skills · Resume Quality · Coding Skill Diversity

**Risk Indicators panel** flags: Academic Backlogs · Low Coding Proficiency · Limited Technical Skill Diversity · Weak Resume Quality

**Strategic Recommendations panel** suggests: Increase internship opportunities · Train in more skills · Encourage project-based learning · Conduct resume & communication workshops

---

## 📈 Key Metrics / KPIs

| KPI | Value |
|---|---|
| **Overall Placement Rate** | 85.6% |
| **Total Students Analyzed** | 9,000 |
| **Placed Students** | 7,702 |
| **Not Placed** | 1,298 |
| **Average CGPA (Cohort)** | 7.5 |
| **Average Salary (Placed)** | ₹64.7 LPA |
| **Maximum Salary** | ₹129.43 LPA |
| **Placement Rate (Students with Internships)** | 90.3% |
| **Placement Rate — Best Resume Category** | 100.00% |
| **Placement Rate — Worse Resume Category** | 40.37% |
| **Placement Rate — Skill Score 4** | 98.65% |
| **Placement Rate — Skill Score 0** | 57.63% |

---

## 🔍 Analysis Performed

### 1. Internship Impact Analysis
Examined how placement rate changes with each additional internship (0 to 3), visualized as a scatter plot showing a strong positive trend.

### 2. Skill Score vs. Placement Rate
Computed a composite skill diversity score (0–4) from four binary skill flags (Python, DSA, ML, Web Dev) and tracked placement rate at each level — from 57.63% at zero skills to 98.65% at full skill coverage.

### 3. Resume Quality Segmentation
Categorized resume scores into six tiers (Worse → Best) and analyzed placement rate per tier, revealing a 59.63 percentage point gap between the best and worst resume groups.

### 4. Placement Driver Identification
Identified top positive drivers of placement: internship experience, communication skills, resume quality, and coding skill diversity.

### 5. Risk Indicator Mapping
Flagged key negative factors: academic backlogs, low coding proficiency, limited skill diversity, and weak resume quality.

### 6. KPI Summary Design
Built executive-level KPI cards tracking placement rate, average CGPA, average salary, and placement rate among students with internship experience.

### 7. Strategic Recommendation Synthesis
Translated data findings into four institution-level recommendations embedded directly within the dashboard.

---

## 💡 Business Insights

> *All insights are strictly derived from the dataset and visible in the dashboard. No assumptions have been made.*

**📌 Skill diversity is a near-linear placement predictor.**
Placement rates rise from 57.63% (no technical skills) to 98.65% (all four skills) — a 41-point gap — confirming that breadth of technical skills, not just depth in one area, drives employability.

**📌 Internships are among the strongest placement drivers.**
Students with multiple internships achieved 25–30% higher placement success. Students with at least one internship reached a 90.3% placement rate, vs. 77% for those with none.

**📌 Resume quality has an outsized impact on placement outcomes.**
Students in the "Best" resume category achieved 100% placement; those in the "Worse" tier reached only 40.37% — a 59.63 percentage point gap, making resume quality one of the highest-leverage intervention points for institutions.

**📌 Backlogs and low coding proficiency are the top risk indicators.**
Students with poor coding scores and academic backlogs consistently showed lower employability outcomes, flagged as primary risk signals in the dashboard.

**📌 Students with knowledge of multiple programming languages showed better placement outcomes even with moderate coding scores** — suggesting that skill breadth compensates for performance gaps in any single assessment.

---

## 🧠 Skills Demonstrated

```
Data Analysis          → Exploratory and segmentation analysis on 9,000 records
DAX / Measures         → Placement rate %, KPI cards, conditional aggregations
Power Query            → Resume tier categorization, data type standardization
Data Modeling          → Clean dimension-fact relationships for cross-filter slicers
Visual Storytelling    → Multi-panel dashboard with insight, risk, and recommendation layers
Business Intelligence  → Executive summary design with decision-oriented KPI layout
HR Analytics           → Skill-gap analysis, talent risk identification, employability benchmarking
Reporting              → Clear, non-technical layout suitable for institutional stakeholders
```

---

## 📁 Repository Structure

```
student-placement-analysis-powerbi/
│
├── 📊 Placement_Analysis.pbix                      # Power BI dashboard file
├── 📄 student_placement_salary_elite_v2.csv        # Source dataset (9,000 records)
├── 📸 screenshots/
│   └── Executive_Summary.png                       # Dashboard preview (Page 1)
└── 📝 README.md
```

> 💡 **To view the dashboard:** Download `Placement_Analysis.pbix` and open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).

---

## 🚀 Project Outcome

This dashboard delivers a centralized analytical view of campus placement performance across 9,000 engineering students — giving academic institutions and placement cells a data-backed foundation to act on. By quantifying the impact of resume quality (40.37% → 100% placement across tiers), skill diversity (57.63% → 98.65% across skill score levels), and internship experience (77% → 97% across internship count), the dashboard moves institutional decision-making from intuition to evidence.

The built-in Risk Indicators and Strategic Recommendations panels translate findings directly into action — making this dashboard useful not just for analysis, but for student counselling, curriculum planning, and placement strategy.

---

## 👩‍💼 About Me

**Kajal Tiwari**
MBA (Business Analytics & HR) | Fresher Data & HR Analyst

I am a final-year MBA student specializing in Business Analytics and Human Resource Management, building a portfolio at the intersection of people data and business intelligence. My focus is on translating raw data into decisions — using SQL, Power BI, and Excel to solve real HR and business problems.

📌 **Technical Skills:** Power BI · SQL (SSMS) · Excel · DAX · Power Query · Data Visualization  
📌 **Domain Skills:** HR Analytics · Workforce Planning · Talent Analytics · Reporting · MIS


---

*This project is part of my Data & HR Analytics portfolio. All data used is synthetic and for educational/portfolio purposes only.*
