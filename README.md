# HR Analytics — Attrition Prediction & Workforce Planning

Predictive HR Analytics using Machine Learning & Workforce Forecasting
Built as part of the Purple Merit Data Analyst Intern Program


# Project Overview
Employee attrition is one of the most costly and overlooked problems in organizations. This end-to-end HR analytics project uses the IBM HR Analytics Dataset (1,470 employees, 35 features) to:

Predict which employees are at risk of leaving
Quantify the financial cost of attrition
Forecast 12-month workforce headcount by department
Deliver an interactive Power BI dashboard for HR decision-makers


# Key Results
MetricValueTotal Employees Analysed1,470High-Risk Employees Identified227Average Attrition Risk37.07%Estimated Annual Attrition Cost$43.02MBest Model (XGBoost) Accuracy86%Best Model ROC-AUC0.76
# Highest Risk Segments
DepartmentJob RoleAttrition ProbabilitySalesSales Representative80.72%R&DResearch Scientist53.08%R&DLaboratory Technician43.63%Human ResourcesHuman Resources42.31%SalesSales Executive37.42%

# Repository Structure
HR-Attrition-Analytics/
│
├── data/
│   └── IBM_HR_Attrition.csv          # Source dataset (from Kaggle)
│
├── notebooks/
│   ├── 01_EDA_Feature_Engineering.ipynb   # Day 1: EDA & feature creation
│   ├── 02_Model_Training_SHAP.ipynb       # Day 2: ML models & SHAP analysis
│   └── 03_Workforce_Planning.ipynb        # Day 3: Headcount forecast & scoring
│
├── dashboard/
│   ├── HR_Attrition_Dashboard.pbix        # Power BI dashboard file
│   └── dashboard_screenshot.png           # Dashboard preview
│
├── report/
│   └── Executive_HR_Report.pdf            # Final HR report with recommendations
│
├── models/
│   └── best_model_xgboost.pkl             # Saved best-performing model
│
└── README.md

# Top Attrition Drivers (SHAP Analysis)
RankFeatureImportance1Number of Companies Worked0.222Environment Satisfaction0.213Years Since Last Promotion0.214OverTime0.185Stock Option Level0.186Job Satisfaction0.187Marital Status0.168Job Involvement0.139Years With Current Manager0.12

# Dashboard Preview
<img width="1459" height="810" alt="Screenshot 2026-05-29 112008" src="https://github.com/user-attachments/assets/928f2c44-5421-4198-adbb-a1bad2c89c58" />

# Key Recommendations

Immediate intervention for Sales Representatives — 80.72% attrition risk; review compensation and workload
Address overtime culture — OverTime is a top SHAP driver; enforce work-life balance policies
Promote internal growth — Years Since Last Promotion is a critical signal; accelerate promotion cycles
Improve environment satisfaction — especially in R&D where Lab Technicians show 43% risk
Hire proactively — headcount projected to drop from 1,450 to 1,245 in 12 months without intervention

