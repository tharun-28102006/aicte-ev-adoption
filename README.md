# 🚗 EV Adoption Analysis - AICTE Internship (Internship Project – Week 1 & Week 2 Submission)

## 📌 Problem Statement
As electric vehicle (EV) adoption surges, urban planners need to anticipate infrastructure needs—especially charging stations. Inadequate planning can lead to bottlenecks, impacting user satisfaction and hindering sustainability goals.

---

## 🎯 Goal
Analyze historical EV adoption data to understand:
- Overall EV growth trend over time
- Distribution of EV adoption across counties
- Comparison between BEVs (Battery Electric Vehicles) and PHEVs (Plug-in Hybrid Electric Vehicles)


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


## 🚀 Project Overview


We cover two major milestones:
- **Week 1**: Exploratory Data Analysis (EDA) and Visualization  
- **Week 2**: Time Series Forecasting for EV demand prediction

---

## 🗂️ Contents
- [`week1_&_Week2_ev_analysis.ipynb`](./week1_&_Week2_ev_analysis.ipynb) – Week1- Data cleaning, correlation, and visualization. Week2- Model training and forecasting  
- [`preprocessed_ev_data.csv`](./preprocessed_ev_data.csv) – Cleaned dataset used for training  
- [`forecasting_ev_model.pkl`](./forecasting_ev_model.pkl) – Trained forecasting model  

---

## 📊 Week 1 – EV Data Exploration and Visualization

### 📌 Objectives:
- Clean raw EV data (state-wise and monthly)
- Visualize EV adoption trends
- Identify influential factors like:
  - Fuel price
  - Charging infrastructure
  - State-level policy strength
  - Population and income

### 🔍 Key Findings:
- States with stronger EV policies and infrastructure (like Delhi and Maharashtra) show higher adoption.
- Fuel price and charging stations have a strong positive correlation with EV growth.
- Urban density and income levels also play a crucial role.

### 📉 Sample Visualization:
> *Heatmaps, line plots, and bar charts were used to reveal patterns over time and across regions.*

---

## 🔮 Week 2 – Time Series Forecasting of EV Demand

### 📌 Objective:
To forecast monthly EV demand using a pre-trained time series model.

### ⚙️ Model Highlights:
- Trained on a preprocessed dataset with factors like fuel cost, income, policy scores, and station count.
- Uses a regression-based approach for monthly forecasting.

### 🧠 Prediction Strategy:
1. Load pre-trained model from `forecasting_ev_model.pkl`
2. Use `preprocessed_ev_data.csv` for inference
3. Forecast EV demand across different months

### ✅ Output:
- A NumPy array showing forecasted demand for each entry in the test set
- Flexible to scale state-wise predictions or aggregate at national level

---

## 🧪 How to Run

Install required libraries:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn