We want to build a model to identify profitable customer segments for cross-selling personal loans at MyBank. The bank executed a pilot campaign, sending offers for personal loans with an attractive interest rate of 12% and a waived processing fee to 20,000 customers via email, SMS, and direct mail. Out of these, 2,512 customers showed interest in the offer, indicated by the "TARGET" variable being marked as 1, while the remaining 17,488 customers did not respond positively.

Our goal is to analyze the data, which includes various demographic and behavioral variables, and identify customer segments that are likely to respond positively to the loan offer. The data will be pre-processed accordingly, and we will make necessary assumptions, such as the data being a Simple Random Sample, independently and identically distributed (i.i.d.), and normally distributed (or assuming normality based on the Central Limit Theorem). 

By developing a predictive model, we aim to find customer groups that are the most profitable to target for future cross-selling of personal loans.

The project uses the following tools/concepts:

1. **Data Manipulation & Visualization**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `pylab`
2. **Statistical Analysis**: `scipy`, `scipy.stats`
3. **Machine Learning**: `sklearn` (for model selection, preprocessing, classification, clustering, feature selection, and evaluation)
