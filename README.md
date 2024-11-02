# Credit Default Prediction Using Machine Learning Models

**Overview:**  
This project applies machine learning models to predict credit default risks, offering insights to aid financial institutions in making data-driven lending decisions. It focuses on data preprocessing, feature selection, model training, and evaluation.

## Project Contents

### 1. Data Preprocessing and Transformation
- **Objective:** Prepare a clean dataset by handling missing values, normalizing numerical features, and encoding categorical variables.
- **Key Steps:**
  - Address missing data using mean imputation for numeric features.
  - Encode categorical variables (e.g., `OneHotEncoder` for nominal data).
  - Normalize continuous features to standardize scales and prevent any single feature from dominating.

### 2. Feature Engineering and Selection
- Used Logistic Regression, K-Nearest Neighbors, Decision Trees, Random Forest and XGBoost models to identify the most predictive features, focusing on critical indicators such as loan grade, home ownership status, and financial burden.
- After performing **SMOTE** to balance the dataset, feature importance was re-evaluated to enhance model interpretability and efficiency.

### 3. Model Training and Evaluation
- **Models trained:**
  - **Logistic Regression:** Baseline model for simple interpretation.
  - **K-Nearest Neighbors (KNN):** Used for non-linear boundary detection.
  - **Decision Trees** and **Random Forest:** To capture complex, non-linear interactions.
  - **XGBoost:** Primary model due to its robustness in handling imbalanced data.
- **Evaluation Metrics:** AUC-ROC, F1 Score, Precision, and Recall.

### 4. Key Findings
- **XGBoost** demonstrated the highest performance with an AUC of 0.94, balancing recall and precision effectively.
- Feature importance highlighted **loan grade** and **home ownership** as critical risk indicators.

## 5. Figures
- **Figure 1:** ROC Curve Comparison for Model Performance
![ROC Curve Comparison for Model Performance](https://github.com/LinZhou606/Credit-Default-Prediction-Using-Machine-Learning-Models/blob/main/ROC%20Curve%20Comparison%20for%20Model%20Performance.png)

- **Figure 2:** Confusion Matrix for XGBoost Model
![Confusion Matrix for XGBoost Model](https://github.com/LinZhou606/Credit-Default-Prediction-Using-Machine-Learning-Models/blob/main/Confusion%20Matrix%20for%20XGBoost%20Model.png)

## 6. Key Technologies Used
- **Python Libraries:** scikit-learn, pandas, NumPy
- **Tools:** Jupyter Notebook, Colab
