# Financial Transactions Analysis Project

**End-to-End Data Cleaning & Business Analysis**

---

## Project Overview

This project demonstrates a complete data analysis workflow:
1. **Data Cleaning** - Transforming messy, "dirty" financial data into reliable, analysis-ready format
2. **Customer & Product Analysis** - Understanding spending patterns and product performance

**Dataset**: 100,000 financial transactions with various data quality issues.

---

## Technologies Used

- Python
- Pandas
- Google Colab

---

## Project Structure
financial-transactions-analysis/
├── data/
│   ├── dirty_financial_transactions.csv
│   └── cleaned_financial_transactions.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   └── 02_customer_product_analysis.ipynb
├── README.md
└── requirements.txt


## Data Cleaning Process (`01_data_cleaning.ipynb`)

### Challenges Addressed:
- Missing values (Transaction_ID, Date, Price, Status)
- Inconsistent formatting (Payment methods, Product names, Status)
- Invalid data (negative quantities/prices, future dates)
- Duplicate and malformed Transaction IDs

### Key Cleaning Steps:
- Standardized IDs and categorical fields
- Handled negative values to derive `Transaction_Type`
- Fixed date formats and invalid entries
- Imputed missing values strategically
- Created `Total_Transaction_Value` column

**Result**: Clean, consistent dataset ready for analysis.

---

## Customer & Product Analysis (`02_customer_product_analysis.ipynb`)

### Analysis Performed:
- Calculated total transaction value per row
- Customer-level metrics (total spending, frequency)
- Product performance (revenue and quantity sold)
- Transaction status breakdown (Completed, Pending, Failed)

### Key Insights:

- **Completed Revenue**: ~$3.26 Billion
- **Pending Revenue Potential**: ~$2.19 Billion
- **Failed Transactions**: ~$1.12 Billion (lost opportunity)
- **Total Transaction Value**: ~$6.56 Billion

**Business Recommendations**:
1. Focus on converting Pending transactions
2. Investigate root causes of Failed transactions
3. Prioritize top-performing products
4. Target high-value customers for retention

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/vValeriecm/financial-transactions-analysis
