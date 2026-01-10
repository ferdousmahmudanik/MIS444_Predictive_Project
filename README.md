# MIS444_Predictive_Project
# Retention_Predictor(Predict behavior to retain customers of IBM)

Predictive Analytics project for customer churn using Python(MIS444)
RetentionRadar is a predictive analytics solution developed for the MIS444 Course Project. The primary goal is to identify customers at risk of leaving a telecommunications provider (churning). By leveraging machine learning, the business can shift from reactive troubleshooting to proactive retention strategies.

📊 Dataset

Source: Kaggle Telco Customer Churn Dataset 
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

Size: ~7,043 customer records.

Key Features:

Demographics: Gender, Senior Citizen status, Dependents.

Services: Fiber optic, DSL, Tech Support, Online Security.

Account Info: Tenure, Contract type (Month-to-month, Annual), Monthly Charges.

Target: Churn (Yes/No).

🛠️ Technical Workflow

Data Preprocessing:

Cleaned TotalCharges by handling missing strings and imputing with the median.

Encoded categorical variables using One-Hot Encoding.

Scaled numerical features using StandardScaler.

Exploratory Data Analysis (EDA):

Identified high churn correlation with month-to-month contracts.

Visualized the "Danger Zone" (first 6 months of tenure).

Modeling:

Baseline: Logistic Regression.

Primary Model: Random Forest Classifier.

Optimization: Hyperparameter tuning via GridSearchCV (optimizing for F1-Score).

📈 Key Results

Model Accuracy: ~80%

ROC-AUC Score: 0.84

Top Predictors:

Contract Type: Month-to-month users are the highest risk group.

Tenure: Customer loyalty increases significantly after 12 months.

Internet Service: Fiber optic users show higher churn rates, suggesting potential service/pricing issues.




