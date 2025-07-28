# Credit Risk Benchmark Dataset

**Source:** [Adil Shamim on Kaggle](https://www.kaggle.com/datasets/adilshamim8/credit-risk-benchmark-dataset)  
**License:** Attribution 4.0 International (CC BY 4.0)

## Overview

This dataset is designed for benchmarking AutoML and predictive modeling in the financial domain. The main task is to predict whether a borrower will experience serious delinquency within two years, using a mix of financial metrics and personal attributes.

## Dataset Characteristics

- **Features:** 10 predictors, 1 target variable
- **Data Types:** All predictors are numerical (real numbers); target is binary (`0` = No delinquency, `1` = Yes delinquency)
- **Task:** Binary classification (credit risk prediction)

## Column Descriptions

| Column         | Description                                                        |
|----------------|--------------------------------------------------------------------|
| `rev_util`     | Ratio of revolving credit utilization (balance/credit limit)        |
| `age`          | Age of the borrower                                                |
| `late_30_59`   | Number of times 30-59 days past due                                |
| `debt_ratio`   | Debt to income (or assets) ratio                                   |
| `monthly_inc`  | Monthly income of the borrower                                     |
| `open_credit`  | Number of open credit lines and loans                              |
| `late_90`      | Number of times 90+ days late on a payment                         |
| `real_estate`  | Number of real estate loans or credit lines                        |
| `late_60_89`   | Number of times 60-89 days past due                                |
| `dependents`   | Number of dependents                                               |
| `dlq_2yrs`     | Target: Serious delinquency in next 2 years (`0` = No, `1` = Yes)  |

## Use Cases

- **Risk Management:** Build and validate credit scoring models to forecast borrower default risks.
- **AutoML Benchmarking:** Compare performance of AutoML frameworks on structured financial data.
- **Academic Research:** Analyze credit behavior and predictive power of financial indicators.
- **Model Interpretability:** Test feature importance and explainable AI solutions in a regulated context.

## Additional Information

- **Preprocessing:** Perform exploratory data analysis, handle missing values/outliers, and apply scaling or feature transformations.
- **Regulatory Considerations:** Ensure model transparency and interpretability.
- **Benchmarking:** Suitable for comparing traditional models (e.g., logistic regression) with modern approaches (e.g., gradient boosting, neural networks).

---

For more details and to download the dataset, visit the [Kaggle dataset page](https://www.kaggle.com/datasets/adilshamim8/credit-risk-benchmark-dataset).