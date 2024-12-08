
# Predicting Shipping Times and Profit Trends: A Data-Driven Approach

## Project Overview
This project analyzes a dataset of over 5 million records to provide actionable insights for a hypothetical company in shipping logistics and profitability. Using data science and machine learning methodologies, we addressed two key business questions:

1. Can we predict shipping times based on order priority, product type, and region?
2. Does unit price impact profit?

## Key Features
- **Dataset Size:** ~5 million records
- **Data Source:** [Excelbianalytics](https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/)
- **Tools & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels
- **Machine Learning Techniques:** Random Forest, Ordinary Least Squares Regression
- **Statistical Methods:** Correlation Analysis, Hypothesis Testing

---

## Required Libraries
Ensure you have Python installed along with the following libraries:
- `matplotlib`
- `pandas`
- `numpy`
- `scipy`
- `scikit-learn`

---

## Structure
The code is organized as follows:
- **`main.py`:** Runs all the functions and acts as the entry point of the project.
- **`clean_data.py`:** Contains the `cleanAndSortData()` function for preprocessing the raw dataset.
- **`generate_plots.py`:** Implements functions for visualizations and graphical analysis.

---

## Data Cleaning & Preparation
The data was preprocessed through the following steps:
- Removed 2.3 million duplicate rows and irrelevant columns.
- Added calculated features (e.g., Days to Ship).
- Encoded categorical variables:
  - **Label Encoding** for ordinal categories like order priority.
  - **One-Hot Encoding** for nominal categories like item type and region.

---

## Analysis & Results

### Question 1: Can Shipping Times Be Predicted?
- **Model Used:** Random Forest Classifier
- **Results:** Test accuracy of 1.9%. Due to uniformly distributed data and lack of correlation, it was concluded that shipping times cannot be reliably predicted.

### Question 2: Does Unit Price Impact Profit?
- **Methodology:** Correlation analysis, scatter plots, and Ordinary Least Squares (OLS) regression.
- **Results:**
  - A positive linear relationship between unit price and profit was observed.
  - OLS Regression confirmed statistical significance (p < 0.05), with an R² value of 0.333, indicating unit price explains 33% of profit variability.

---

## Files Produced
At the beginning of `main.py`, the function `cleanAndSortData(dataFrame_raw, output_file_name)` is executed, which creates a cleaned dataset file named `SalesRecordClean.csv`. This cleaned file is used for the data analysis.  
For details about `cleanAndSortData()`, refer to the **ETL Section** of the project.

---

## Running the Code
Run the project using the following command:

```bash
python3 main.py [INPUT_PATH]
```

For example:
```bash
python3 main.py SalesRecords/SalesRecords_5m.csv
```

Make sure the dataset is downloaded and placed in the specified path before running the script.  

**Download Dataset:** [Sample CSV Files for Testing Sales](https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/)

---

## Conclusion
- Predicting shipping times was infeasible due to the dataset's limitations (uniform distribution and lack of correlations).
- Unit price positively impacts profitability, suggesting a focus on higher-priced products for greater margins.

---

## Project Contributions
### Ozafa Mahmood
- Built predictive models and conducted regression analysis.
- Performed data preprocessing, feature engineering, and exploratory data analysis (EDA).
- Validated business insights using statistical tests and residual checks.

### Daniel Surina
- Conducted data analysis and implemented predictive models.
- Created visualizations and performed statistical testing to uncover trends.

--- 

This README provides a comprehensive overview of the project and instructions to reproduce the analysis.
