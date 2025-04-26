
# 📊 Analyzing Startup Failures and Predicting Overhype Trends

## Project Overview
This project explores startup failures across different industry sectors by analyzing structured and unstructured data from six datasets. The goals are:
- To uncover patterns and common causes of startup failure
- To develop predictive models for estimating the "Overhype" metric (binary classification)
- To extract insights using Natural Language Processing (NLP) on textual reasons for failure

---

## Team Members
- **Stuti Jandhyala**
- **Sunidi Vijayakrishna Kumar**
- **Akshata Krishnamohan**

---

## Datasets
- **Sources:** CB Insights' "Startup Failure Post-Mortem" compilation (last updated May 29, 2024)
- **Sectors Covered:** 
  - Finance and Insurance
  - Retail Trade
  - Food and Services
  - Manufacturing
  - Information Sector
- **Data Fields Include:** Name, Industry Sector, Funding Amounts, Years of Operation, Failure Reasons, Overhype Metric

---

## Project Workflow

### 1. Data Preprocessing
- Handling missing values (funding, years of operation, failure reasons)
- Standardizing and cleaning textual fields
- Encoding categorical variables
- Feature engineering: extracting operational years, funding buckets, etc.
- SMOTE resampling for balancing the Overhype classes

### 2. Exploratory Data Analysis (EDA)
- Visualization of failure trends across industries
- Correlation analysis between attributes
- Word cloud and sentiment analysis on textual fields

### 3. Modeling
- **Regression:**
  - Linear Regression (baseline)
  - Random Forest Regression
  - Gradient Boosting Models (e.g., XGBoost, LightGBM)
- **Classification:**
  - Logistic Regression
  - Decision Tree
  - Random Forest Classifier
  - SVM
- **Text Analysis:**
  - TF-IDF vectorization on "Why They Failed"
  - Sentiment and keyword extraction
  
### 4. Evaluation
- Regression Metrics: RMSE, MAE, R²
- Classification Metrics: Accuracy, Precision, Recall, F1-Score
- Cross-validation and hyperparameter tuning

---

## Libraries and Tools
- **Pandas** – Data manipulation
- **Matplotlib / Seaborn** – Visualization
- **Scikit-learn** – Machine learning models and metrics
- **NLTK / SpaCy** – Natural Language Processing
- **Imbalanced-learn (SMOTE)** – Class balancing
- **Jupyter Notebook** – Development environment

---

## Results
- Key trends and common patterns in startup failures identified
- Predictive model for "Overhype" metric developed with improved accuracy over baseline
- NLP insights: Sentiment trends and common themes extracted from textual failure reasons

---

## Potential Challenges
- Class imbalance in the Overhype metric (handled using SMOTE)
- Noisy and sparse text data requiring intensive preprocessing

---

## Future Work
- Incorporating more recent startup datasets for generalization
- Applying advanced NLP models (e.g., BERT) for deeper text understanding
- Building a web-based dashboard to display failure predictions interactively

---

## References
- [Speech and Language Processing - Stanford](https://web.stanford.edu/~jurafsky/slp3/)
- [NLP Class Notes – Georgia Tech](https://github.com/jacobeisenstein/gt-nlp-class/blob/master/notes/eisenstein-nlp-notes.pdf)
- [Springer Link – Text Analytics](https://link.springer.com/chapter/10.1007/978-81-322-3...)
