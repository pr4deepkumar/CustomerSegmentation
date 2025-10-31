# Customer Segmentation for Loan Cross-Selling

## Project Overview
This project analyzes customer data from a Bank to identify profitable segments for **personal loan cross-selling**.  
The dataset originates from a pilot campaign where 20,000 customers were offered a personal loan.

- **2,512 customers** accepted the offer (`TARGET = 1`)  
- **17,488 customers** declined (`TARGET = 0`)

The goal of this project is to develop and evaluate classification models that will predict whether a customer will respond positively to a cross-selling offer for a loan with the highest accuracy.

---

## Objectives
- Analyze the dataset to understand the relationships between customer attributes and loan acceptance.  
- Build baseline predictive models to identify factors influencing a positive response.
- Use cross-validation to find the best predictive model for classification.
- Evaluate the limitations of the current data and models to inform future strategy.

---

## Methodology

### 1. Data Preprocessing
Cleaned and prepared numerical and categorical features for modeling.

### 2. Exploratory Data Analysis (EDA)
Visualized relationships between customer attributes (e.g., balance, transactions) and the target variable (loan acceptance).

### 3. Predictive Modeling
Tested various classification models, including **tree-based ensembles**, to predict loan acceptance.

### 4. Model Tuning
Applied appropriate **scaling**, **resampling** (to handle class imbalance), and **hyperparameter tuning** to enhance model generalization.

---

## Results & Insights

- **Modest Accuracy**:
  Predictive performance was constrained more by data richness than by model complexity. 
- **Nonlinear Patterns**:  
  The relationship between account balance and loan acceptance was **nonlinear** — customers with extremely high or low balances were less likely to accept.  
- **Class Imbalance**:  
  The imbalance between accepted (2,512) and declined (17,488) offers reduced sensitivity to the minority class (acceptances).  
- **Model Limitations**:  
  Tree-based ensembles performed better than linear models but still lacked discriminative power to fully capture complex customer behavior.

---

## Conclusion & Future Work

This study successfully met its **exploratory objective** by diagnosing the limits of the current models and data.  
The key takeaway: **Predictive performance depends more on data richness and representation than on model choice.**

### Future Work
- **Deeper Feature Extraction**: Engineer new features that better capture customer intent.  
- **Temporal Pattern Analysis**: Analyze behavioral patterns over time, not just at a single snapshot.  
- **Advanced Models**: Explore hybrid approaches or deep learning models to capture complex, nonlinear relationships.

---

## Tech Stack

| Category | Tools |
|-----------|--------|
| Data Manipulation | `pandas`, `numpy` |
| Data Visualization | `matplotlib`, `seaborn` |
| Statistical Analysis | `scipy` |
| Machine Learning | `scikit-learn` (preprocessing, model selection, classification, evaluation) |

---

## Files

| File | Description |
|------|--------------|
| `PL_XSELL_Project.ipynb` | Jupyter Notebook with the full analysis |
| `PL_XSELL.csv` | Dataset used for the analysis |
| `PL_XSELL_METADATA.xlsx` | Metadata (data dictionary) for the dataset |

---

## How to Run

### 1. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter

``` 
### 2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook MyBank_Project.ipynb
   ```
