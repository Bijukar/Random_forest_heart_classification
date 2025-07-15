# 🫀 Heart Disease Prediction using Random Forest Classifier

This project uses a **Random Forest Classifier** to predict the presence of heart disease in patients based on their medical records. It includes Exploratory Data Analysis (EDA), preprocessing, hyperparameter tuning, ROC curve analysis, and feature importance visualization.

---

## 📁 Dataset

- **Source**: [Heart Disease UCI - Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci)
- **Target**: `target` (1 = heart disease, 0 = no disease)
- **Features**:
  - `age`, `sex`, `cp`, `trestbps`, `chol`, `fbs`, `restecg`, `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`

---

## 🔍 Exploratory Data Analysis (EDA)

- Checked for missing values and data types.
- Class distribution plot (`target`)

---

## 🧠 Model: Random Forest Classifier

- Used `RandomForestClassifier` from `sklearn.ensemble`
- Handled categorical features (`cp`, `thal`, `slope`) using **One-Hot Encoding**
- Split data: 80% train, 20% test
- Hyperparameter tuning using `GridSearchCV`

### ✅ Best Parameters Found

  -'n_estimators': 100,
  -'max_depth': None,
  -'max_features': 'sqrt',
  -'criterion': 'entropy'

### 📊 Visualizations

✅ Confusion Matrix

✅ Feature Importance Plot


### 💾 Save The Model 
- import joblib
- joblib.dump(best_model, "random_forest_model.joblib")

  ### 📂 Project Structure

- random_forest_classification.ipynb            # Jupyter Notebook with full project
- README.md                   # Project documentation
- requirements.txt            # Python package requirements (optional)
- random_forest_model.joblib          # Trained model (optional)
