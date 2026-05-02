# hr-attrition-dashboard
HR attrition analysis and risk dashboard using Python, Power BI, and scikit-learn.

# HR Analytics: Employee Attrition Risk Dashboard

**Tools:** Python · Power BI · Excel · scikit-learn  
**Domain:** Human Resources · People Analytics  
**Role fit:** Data Analyst · Business Analyst

---

## Business problem
A mid-size technology company is experiencing 16% annual employee attrition —
above the industry average of 10-12%. HR leadership needs to understand which
departments and employee segments are most at risk, and what interventions to
prioritise.

## What I built
- **EDA notebook** — explored 1,470 employee records across 35 features
- **Attrition prediction model** — logistic regression with 78% ROC-AUC
- **Risk scoring** — assigned Low / Medium / High risk tier to all 1,470 employees
- **Power BI dashboard** — 4-page interactive report for HR leadership
- **Excel summary** — pivot dashboard for stakeholders without BI tool access
- **Recommendation memo** — 3 data-backed HR policy proposals

## Key findings
- Employees working overtime leave at **3x the rate** of those who don't (30% vs 10%)
- High-risk employees earn on average **₹8,200/month less** than low-risk peers
- Sales department has the highest attrition rate at **20.6%**
- 312 employees scored as High Risk — concentrated in Sales and R&D

- ## Project structure
hr-attrition-dashboard/
├── data/processed/       ← cleaned + scored dataset
├── notebooks/            ← EDA and model notebooks
├── excel/                ← pivot summary for stakeholders
├── powerbi/              ← .pbix dashboard file
├── reports/              ← recommendation memo (PDF)
└── screenshots/          ← dashboard previews

## Dashboard preview
![Overview page](screenshots/dashboard_overview.png)
![Risk heatmap](screenshots/risk_heatmap.png)

## Data source
IBM HR Analytics Employee Attrition & Performance dataset  
Source: Kaggle (public domain) — 1,470 rows × 35 columns  
Raw data not included in repo. Download from:  
https://kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

## How to run
1. Clone the repo
2. pip install -r requirements.txt
3. Place raw CSV in data/raw/
4. Run notebooks in order: 01_eda.ipynb → 02_model.ipynb
5. Open powerbi/HR_Attrition_Dashboard.pbix in Power BI Desktop
