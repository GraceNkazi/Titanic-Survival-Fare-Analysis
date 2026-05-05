# Titanic Survival & Fare Prediction: A Machine Learning Study

## 📌 Project Overview
This project explores the Titanic dataset to solve two distinct machine learning problems:
1. **Regression:** Predicting the passenger's fare based on Age, Pclass, and Sex.
2. **Classification:** Predicting passenger Survival.

The project follows a  70/15/15 Data Split (Train, Validation, Test) to ensure model generalization and avoid overfitting.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib/Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📊 Data Preprocessing
To meet the project requirements, the following steps were taken:
* **Missing Value Handling:** Rows with missing Age or Fare values were dropped to ensure data integrity.
* **Categorical Encoding:** The Sex column was mapped to numerical values (Male: 0, Female: 1).
* **Feature Scaling:** StandardScaler was applied to numerical features to optimize performance for distance-based models like KNN and SVC.

## 🤖 Models Implemented
### Regression
* Linear Regression 
* Decision Tree & Random Forest
* Gradient Boosting
* **Ensembles:** Voting Regressor (Best 3) & Bayesian Ensemble

### Classification
* Logistic Regression 
* Decision Tree & Random Forest
* Gradient Boosting
* Support Vector Classifier (SVC)
* **Ensemble:** Soft-Voting Classifier (RF + GB + SVC)

## 📈 Key Results

### Regression Performance
| Metric | Baseline (LR) | Voting Ensemble |
| :--- | :--- | :--- |
| **MAE** | $30.00 | **$25.50** |
| **Test R²** | 0.36 | **0.84** |

### Classification Performance
| Metric | Logistic Regression | Voting Ensemble |
| :--- | :--- | :--- |
| **Test Accuracy** | 77.78% | 76.85% |
| **Test Precision** | 0.72 | **0.77** |
| **F1-Score** | **0.75** | 0.71 |




