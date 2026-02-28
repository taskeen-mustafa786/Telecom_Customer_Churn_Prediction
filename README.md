# Telecom Customer Churn Prediction

A machine learning project demonstrating **customer churn prediction** using classification models
and production-ready scikit-learn pipelines.

## 📋 Objective
Build a predictive model to classify whether a customer will churn (leave) or stay with a telecom company.
The project focuses on constructing robust, reusable machine learning pipelines with proper data preprocessing
and hyperparameter tuning.

## 📁 Dataset
- Data is sourced from the **IBM Telco Customer Churn** dataset.
- The dataset includes customer demographics, account information, and usage patterns.
- Target variable: `Churn` (Yes/No) - whether the customer churned.
- Includes both numerical features (age, charges, tenure) and categorical features (contract type, services).

## 🛠️ Models Applied
1. **Logistic Regression** – a simple baseline for binary classification with interpretability.
2. **Random Forest Classifier** – an ensemble method capable of capturing complex, non-linear patterns.

Both models are tuned using GridSearchCV with 5-fold cross-validation to find optimal hyperparameters.

## 🔧 Pipeline Architecture
- **Numeric Features**: Imputation (median strategy) + Standardization
- **Categorical Features**: Imputation (constant strategy) + One-Hot Encoding
- **Feature Preprocessing**: ColumnTransformer for automated handling of mixed data types
- **Model Export**: Joblib serialization for deployment in production environments (Flask, FastAPI, Cloud Functions)

## 📊 Key Results & Findings
- Models are evaluated using F1-score and cross-validation.
- Classification reports include precision, recall, and F1-score for each class.
- The complete pipeline (preprocessor + classifier) is exported as `telco_churn_pipeline.pkl`.
- Confusion matrices and detailed metrics provide insights into model performance.

## 🧠 Skills Demonstrated
- Data preprocessing and pipeline construction with scikit-learn
- Handling mixed data types (numerical and categorical features)
- Hyperparameter tuning using GridSearchCV
- Binary classification modeling
- Model serialization and production readiness
- Classification evaluation metrics

## 📝 Usage
Open the notebook at `dh_int_02.ipynb` to walk through:
1. Environment setup and library imports
2. Data loading and preprocessing pipeline construction
3. Model selection and hyperparameter tuning
4. Model evaluation and pipeline export

The notebook provides a production-ready template for churn prediction tasks.
