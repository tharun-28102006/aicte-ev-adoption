# 🚗 EV Adoption Analysis - AICTE Internship (Week 1)

## 📌 Problem Statement
As electric vehicle (EV) adoption surges, urban planners need to anticipate infrastructure needs—especially charging stations. Inadequate planning can lead to bottlenecks, impacting user satisfaction and hindering sustainability goals.

---

## 🎯 Goal
Analyze historical EV adoption data to understand:
- Overall EV growth trend over time
- Distribution of EV adoption across counties
- Comparison between BEVs (Battery Electric Vehicles) and PHEVs (Plug-in Hybrid Electric Vehicles)

This forms the foundation for **Week 2 forecasting models**.

---

## 📂 Dataset Information
- **Source:** Washington State Department of Licensing
- **Duration:** 2017-01-31 to 2024-02-29
- **Key Columns:**
  - `Date` – Month-end registration counts
  - `County` – County where the vehicle is registered
  - `Battery Electric Vehicles (BEVs)`
  - `Plug-In Hybrid Electric Vehicles (PHEVs)`
  - `Electric Vehicle (EV) Total`
  - `Total Vehicles`
  - `Percent Electric Vehicles`

---

## ✅ Week 1 Deliverables
- Jupyter Notebook: `Week1_EV_Adoption_Analysis.ipynb`
- Key tasks completed:
  - Data Loading and Cleaning
  - Missing value analysis
  - Convert `Date` column to datetime
  - **Visualizations:**
    - EV Adoption Trend Over Time
    - Top 10 Counties by EV Count
    - BEVs vs PHEVs Trend

---

## 📊 Sample Visualizations
- Line graph of EV growth trend
- Bar chart of top counties by EV count
- Line graph comparing BEVs vs PHEVs

---

## 🔮 Future Scope
- **Week 2:** Growth Rate Analysis (CAGR) & Feature Engineering
- **Week 3:** Forecasting Models (Linear Regression, XGBoost)
- **Week 4:** Model Evaluation and Deployment

---

### ▶ How to Run
1. Clone the repository or download files.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
