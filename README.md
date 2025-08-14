# Customer Segmentation for Loan Cross-Selling

## Project Overview

This project analyzes customer data from **MyBank** to identify profitable segments for **personal loan cross-selling**.
The dataset comes from a pilot campaign where **20,000 customers** were offered loans at a **12% interest rate** with a **waived processing fee**. Out of these:

* **2,512 customers** accepted the offer (**TARGET = 1**)
* **17,488 customers** declined (**TARGET = 0**)

Our goal is to analyze demographic and behavioral variables to find **customer profiles most likely to respond positively** in future campaigns.

## Objectives

1. **Analyze** the dataset to detect key factors influencing loan acceptance.
2. **Segment** customers into profitable groups for targeted marketing.
3. **Build** predictive models to assist in cross-sell decision-making.

## Methodology

* **Data Preprocessing**: Checked for missing values, cleaned categorical/numerical features, removed anomalies.
* **Statistical Assumptions**: Treated data as a simple random sample, i.i.d., and assumed approximate normality via the **Central Limit Theorem**.
* **Exploratory Data Analysis (EDA)**: Visualized relationships between customer attributes and loan acceptance.
* **Clustering**: Identified 3 customer clusters, with only 1 being highly profitable.
* **Classification Modeling**: Tested multiple algorithms to predict loan acceptance and cluster membership.

## Results & Insights

* **High balance**, **self-employed**, and customers in their **30s–40s** were more likely to take loans.
* **Holding Period**, **Total Transactions**, and **Debit Transactions** emerged as top features for segmentation.

## Best Models
  * **Loan Acceptance Prediction ('TARGET' column)**: K-Nearest Neighbors (**91% accuracy** without overfitting).
  * **Cluster Classification ('CLUSTER' column)**: Support Vector Classifier (**98% accuracy** without overfitting).
* **Business Recommendation**: Focus marketing efforts on the profitable cluster while creating alternative schemes to attract other segments.

## Tech Stack

* **Data Manipulation & Visualization**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `pylab`
* **Statistical Analysis**: `scipy`, `scipy.stats`
* **Machine Learning**: `scikit-learn` (model selection, preprocessing, classification, clustering, feature selection, evaluation)

## Files

```
MyBank_Project.ipynb      # Jupyter Notebook with full analysis and visualizations
MyBank_DATA.csv           # Dataset used for analysis
MyBank_METADATA.xlsx      # Metadata for dataset columns
```

## How to Run

1. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
   ```
2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook MyBank_Project.ipynb
   ```