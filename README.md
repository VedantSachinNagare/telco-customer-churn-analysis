# telco-customer-churn-analysis
Python EDA of 7,043 telecom customers: month-to-month contracts churn 15x more than 2-year plans, and e-check users drive 57% of churn. Pandas, Seaborn, Matplotlib.

# Telco Customer Churn Analysis

Exploratory data analysis of 7,043 telecom customers to find what drives churn, using Python.

**Stack:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

---

## Key Findings

| Finding | Result |
|---|---|
| Overall churn | 26.5% (1,869 of 7,043 customers) |
| Month-to-month contracts | 42.7% churn vs 11.3% (1-year) and 2.8% (2-year), about 15x the two-year rate |
| Share of all churn from month-to-month | About 89% |
| Electronic-check payers | 45.3% churn vs 15.2% (credit card), 16.7% (bank transfer), 19.1% (mailed check) |
| Electronic-check share | 34% of customers, 57% of all churn |
| Estimated annualized revenue at risk | About $1.45M (1,869 churned customers x $64.76 average monthly charge x 12) |

---

## What I Did

- Converted `TotalCharges` to numeric, treating blanks as 0 for customers with zero tenure
- Checked for nulls and duplicate customer IDs (none found)
- Recoded `SeniorCitizen` from 0/1 to No/Yes for readability
- Visualized churn by contract type, payment method, tenure, gender and service add-ons

---

## Run It

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook churn_analysis.ipynb
```

The dataset (`Customer Churn.csv`) is in the same folder as the notebook.

---

## Next Steps

- Churn rate by tenure bucket and internet service type
- Logistic regression baseline to predict churn

---

## Data

Telco customer churn sample dataset (7,043 rows, 21 columns).
