# Task-4
## 📌 Customer Churn Prediction (Telecom)

## 🎯 Objective

This project predicts whether a telecom customer is likely to churn (leave the service) based on their demographic, account, and usage details.
## Tools Used: 
- Python (Pandas, Matplotlib, Seaborn, numpy, scikit-learn)
- Jupyter Notebook
## 📂 Dataset :[Telco_Customer_Churn.csv](https://github.com/user-attachments/files/22206998/Telco_Customer_Churn.csv)

## 🔎 Steps Performed

### Data Preprocessing

- Dropped customerID (not useful for prediction).

- Converted TotalCharges to numeric and filled missing values.

- Encoded categorical variables:

- LabelEncoder for binary columns (Yes/No).

- OneHotEncoder for multi-class categorical features.

- Scaled numerical columns (tenure, MonthlyCharges, TotalCharges) using StandardScaler.

### Model Building

- Split dataset into train (80%) and test (20%) sets.

- #### Trained two models:

- Logistic Regression

- Random Forest Classifier

### Model Evaluation

- Accuracy Score
  
- Classification Report (Precision, Recall, F1-score)

- Confusion Matrix

- Feature Importance (Random Forest)

### Model Saving

- Best performing model (RandomForestClassifier) was saved as churn_model.pkl using joblib.


## 📊 Results

- Random Forest Accuracy: ***79%***

  ### Top Features Influencing Churn:

- Monthly charges

- Payment method

- Online security

