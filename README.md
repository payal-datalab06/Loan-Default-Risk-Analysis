# 📊 Loan Default Risk Analysis | Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![DAX](https://img.shields.io/badge/Analysis-DAX-blue)
![Project](https://img.shields.io/badge/Project-Data%20Analytics-green)

## 📌 Project Overview

This project focuses on analysing loan portfolio data to identify patterns and factors associated with loan defaults.

Using **Microsoft Power BI**, I developed an interactive dashboard to explore borrower characteristics, financial indicators, and loan default trends.

The objective is to turn raw loan data into meaningful insights that can support better understanding of lending risk.

## 🎯 Business Objectives

- Analyse overall loan portfolio performance.
- Calculate the loan default rate.
- Identify borrower segments with higher default rates.
- Understand the relationship between financial indicators and loan defaults.
- Present insights through interactive visualisations.

## 🛠️ Tools & Technologies

- **Microsoft Power BI** – Dashboard development and visualisation.
- **Power Query** – Data cleaning and transformation.
- **DAX** – Measures and calculations.
- **Microsoft Excel / CSV** – Dataset preparation.

## 📂 Dataset Overview

- Total records: 255,347
- Total original columns: 18
- Missing values: 0
- Duplicate records: 0
- Duplicate Loan IDs: 0

### Data Preparation

- Standardised column names.
- Removed unnecessary spaces from text fields.
- Checked missing values and duplicate records.
- Maintained loan IDs as text.
- Created a readable default status column.
- Created additional categories for analysis.

**Note:** No records were removed during data cleaning.

## 📊 Dashboard Pages

### 1. Loan Portfolio Overview

- Total Loans
- Defaulted Loans
- Default Rate
- Default vs. Non-Default Distribution
- Default Rate by Loan Purpose
- Default Rate by Credit Score Category

### 2. Borrower Risk Analysis

- Default Rate by Employment Type
- Default Rate by Education Level
- Default Rate by Age Group
- Default Rate by Marital Status
- Default Rate by Dependent Status

### 3. Financial Risk Analysis

- Default Rate by Loan Amount Group
- Default Rate by DTI Group
- Default Rate by Income Group
- Defaulted Loans by Co-signer Status

## 📈 Key Performance Indicators

| KPI | Value |
|---|---:|
| Total Loans | 255,347 |
| Defaulted Loans | 29,652 |
| Non-Defaulted Loans | 225,695 |
| Default Rate | 11.61% |

*Please verify these figures against the final Power BI dashboard before publishing.*

## 🔍 Key Insights

- Higher loan amount categories show higher default rates in the analysed dataset.
- Unemployed borrowers show a higher default rate than the other employment categories displayed.
- The 18–25 age group shows a higher default rate than the other age groups displayed.
- Default rates vary across loan purposes and credit score categories.
- Financial indicators such as income, loan amount, and DTI provide additional dimensions for exploring default patterns.

## 🧮 DAX Measures

Examples of the measures used in the dashboard:

**Total Loans**
```dax
Total Loans = COUNTROWS(LoanData)
```

**Defaulted Loans**
```dax
Defaulted Loans =
CALCULATE(
    [Total Loans],
    LoanData[default] = 1
)
```

**Default Rate**
```dax
Default Rate =
DIVIDE(
    [Defaulted Loans],
    [Total Loans],
    0
)
```

*Replace `LoanData` with the actual table name in your Power BI model.*

## 💡 Skills Demonstrated

- Data Cleaning and Transformation
- Data Modelling
- DAX Calculations
- KPI Development
- Data Visualisation
- Business Intelligence
- Analytical Thinking
- Dashboard Design
- Insight Generation

## 📁 Project Structure

```text
Loan-Default-Risk-Analysis/
│
├── Dashboard/
│   └── Loan_Default_Risk_Dashboard.pbix
│
├── Dataset/
│   └── Dataset information and source
│
├── Screenshots/
│   ├── Loan_Portfolio_Overview.png
│   ├── Borrower_Risk_Analysis.png
│   └── Financial_Risk_Analysis.png
│
└── README.md
```

## 🚀 Project Outcome

Developed a three-page interactive Power BI dashboard to explore loan default patterns across borrower demographics, loan characteristics, and financial indicators.

This project strengthened my practical understanding of data analysis, DAX, Power Query, and business intelligence dashboard development.

## ⚠️ Disclaimer

- This is an educational portfolio project.
- The analysis identifies patterns and associations, not causal relationships.
- The dashboard is not a validated credit-scoring or lending decision model.
- Dataset units and currency are not fully documented; therefore, no currency assumptions have been made.

## 👩‍💻 About Me

I am a B.Com graduate interested in Data Analytics and Business Intelligence.

Currently developing my skills in:

- Excel
- SQL
- Python
- Power BI

I enjoy working with data, discovering patterns, and presenting insights through meaningful visualisations.

## 🤝 Connect With Me

- 📧 **Email:** [payal.patil.work@gmail.com](mailto:payal.patil.work@gmail.com)
- 🔗 **LinkedIn:** [Connect with me on LinkedIn](https://www.linkedin.com/in/payalpatildataanalytics/)
- 🐙 **GitHub:** [@payal-datalab06](https://github.com/payal-datalab06)


## 🏷️ Project Tags

#PowerBI #DataAnalytics #BusinessIntelligence #DataVisualization #DAX #PowerQuery #DashboardDevelopment #FinancialAnalytics #LoanDefaultAnalysis #DataCleaning #DataStorytelling #PortfolioProject #LearningByDoing
