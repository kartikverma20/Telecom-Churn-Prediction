**Telecom Churn Prediction**
## ** Overview**
Predicts which telecom customers are likely to churn using historical data, exploratory analysis, feature engineering, class balancing, and machine learning models. The goal is to identify at-risk customers and provide insights to reduce churn.

## ** Dataset**
* Customer information (gender, tenure, contract type, payment method, etc.)
* Numerical features: MonthlyCharges, TotalCharges, Tenure
* Target: Churn (Yes/No)

## ** Exploratory Data Analysis (EDA)**
* **Univariate Analysis:** Distribution of numerical features (histograms, boxplots) and categorical features (bar plots, proportions).
* **Bivariate Analysis:**

  * Categorical vs categorical: Chi-squared tests, cross-tabulations.
  * Numerical vs categorical: Boxplots, violin plots, t-tests / Mann-Whitney tests.
  * Numerical vs numerical: Correlation analysis, scatter plots, heatmap.

## ** Feature Engineering**
* Created interaction features (e.g., Contract + PaymentMethod)
* Binary flags for thresholds (e.g., HighMonthlyCharge, ShortTenure)
* Encoded categorical features (manual mapping for binary, label encoding/one-hot for multi-class)

## ** Data Preprocessing**
* Scaled numerical features using **StandardScaler / MinMaxScaler**
* Handled class imbalance using **SMOTE** (oversampling only on training set)

## ** Modeling**
Trained and evaluated multiple models:
* **Decision Tree**
* **Random Forest**
* **Support Vector Machine (SVM)**

Metrics evaluated: Accuracy, Precision, Recall, F1-score

## ** Model Comparison**
* Visual comparison of models using bar charts for metrics
* Confusion matrices for each model to see classification performance
* Random Forest / best-performing model selected based on F1-score and balanced performance
