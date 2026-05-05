# Titanic Survival & Fare Prediction: A Machine Learning Study

## 📌 Project Overview
This project explores the Titanic dataset to solve two distinct machine learning problems:
1. **Regression:** Predicting the passenger `Fare` based on Age, Pclass, and Sex.
2. **Classification:** Predicting passenger `Survival` (Survived vs. Perished).

The project follows a rigorous **70/15/15 Data Split** (Train, Validation, Test) to ensure model generalization and avoid overfitting.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib/Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📊 Data Preprocessing
To meet the project requirements, the following steps were taken:
* **Missing Value Handling:** Rows with missing `Age` or `Fare` values were dropped to ensure data integrity.
* **Categorical Encoding:** The `Sex` column was mapped to numerical values (Male: 0, Female: 1).
* **Feature Scaling:** `StandardScaler` was applied to numerical features to optimize performance for distance-based models like KNN and SVC.

## 🤖 Models Implemented
### Regression
* Linear Regression (Baseline)
* Decision Tree & Random Forest
* Gradient Boosting
* **Ensembles:** Voting Regressor (Best 3) & Bayesian Ensemble

### Classification
* Logistic Regression (Baseline)
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

## 💡 Critical Takeaways
* **Complexity vs. Generalization:** While complex models (Random Forest) performed better on Validation data, simpler models like **Logistic Regression** showed superior robustness on the final Test set.
* **Ensemble Stability:** The **Voting Ensemble** significantly reduced prediction variance and provided the highest Precision for survival classification.
* **Feature Importance:** **Sex** and **Pclass** were consistently identified as the most influential features across all models.

## 📂 Project Structure
* `notebook.ipynb`: The main Jupyter Notebook containing all code, analysis, and visualizations.
* `Machine_Learning_Analysis_Report.pdf`: A formal summary of the project findings and methodology.
* `model_comparison.csv`: Exported metrics for all trained models.
