🏦 Loan Approval Prediction using Machine Learning
Project Overview

This project focuses on predicting loan approval status based on applicant and loan-related attributes using multiple machine learning classification models.
The goal is to analyze customer data, preprocess it effectively, train different models, and compare their performance using standard evaluation metrics such as Accuracy, Confusion Matrix, Classification Report, and ROC–AUC Curve.

The project follows a complete data science pipeline, making it suitable for academic evaluation as well as portfolio presentation.

Dataset Description

The dataset contains information related to loan applicants, including:

Demographic Details: Gender, Marital Status, Dependents, Education

Financial Information: Applicant Income, Co-applicant Income, Loan Amount

Loan Details: Loan Amount Term, Credit History, Property Area

Target Variable: Loan Status (Approved / Not Approved)

The dataset was loaded from a CSV file and inspected for missing values, data types, and overall structure.

⚙️ Data Preprocessing

Several preprocessing steps were applied to ensure data quality and model readiness:

🔹 Handling Missing Values

Forward Fill (ffill) was applied to categorical features such as Gender, Married, Dependents, Self Employed, and Credit History.

Mean Imputation was used for numerical features like Loan Amount and Loan Amount Term.

🔹 Feature Engineering

The Loan_ID column was removed as it does not contribute to prediction.

Label Encoding was applied to convert categorical variables into numerical format.

Standard Scaling was used on numerical features to normalize data and improve model performance.

📊 Exploratory Data Analysis (EDA)

To better understand the dataset, the following visualizations were created:

Correlation Heatmap to analyze relationships between variables.

Pie Chart to visualize the distribution of loan approvals vs rejections.

These visualizations help in identifying influential features and understanding class distribution.

🤖 Machine Learning Models Implemented

The following classification models were trained and evaluated:

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest Classifier

Each model was trained on the same training data and evaluated on a common test set to ensure fair comparison.

📈 Model Evaluation Metrics

The models were evaluated using:

Accuracy Score

Confusion Matrix

Classification Report (Precision, Recall, F1-Score)

ROC–AUC Score

ROC Curves

Additionally:

Individual ROC curves were plotted for each model.

A combined ROC curve was created to visually compare model performance.

A bar chart was used to compare accuracy scores across models.

🏆 Results & Observations

Ensemble models like Random Forest showed strong performance due to their ability to capture non-linear patterns.

Logistic Regression provided a solid baseline with good interpretability.

ROC–AUC comparison highlighted the trade-off between sensitivity and specificity for each model.

Feature scaling significantly improved the performance of distance-based models like KNN and SVM.

🛠️ Technologies & Libraries Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn
