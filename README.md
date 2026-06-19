# 📊 Customer Behaviour — Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

This project performs a complete **Exploratory Data Analysis (EDA)** on a Customer Behaviour dataset.  
The goal is to understand customer patterns, identify key trends, and extract actionable insights around **Order Value, Return Behaviour, and Customer Satisfaction**.

---

## 📂 Dataset — `stats_data.csv`

| Column | Type | Description |
|---|---|---|
| Customer_ID | Categorical | Unique customer identifier |
| Age | Numerical | Customer age |
| Gender | Categorical | Male / Female |
| Region | Categorical | North / South / East / West |
| Segment | Categorical | Consumer / Corporate / Small Business |
| Monthly_Orders | Numerical | Number of orders per month |
| Order_Value | Numerical | Order value in Rs. |
| Return_Flag | Binary | 1 = Returned, 0 = Not Returned |
| Customer_Tenure | Numerical | Years as customer |
| Support_Calls | Numerical | Number of support calls made |
| Payment_Method | Categorical | UPI / Credit Card / Debit Card |
| Satisfaction_Score | Numerical | Score out of 5 |

- **Rows:** 15  
- **Columns:** 12  
- **Missing Values:** None

---

## 🔍 Key Insights

- 📦 **Corporate Segment** has the highest avg order value — **Rs. 4,720**
- 🔄 **Return Rate** is **33%** — all returners are from Corporate segment
- 📞 **More Support Calls = Lower Satisfaction** (r = -0.82)
- 💳 **Credit Card users** have higher order values and return rates
- 📈 **Monthly Orders & Order Value** are strongly correlated (r = 0.97)

---

## 📊 Analysis Performed

### 1. Univariate Analysis — Order Value
- Distribution (Histogram + KDE)
- Box Plot (Outlier Detection)
- Percentile Analysis (P0 to P100)
- Skewness & Kurtosis

### 2. Bivariate Analysis
- Order Value by Segment, Region, Gender
- Order Value by Return Flag
- Order Value by Payment Method
- Scatter Plots (Order Value vs Age, Monthly Orders, Support Calls)

### 3. Multivariate Analysis
- Correlation Heatmap (All Numerical Columns)
- Support Calls vs Satisfaction (colored by Return Flag)

---

## 🛠️ Tech Stack

| Tool | Version |
|---|---|
| Python | 3.12 |
| Pandas | 2.0+ |
| NumPy | 1.26+ |
| Matplotlib | 3.8+ |
| Seaborn | 0.13+ |

---

## 🚀 How to Run

```bash
# Step 1: Clone the repo
git clone https://github.com/Tushar-DataAnalyst/stats-eda-project.git

# Step 2: Go to folder
cd stats-eda-project

# Step 3: Create virtual environment
python -m venv statsenv

# Step 4: Activate virtual environment
statsenv\Scripts\activate

# Step 5: Install libraries
pip install pandas numpy matplotlib seaborn openpyxl

# Step 6: Launch Jupyter
jupyter notebook
```

---

## 📁 Project Structure

```
stats-eda-project/
│
├── 📄 stats_data.csv        ← Dataset
├── 📄 Sales .ipynb          ← EDA Notebook
├── 📄 .gitignore            ← Git ignore file
└── 📄 README.md             ← Project documentation
```

---

## 👤 Author

**Tushar**  
Senior Data Analyst | Power BI Developer  
📍 Gurugram, India  
🔗 [GitHub](https://github.com/Tushar-DataAnalyst)

---

## 📜 License

This project is open source and available for educational purposes.
