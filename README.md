## 🏥 Health Insurance Cost Prediction

### 📌 Project Overview

This project implements an end-to-end machine learning regression pipeline to predict Medical Insurance Charges. By analyzing patient demographics and health metrics, the model provides an estimate of health care costs, which is a critical task for both insurance providers and policyholders.

### 📊 Dataset Description
The dataset includes several key features that influence healthcare premiums:

Feature      |   Description
Age          |   Age of the primary beneficiarr
Sex          |  Insurance contractor gender (Female, Male)
BMI          |  Body Mass Index (kg/m^2), providing an understanding of body weight relative to height
Children.    |   Number of children covered by health insurance / Number of dependents
Smoker.      |  Smoking status of the beneficiary
Region.      |   The beneficiary's residential area in the Us
Charges      |  Target Variable: Individual medical costs billed by health insurance




### ⚙️ The Workflow

1. Data Preprocessing
To ensure model integrity and prevent Data Leakage, the following steps were taken:
Encoding: Categorical variables (Sex, Smoker, Region) were transformed into numerical format.
Train-Test Split: Data was split before any scaling to ensure the model remains "blind" to the test set.
Feature Scaling: Applied StandardScaler to normalize the feature ranges, ensuring the Linear Regression model converges efficiently.


3. Model Architecture
We utilized Linear Regression, which models the relationship between features using the equation:
y = \beta_0 + \beta_1x_1 + \beta_2x_2 + ... + \beta_nx_n + \epsilon




✅ Model Performance

The model was evaluated using metrics that account for both fit and complexity:
R² Score: ~0.80 (The model explains 80% of the variance in charges)
Adjusted R²: ~0.79

🧠 Key Technical Learnings

Data Leakage Prevention: Learned why scaling must happen after the split to avoid information from the test set "leaking" into the training phase.
Feature Engineering: Observed how specific features (like smoker status) have a disproportionately high impact on the target variable.
Statistical Robustness: Understanding why Adjusted R² is a more reliable metric than standard R² when evaluating multiple features.

🛠 Tech Stack

Language: Python
Data Manipulation: Pandas, NumPy
Visualization: Matplotlib, Seaborn
Machine Learning: Scikit-learn



🚀 Future Roadmap

[ ] Non-Linear Models: Implement Random Forest and XGBoost to capture non-linear relationships.
[ ] Log Transformation: Apply log(y) to the target variable to handle skewed price distributions.
[ ] Deployment: Create a Flask or Streamlit web app for real-time predictions.
