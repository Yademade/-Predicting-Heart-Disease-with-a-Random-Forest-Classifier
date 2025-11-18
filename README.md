GROUP ONE
1. Meron Bimrew………………………………….1339
2.Amanuel Ewnetu………………………………..1077
3.Yabsera Amsalu…………………………………0833
4.Metmku Yohannes………………………………1479
5.Meron Tadesse…………………………………..1519
6.Edlam Wondesen………………………………...1465


# -Predicting-Heart-Disease-with-a-Random-Forest-Classifier
📌 Heart Failure Prediction Dataset – Data Mining Project
1. Title & Introduction

Project Title:
Heart Failure Prediction Using Machine Learning

Introduction:
The goal of this project is to analyze the Heart Failure Prediction Dataset and build machine learning models that can predict whether a patient is likely to have heart disease based on various medical attributes. The project focuses on data cleaning, exploratory analysis, feature processing, model development, and evaluation.

2. Data Loading

The dataset was obtained from Kaggle (“Heart Failure Prediction Dataset”).
It was loaded into Google Colab using the file uploader.

The raw data was inspected by viewing:

  .The first few rows
  .Column names
  .Basic dataset shape (rows, columns)

This step helps verify that the dataset was correctly imported.

3. Data Cleaning & Preprocessing

To prepare the data for analysis and modeling, several cleaning steps were performed:

✔ Missing Values

Columns were checked for null values.
Missing numerical values were handled using median imputation.
Missing categorical values were filled with the most frequent category.

✔ Handling Outliers

Key features like cholesterol and maximum heart rate were inspected visually.
Outliers were addressed using appropriate transformations or by capping extreme values.

✔ Data Type Corrections

Columns were checked to ensure they had the correct types (e.g., numeric, categorical).
Boolean-like columns were converted to integer (0/1).

This process ensures the dataset is consistent, clean, and ready for modeling.

4. Exploratory Data Analysis (EDA)

EDA was performed to understand the relationships and patterns within the dataset.
Key steps included:

✔ Target Variable Distribution

Visualized the count of patients with and without heart disease.

✔ Correlation Heatmap

Numerical features were compared to identify strong correlations with the target.

✔ Feature Distributions

Histograms and KDE plots were used to examine the spread of important variables such as:

  .Age
  .Cholesterol
  .Resting blood pressure
  .Maximum heart rate

✔ Insights

  .Age and chest pain type showed meaningful patterns.
  .Certain features had skewed distributions requiring scaling later.
  .Some variables had moderate correlation with the target.

5. Feature Engineering

Feature engineering was performed to improve model accuracy and interpretability.

✔ New Features

  .Age was categorized into bins/groups to capture risk categories (e.g., <30, 30–45, 45–60, 60+).

✔ Encoding Categorical Variables

Categorical columns were transformed using One-Hot Encoding to convert them into numeric form suitable for machine learning algorithms.

✔ Scaling Numerical Data

Continuous variables were standardized so models like Logistic Regression and SVM could perform better.

These steps ensured all input features were properly formatted and optimized for modeling.

6. Model Building

The cleaned dataset was split into training (80%) and testing (20%) sets.

Multiple machine learning models were built and trained, including:

  .Logistic Regression
  .Decision Tree
  .Random Forest
  .K-Nearest Neighbors
  .Support Vector Machine
  .XGBoost (if available)

Each model was trained using the preprocessed features to learn patterns associated with heart disease.

7. Model Evaluation

The performance of each model was assessed using various evaluation metrics, such as:

✔ Accuracy

Measures overall correctness of predictions.

✔ Precision, Recall, F1-Score

Used for deeper classification analysis, especially when class imbalance exists.

✔ ROC-AUC

Measures how well the model separates positive vs negative classes.

✔ Confusion Matrix

Visualizes correct and incorrect predictions.

✔ Cross-Validation

Top-performing models were further validated using 5-fold cross-validation to check consistency.

✔ Best Model

The best model was selected based on accuracy, ROC-AUC, and cross-validation performance.
This final model was retrained on the entire dataset and saved for future use.

8. Conclusion & Discussion
✔ Summary of Findings

  .EDA revealed meaningful relationships between age, chest pain, cholesterol, and heart disease.
  .Models like Random Forest or XGBoost generally performed best.
  .Preprocessing (scaling, encoding, imputation) significantly improved model accuracy.

✔ Limitations

  .The dataset may not generalize to all populations.
  .Some important medical features were not included.
  .Hyperparameter tuning was not extensively performed.

✔ Recommendations for Improvement

  .Apply GridSearchCV or RandomizedSearchCV for parameter optimization.
  .Use external datasets for validation.
  .Deploy the final model using a web interface (Flask or FastAPI).
  .Explore feature importance to better understand risk factors.


