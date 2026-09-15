# 📊 HR Workforce Analytics — Insights & Dashboard

A department-level analysis of workforce data (1,500 employees) covering headcount, compensation, engagement, attrition, promotion, and hiring sources — taken from raw data, through SQL-driven insights, to an interactive dashboard, to a stakeholder-ready presentation.

---

## 🖼️ Dashboard Preview

**Employee View** — team size, headcount, salary by gender, monthly income, and promotion split by department.
<img width="1335" height="746" alt="EMPLOYEE" src="https://github.com/user-attachments/assets/08ae4754-623b-4ab6-b661-c822edcf7319" />
**Company View** — income vs. tenure, satisfaction scores, work arrangement, hiring source, and attrition by department.
<img width="1331" height="745" alt="COMPANY" src="https://github.com/user-attachments/assets/524cdc7a-59c3-4bc6-a097-d44daea6dfa7" />


---

## 🔁 Project Workflow

**1. Brief Data Analysis**
Started with a quick exploratory pass over the raw HR dataset to understand structure, fields, and data quality (departments, gender, salary, tenure, satisfaction scores, attrition/promotion flags, hiring source, etc.).

**2. Insight Generation with SQL**
Wrote SQL queries to aggregate and slice the data — average salary by gender, average monthly income by department, headcount and attrition by department, promotion share, satisfaction scores, hiring source breakdown, and income trends by tenure. These queries formed the foundation for every insight in the project.

**3. Visualization of Insights**
Converted the SQL output into charts (bar, pie, scatter) to make each insight easy to read at a glance — e.g., attrition rate by department, selection type breakdown, and income vs. years at company.

**4. Dashboard Creation**
Combined the visuals into an interactive dashboard with two views (Employee and Company — see previews above).

**5. Presentation of Insights**
Packaged the key findings into a slide deck (`HR_Dashboard_Insights.pptx`) for a non-technical audience — an executive summary, one focused slide per theme (workforce overview, compensation, tenure & team structure, engagement, attrition, promotion, hiring sources), and a closing set of recommendations.

---

## 📊 Key Insights

- R&D and Sales make up 54% of headcount and also post the highest attrition (24.5% each).
- Average female salary ($65.56K) is ~6% above average male salary ($61.84K) company-wide.
- R&D's average monthly income ($98K) is 66% higher than the next department (Finance, $59K) — likely driven by R&D also being the largest department, with most employees (junior through senior) paid at this elevated rate rather than a small senior cohort skewing the mean.
- Job satisfaction, work-life balance, and environment scores cluster tightly (2.8–2.95 out of 4) across every department — engagement is flat, not failing.
- Promotion share is near-even across departments (~16–17% each), tracking headcount rather than attrition risk.
- LinkedIn, Referral, and Job Portal together source about two-thirds of all hires.

---

## 🗂️ Dataset

- **Source:** *add your dataset link/source here (e.g. Kaggle "HR Analytics Employee Attrition" dataset, or internal/synthetic data)*
- **Size:** 1,500 employee records
- **Fields:** Department, Gender, MonthlyIncome, YearsAtCompany, JobSatisfaction, WorkLifeBalance, EnvironmentSatisfaction, Attrition, PromotionStatus, WorkType (On-site/Hybrid/Remote), SelectionType (hiring source), TeamSize

> Update this section with the exact dataset name/link once finalized — reviewers usually check this first.

---

## 🛠️ Tools Used

| Stage | Tool |
|---|---|
| Data analysis & querying | SQL |
| Dashboard | Power BI *(or your actual BI tool — update if different)* |
| Presentation | PowerPoint (.pptx) |

---

## ▶️ How to View

1. **Dashboard:** Open `dashboard/HR_Dashboard.pbix` in Power BI Desktop *(or open the exported PDF/image if you're not sharing the live file)*.
2. **Presentation:** Open `presentation/HR_Dashboard_Insights.pptx` in PowerPoint, Google Slides, or Keynote.
3. **SQL:** Browse `sql/` for the queries used to generate each insight.

---

## 🚀 Future Plans

- **Exploratory Data Analysis (EDA) in Python** — revisit the raw dataset using `pandas`, `matplotlib`/`seaborn`, and `numpy` to:
  - Validate and extend the SQL-derived insights with statistical summaries and distributions.
  - Explore correlations between attrition, satisfaction, tenure, and compensation in more depth.
  - Build reusable, version-controlled analysis notebooks to complement the BI dashboard.

---

## 📁 Repository Structure

```
├── data/                # Raw / cleaned dataset
├── sql/                 # SQL queries used to generate insights
├── dashboard/           # Power BI dashboard file
├── presentation/        # HR_Dashboard_Insights.pptx
├── assets/              # Dashboard screenshots used in this README
└── README.md
```

---

## 📌 Status

✅ Data analysis → ✅ SQL insights → ✅ Visualization → ✅ Dashboard → ✅ Presentation → ⏳ Python EDA (planned)
