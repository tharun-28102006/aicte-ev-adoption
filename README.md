# ⚡ Electric Vehicle (EV) Demand Forecasting using Machine Learning

## 🚀 Project Overview

This project focuses on building a machine learning-based forecasting system to predict the **state-wise monthly electric vehicle (EV) demand in India**. With the increasing importance of sustainable transportation, predicting future EV demand can help policymakers, manufacturers, and infrastructure developers make data-driven decisions.

The project uses **regression-based machine learning models** trained on real-world features like fuel prices, government EV policies, number of charging stations, per capita income, population, and estimated energy demand.

---

## 🎯 Learning Objectives

- To apply machine learning algorithms for real-world forecasting problems.
- To understand the influence of socio-economic and infrastructural factors on EV adoption.
- To practice data preprocessing, feature engineering, and model evaluation.
- To develop a user-friendly web interface using **Streamlit** for EV demand prediction.

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

## 🧰 Tools and Technologies Used

| Category               | Tools / Libraries                               |
|------------------------|--------------------------------------------------|
| Programming Language   | Python                                           |
| Data Manipulation      | Pandas, NumPy                                    |
| Data Visualization     | Matplotlib, Seaborn                              |
| Machine Learning       | Scikit-learn, XGBoost                            |
| Forecasting Models     | Linear Regression, Random Forest, XGBoost        |
| Web Application        | Streamlit                                        |
| Deployment (optional)  | Streamlit Cloud / Localhost                      |

---

## 🔎 Problem Statement

As electric vehicles gain traction in India, **predicting their adoption rate** becomes crucial for urban planning, infrastructure development, and energy management. However, forecasting EV demand is challenging due to the involvement of multiple dynamic factors like fuel prices, government policies, and income levels.

---

## 💡 Solution

The project proposes a **regression-based predictive model** trained on historical EV registration data enriched with external features. The key steps include:

- Data cleaning and preprocessing.
- Feature selection based on correlation with target.
- Model training using different regression algorithms.
- Performance evaluation using RMSE, R² score.
- Future EV demand forecasting (2025–2027).
- Simple interactive frontend using Streamlit for real-time predictions.

---

## 📈 Methodology

1. **Data Collection**  
   - Historical EV registration data (state/county-wise)
   - External features: Fuel Price, Policy Strength, Charging Stations, Income, Population, Energy Demand

2. **Preprocessing**  
   - Handling missing values  
   - Date conversion and time-based grouping  
   - Outlier removal and normalization  

3. **Feature Engineering**  
   - Correlation analysis  
   - Feature importance (Random Forest)  
   - Selection of most influential features  

4. **Model Building**  
   - Tried models: Linear Regression, Decision Tree, Random Forest, XGBoost  
   - Chosen model: **XGBoost** (best performance in accuracy and generalization)  

5. **Forecasting Future Demand**  
   - Used trained model to predict demand for next 3 years (2025–2027)  
   - Scenario-based predictions (e.g., increasing fuel price, better policies)

6. **Web App Interface**  
   - Built with Streamlit  
   - Allows manual input of feature values and gives real-time EV demand predictions

---

## 🧪 Results

- **Best Model**: XGBoost Regressor  
- **Performance Metrics**:  
  - RMSE: *Low error values observed*  
  - R² Score: *>90% on test data*  

- **Insights**:
  - **Fuel Prices** and **Policy Strength** are major drivers of EV demand.
  - States with more charging stations show higher EV adoption rates.

---

## 💻 How to Run the Project Locally

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/ev-demand-forecasting.git
cd ev-demand-forecasting
