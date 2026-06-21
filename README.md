# ❤️ Cardiovascular Risk Prediction using Machine Learning

Predicting the **10-year risk of Coronary Heart Disease (CHD)** using machine learning techniques based on the Framingham Heart Study dataset.

## 📌 Project Overview

Cardiovascular diseases are among the leading causes of death worldwide. Early identification of high-risk individuals can help healthcare providers take preventive measures and improve patient outcomes.

This project leverages machine learning algorithms to predict whether a person is at risk of developing **Coronary Heart Disease (CHD)** within the next 10 years.

---

## 🎯 Problem Statement

Develop a machine learning model capable of predicting the 10-year risk of Coronary Heart Disease (CHD) using demographic, behavioral, and medical attributes collected from the Framingham Heart Study.

---

## 📂 Dataset

- **Source:** Framingham Heart Study
- **Rows:** 3,390
- **Columns:** 17
- **Target Variable:** `TenYearCHD`
  - 0 → No Risk
  - 1 → Risk of CHD

### Features Include

- Age
- Sex
- Education
- Smoking Status
- Cigarettes Per Day
- Blood Pressure Medication
- Stroke History
- Hypertension
- Diabetes
- Cholesterol Level
- Systolic Blood Pressure
- Diastolic Blood Pressure
- BMI
- Heart Rate
- Glucose Level

---

## 🔍 Exploratory Data Analysis

Performed extensive EDA with:

- Distribution Analysis
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis
- Outlier Detection
- Correlation Analysis
- Feature Relationships
- Class Imbalance Visualization

More than **15 visualizations** were created using:

- Matplotlib
- Seaborn

---

## 🛠 Data Preprocessing

### Missing Value Handling

- Median Imputation
- Mode Imputation
- KNN Imputation

### Outlier Treatment

- Interquartile Range (IQR) Method

### Feature Engineering

Created a new feature:

```python
Pulse Pressure = Systolic BP − Diastolic BP
```

### Multicollinearity Removal

- Variance Inflation Factor (VIF)

### Data Scaling

- StandardScaler

### Handling Imbalanced Dataset

- SMOTE
- SMOTE + Tomek Links

---

## 🤖 Machine Learning Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
- XGBoost Classifier
- Multi-layer Perceptron (Neural Network)

---

## ⚙ Hyperparameter Tuning

Performed using:

- GridSearchCV
- RandomizedSearchCV
- Cross Validation
- Repeated Stratified K-Fold

---

## 📊 Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

### Priority Metric: Recall

Since failing to identify high-risk patients can have serious consequences, **Recall** was prioritized to minimize false negatives.

---

## 🏆 Best Model

After evaluating multiple models, the **Tuned Neural Network (MLPClassifier)** achieved the best performance with the highest recall score and was selected as the final model.

---

## 📈 Libraries Used

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
xgboost
warnings
datetime
```

---

## 📁 Project Structure

```
cardiovascular-risk-prediction-using-ml-model
│
├── cardiovascular_risk_prediction_ml_project.ipynb
├── data_cardiovascular_risk.csv
├── README.md
└── images/
```

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/hussainaarish7/cardiovascular-risk-prediction-uisng-ml-model.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
cardiovascular_risk_prediction_ml_project.ipynb
```

---

## 📌 Key Insights

- Older individuals are at higher risk of CHD.
- Smoking significantly increases cardiovascular risk.
- High cholesterol and elevated BMI are associated with increased CHD risk.
- Diabetes and hypertension are major contributing factors.
- Addressing class imbalance improved model performance.

---

## 💡 Future Improvements

- Deploy model using Streamlit or Flask.
- Save trained model using Pickle.
- Build an interactive web application.
- Integrate SHAP for model explainability.
- Experiment with deep learning approaches.

---

## 👨‍💻 Author

**Mohd Aarish**

📧 Email: hussainaarish7@gmail.com

🔗 GitHub: https://github.com/hussainaarish7

---

## ⭐ If you found this project useful, don't forget to star the repository!
