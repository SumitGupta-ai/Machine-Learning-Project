🏥 Health Insurance Cost Prediction

This project focuses on building a machine learning regression model to predict medical insurance charges based on patient details.
It demonstrates a complete end-to-end ML workflow with proper preprocessing, model training, and evaluation.

📌 Problem Statement

Health insurance costs depend on several factors such as age, BMI, smoking status, and number of children.
The goal of this project is to predict insurance charges using these features with a regression model.

1 📊 Dataset

° The dataset contains the following features:

° age – Age of the individual

° sex – Gender (encoded numerically)

° bmi – Body Mass Index

° children – Number of dependents

° smoker – Smoking status (encoded)

° region – Residential region (encoded)

° charges – Health insurance cost (target variable)

Note: All categorical variables were converted into numerical format before modeling.

2 ⚙️ Approach

° Data cleaning and preparation

° Train–test split to avoid data leakage

° Feature scaling using StandardScaler

° Model training using Linear Regression

° Model evaluation using R² Score and Adjusted R²

3 ✅ Model Performance

° R² Score: ~0.80

° Adjusted R²: ~0.79

The results indicate that the model explains approximately 80% of the variance in insurance charges, which is strong performance for real-world insurance data.

4 🧠 Key Learnings

° Importance of applying preprocessing after train-test split

° Understanding data leakage and how to avoid it

° Difference between R² and Adjusted R²

° Evaluating regression models beyond simple accuracy

5 🛠 Tech Stack

° Python

° Pandas

° NumPy

° matplotlib

° seaborn

° Scikit-learn

° Linear Regression

6 🚀 Future Improvements

Try non-linear models (Random Forest, Gradient Boosting)

Apply log transformation on target variable

Perform feature interaction and model comparison
