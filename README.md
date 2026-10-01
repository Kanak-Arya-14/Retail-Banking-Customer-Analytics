# Retail Banking Customer Analytics & Subscription Propensity

An end-to-end retail banking analytics project using **Excel, Python, Machine Learning, and Power BI** to analyze customer behavior and predict the likelihood of customers subscribing to a bank term deposit.

## 📌 Project Overview

This project analyzes customer and marketing campaign data to:

- Understand customer subscription patterns
- Identify customer segments with higher subscription rates
- Perform exploratory analysis using Excel
- Build machine learning models for subscription propensity
- Generate propensity scores for individual customers
- Segment customers into Low, Medium, and High propensity groups
- Create an interactive Power BI dashboard

### End-to-End Workflow

**Raw Data → Data Cleaning → Exploratory Analysis → Machine Learning → Propensity Scoring → Power BI Dashboard**

---

## 🎯 Business Problem

Banks conduct marketing campaigns to promote financial products such as term deposits.

The objective of this project is to understand:

- Which customer groups have higher subscription rates?
- How does subscription behavior vary by age, occupation, education, and marital status?
- Can machine learning estimate a customer's likelihood of subscribing?
- How can customers be segmented based on their predicted propensity?

---

## 🗂️ Dataset

The project uses the **Bank Marketing dataset** containing customer information and marketing campaign details.

- **45,211 customers**
- **17 original features**
- Target variable: `y`
  - `yes` → Customer subscribed
  - `no` → Customer did not subscribe

The `duration` feature was excluded from predictive modeling because it contains information from the customer contact itself and could introduce **data leakage** when making a pre-contact prediction.

---

## 🛠️ Technologies Used

### Data Analysis
- Python
- Pandas
- NumPy
- Jupyter Notebook
- Microsoft Excel

### Machine Learning
- Scikit-learn
- Logistic Regression
- Random Forest
- StandardScaler
- OneHotEncoder
- ColumnTransformer
- Pipeline

### Visualization & Business Intelligence
- Power BI
- Matplotlib

### Version Control
- Git
- GitHub

---

## 📁 Project Structure

```text
Retail-Banking-Customer-Analytics/
│
├── data/
│   ├── raw/
│   │   └── bank-full.csv
│   │
│   └── processed/
│       ├── bank_analysis.xlsx
│       └── customer_propensity_scores.csv
│
├── notebooks/
│   ├── 01_data_cleaning_and_eda.ipynb
│   └── 02_customer_propensity_model.ipynb
│
├── reports/
│   └── customer_analytics.pbix
│
├── sql/
├── src/
│
├── README.md
├── requirements.txt
└── .gitignore