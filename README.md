# ❤️ CodeAlpha – Heart Disease Prediction

## 📌 Overview
This project was developed as part of my **Machine Learning Internship at CodeAlpha**.  
The goal is to predict whether a patient is at risk of heart disease using clinical and demographic data.  
By leveraging **machine learning classification models**, healthcare professionals can make early, informed decisions and improve patient outcomes.



## 🎯 Objectives
- Use the **Cleveland Heart Disease dataset (UCI)** to build a predictive model.
- Explore and preprocess the dataset to handle missing values and categorical features.
- Train and evaluate multiple classification models to identify the best performer.
- Save and share the cleaned dataset for reproducibility.



## 🗂 Dataset
**Source:** [UCI Machine Learning Repository – Heart Disease Data](https://archive.ics.uci.edu/ml/datasets/heart+Disease)  
- **Rows:** 303 (after cleaning: fewer due to missing value removal)  
- **Target Variable:** `target` (0 = no disease, 1 = disease)  
- **Features:**
  - `age` – Age of patient  
  - `sex` – Gender (1 = male, 0 = female)  
  - `cp` – Chest pain type  
  - `trestbps` – Resting blood pressure  
  - `chol` – Serum cholesterol (mg/dl)  
  - `fbs` – Fasting blood sugar (> 120 mg/dl)  
  - `restecg` – Resting electrocardiographic results  
  - `thalach` – Maximum heart rate achieved  
  - `exang` – Exercise induced angina  
  - `oldpeak` – Depression induced by exercise  
  - `slope` – Slope of peak exercise ST segment  
  - `ca` – Number of major vessels colored by fluoroscopy  
  - `thal` – Thalassemia type



## 🛠 Tools & Technologies
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Models:** RandomForestClassifier, LogisticRegression  
- **IDE/Platform:** Google Colab  



## 📊 Data Preprocessing
1. Load dataset from UCI repository.
2. Replace `?` with NaN.
3. Convert categorical features to numeric.
4. Drop rows with missing values (small dataset).
5. Encode categorical features using one-hot encoding.

---

## 🔍 Exploratory Data Analysis (EDA)
- Class distribution visualization.
- Correlation heatmap for feature importance.
- Summary statistics to understand feature ranges.



## 🤖 Model Training
**Models Used:**
- **RandomForestClassifier** – Performed best with ~85% accuracy and high ROC-AUC.
- **LogisticRegression** – Simpler, interpretable model for baseline comparison.

**Metrics Evaluated:**
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix


## 📈 Results
| Model               | Accuracy | ROC-AUC |
|---------------------|----------|---------|
| Random Forest       | ~85%     | High    |
| Logistic Regression | ~82%     | Good    |
