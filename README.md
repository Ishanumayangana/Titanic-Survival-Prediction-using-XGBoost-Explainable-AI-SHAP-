# 🚢 Titanic Survival Prediction using XGBoost & Explainable AI (SHAP)

![XGBoost Logo](https://upload.wikimedia.org/wikipedia/commons/6/69/XGBoost_logo.png)

## 📌 Project Overview
This project applies **Machine Learning & Explainable AI** techniques to predict passenger survival on the **Titanic dataset**.  
The highlight of this project is using **XGBoost** (Extreme Gradient Boosting) along with **SHAP (SHapley Additive Explanations)** for model interpretability.  

I also compare XGBoost with other popular algorithms (Logistic Regression, Random Forest, LightGBM, CatBoost) to show performance differences.  

---

## 🎯 Objectives
- Perform **data preprocessing & feature engineering**  
- Train an **XGBoost classifier** with hyperparameter tuning  
- Compare XGBoost with **other ML algorithms**  
- Visualize **feature importance, confusion matrix, learning curves**  
- Apply **Explainable AI (SHAP)** for interpretability  

---

## 🛠️ Tech Stack
- **Languages**: Python  
- **Libraries**:  
  - [XGBoost](https://xgboost.readthedocs.io/)  
  - [LightGBM](https://lightgbm.readthedocs.io/)  
  - [CatBoost](https://catboost.ai/)  
  - [Scikit-Learn](https://scikit-learn.org/)  
  - [SHAP](https://shap.readthedocs.io/)  
  - [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/)  

---

## 📊 Dataset
I used the **Titanic dataset** (from Seaborn).  
- Target variable: `survived` (0 = Did not survive, 1 = Survived)  
- Features: Passenger class, age, gender, siblings/spouses aboard, parents/children aboard, fare, and embarkation port.  

---

## 🔑 Key Features
### 1. Feature Engineering
- Handling missing values (Age, Embarked)  
- Encoding categorical variables (`sex`, `embarked`, etc.)  
- Dropping irrelevant features  

### 2. Model Training
- **Baseline XGBoost model**  
- **Hyperparameter tuning** using GridSearchCV / Optuna  
- **Evaluation metrics**: Accuracy, Classification Report, Confusion Matrix  

### 3. Model Comparison
We compared **5 models**:  
- Logistic Regression  
- Random Forest  
- LightGBM  
- CatBoost  
- XGBoost  

### 4. Explainable AI with SHAP
- **SHAP Summary Plot**: Global feature importance  
- **SHAP Bar Plot**: Mean feature impact  
- **SHAP Dependence Plot**: Feature interactions  

---

## 📈 Results
- **XGBoost** achieved the best balance of accuracy and interpretability.  
- Feature importance showed that **gender, passenger class, and fare** were the strongest predictors.  
- SHAP provided **clear explanations** of why certain passengers survived.  
