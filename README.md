# Machine Learning Finance Project  
## Bankruptcy Prediction (Taiwan)

Academic machine learning project focused on **predicting corporate bankruptcy**
using financial indicators from Taiwanese companies.

---

## Project overview
This project analyzes bankruptcy data from the **Taiwan Economic Journal**
covering the years **1999–2009**.
A company is labeled as bankrupt according to the business regulations of the
**Taiwan Stock Exchange**.

The objective is to build robust machine learning models capable of detecting
early signs of bankruptcy based on financial ratios.

---

## Objectives
- Explore and understand a high-dimensional financial dataset
- Clean and preprocess financial data
- Handle class imbalance and outliers
- Train and compare multiple classification models
- Evaluate model performance using relevant metrics

---

## Dataset
- **6,819 companies**
- **96 columns** (95 financial features + target variable)
- Examples of financial indicators:
  - Debt Ratio
  - Borrowing Dependency
  - Current Liability to Assets
  - Net Income / Total Assets

The dataset is **highly imbalanced**, with significantly fewer bankrupt companies.

---

## Data preprocessing
Main preprocessing steps include:
- **Outlier handling**  
  Values below the 15% quantile and above the 85% quantile were capped to reduce
  noise while preserving useful information.
- **Dimensionality reduction**  
  Principal Component Analysis (PCA) was applied to reduce the feature space
  (from 95 features to approximately 20–27 components).
- **Class imbalance handling**  
  Borderline SMOTE was used to balance bankrupt and non-bankrupt classes.

---

## Models implemented
This is a **binary classification** problem.  
The following models were trained and compared:

- Logistic Regression
- Random Forest Classifier
- XGBoost
- CatBoost
- LightGBM
- Stacking Classifier

Hyperparameters were optimized using **Grid Search**.

---

## Evaluation metrics
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrices

Tree-based models and ensemble methods achieved the best performance.

---

## Repository structure

.
├── TaiwanBankruptcy.ipynb      # Main analysis notebook
├── code_snippets.ipynb         # Utility and experimentation code
├── data.csv                    # Dataset
├── presentation/               # Slides and final report
│   ├── ml-finance-project-presentation.pdf
│   ├── ml-finance-project-report.pdf
│   └── README.md
└── README.md


---

## Presentation & report
The full **project presentation slides** and **final report** are available in the  
[`presentation`](./presentation) folder.

---

## Academic context
This project was developed as part of a **Machine Learning / Finance academic course**.

This repository is an **individual presentation repository** of a **group project**  
and is shared for **educational and portfolio purposes only**.
