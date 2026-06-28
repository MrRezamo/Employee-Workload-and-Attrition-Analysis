# 👔 Employee Performance, Workload & Attrition Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?logo=kaggle)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

A complete HR analytics project that explores employee attrition patterns,
workload distribution, and performance behavior using **Exploratory Data
Analysis (EDA)**, **Machine Learning classification models**, and an
**interactive Plotly dashboard**.

---

## 📁 Project Structure
```
EMPLOYEE-WORKLOAD-ATTRITION/
│
├── data/
│ └── employee_performance_workload_attrition.csv
│
├── images/
│ └── (charts exported from notebooks)
│
├── models/
│ └── (trained model files saved as .joblib)
│
├── notebooks/
│ ├── EDA.ipynb # Exploratory Data Analysis
│ ├── modeling.ipynb # ML Model Training & Evaluation
│ └── dashboard.ipynb # Interactive Plotly Dashboard
│
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```
---

## 📊 Dataset Overview

> 📌 Source: [Kaggle – Employee Workload and Attrition Analysis](https://www.kaggle.com/)

| Feature              | Type        | Description                                            |
| -------------------- | ----------- | ------------------------------------------------------ |
| `employee_id`        | int         | Unique employee identifier                             |
| `department`         | categorical | HR, Engineering, Finance, Sales, Marketing, Operations |
| `role_level`         | categorical | Junior, Mid, Senior                                    |
| `monthly_salary`     | int         | Monthly salary                                         |
| `avg_weekly_hours`   | int         | Average weekly working hours                           |
| `projects_handled`   | int         | Number of projects managed                             |
| `performance_rating` | int (1–5)   | Employee performance score                             |
| `absences_days`      | int         | Number of absence days                                 |
| `job_satisfaction`   | int (1–5)   | Job satisfaction score                                 |
| `attrition`          | binary      | Whether the employee left: Yes / No                    |

- **Total Records:** 2,800 &nbsp;|&nbsp; **Format:** CSV &nbsp;|&nbsp; **Type:** Synthetic & anonymized

---

## 🔍 Notebook 1 — EDA (`EDA.ipynb`)

- Data overview: shape, dtypes, missing values
- Target variable distribution (Attrition: Yes vs No)
- Univariate & bivariate analysis
- Correlation heatmap
- Department & role-level breakdowns
- Key business insights & observations

---

## 🤖 Notebook 2 — ML Modeling (`modeling.ipynb`)

- Feature engineering & encoding
- Train/test split with stratification
- Baseline: Logistic Regression
- Advanced models: Random Forest, XGBoost
- Evaluation: Accuracy, Precision, Recall, F1, ROC-AUC
- Confusion matrix & feature importance plots
- Model export with `joblib` → saved to `models/`

---

## 📈 Notebook 3 — Dashboard (`dashboard.ipynb`)

- Interactive charts built with **Plotly**
- Attrition breakdown by department, role, and salary band
- Workload vs performance scatter plots
- Satisfaction vs attrition trend analysis
- Filters and dropdowns for dynamic exploration

---

## 💡 Key Business Questions

1. Which departments have the highest attrition rate?
2. Does overworking correlate with leaving the company?
3. What is the relationship between salary and job satisfaction?
4. Which features are the strongest predictors of attrition?
5. Can we reliably predict which employee is likely to leave?

---

## 🛠️ Tech Stack

| Library                  | Purpose                      |
| ------------------------ | ---------------------------- |
| `pandas`                 | Data manipulation            |
| `numpy`                  | Numerical operations         |
| `matplotlib` / `seaborn` | Static visualizations        |
| `plotly`                 | Interactive dashboard        |
| `scikit-learn`           | ML modeling & evaluation     |
| `xgboost`                | Gradient boosting classifier |
| `joblib`                 | Model persistence            |

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/your-username/employee-workload-attrition.git
cd employee-workload-attrition

# 2. Create and activate virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter
jupyter notebook
```

---

## 📸 Visuals

> _(Charts will be added here after EDA and Dashboard notebooks are complete)_

<!-- Example (uncomment after adding images):
![Attrition Distribution](images/attrition_distribution.png)
![Correlation Heatmap](images/correlation_heatmap.png)
![Dashboard Overview](images/dashboard_overview.png)
-->

---

## 📌 Project Status

- [x] Repository setup & folder structure
- [x] Dataset added
- [ ] EDA notebook complete
- [ ] Modeling notebook complete
- [ ] Dashboard notebook complete
- [ ] Visuals added to README

---

## 👤 Author

**Reza Sharifi**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://linkedin.com/in/reza.sharifii)
[![GitHub](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/MeRezamo)

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
