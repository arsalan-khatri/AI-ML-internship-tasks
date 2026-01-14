# Task 3: Heart Disease Prediction & Classification

## 1. Task Objective
The primary objective of this project was to build a machine learning model to predict the presence of **heart disease** in patients based on various medical attributes. This system is designed to assist in early diagnosis and risk assessment.
- Analyze key risk factors (Age, Cholesterol, Chest Pain, etc.).
- Build a classification model to distinguish between healthy patients and those with heart disease.
- Deploy a simple prediction function ("Doctor AI") for real-time risk assessment.

## 2. Dataset Used
- **Source:** [UCI Machine Learning Repository - Cleveland Heart Disease Data](https://archive.ics.uci.edu/dataset/45/heart+disease).
- **Data Shape:** 303 Rows, 14 Columns.
- **Target Variable:** `target` (0 = Healthy, 1 = Disease Detected).
- **Key Features:**
  - `age`: Age of the patient.
  - `sex`: Gender (1 = Male, 0 = Female).
  - `cp`: Chest Pain Type (1-4).
  - `trestbps`: Resting Blood Pressure.
  - `chol`: Serum Cholesterol.
  - `thalach`: Maximum Heart Rate Achieved.
  - `exang`: Exercise Induced Angina.

## 3. Models Applied
I utilized the **Random Forest Classifier** for this task because of its ability to handle non-linear relationships and reduced risk of overfitting compared to single Decision Trees.

- **Algorithm:** `RandomForestClassifier` (Scikit-Learn).
- **Hyperparameters:** `n_estimators=100`, `random_state=42`.
- **Training Strategy:**
  - **Stratified Split:** Used to maintain the proportion of healthy vs. sick patients in both training and test sets.
  - **Data Cleaning:** Handled missing values (marked as `?`) by imputing with the mode.

## 4. Key Results and Findings

### Performance
- **Model Accuracy:** **88.52%**.
- **Precision:** 0.84 for the Disease class (minimizing false alarms).
- **Recall:** 0.93 for the Disease class (successfully detecting 93% of actual heart patients).

### Data Insights
- **Gender Risk:** The data showed a significant gender disparity: **55.34%** of men in the dataset had heart disease compared to **25.77%** of women.
- **Chest Pain (CP):** Asymptomatic chest pain (Type 4) was the strongest indicator, with a **72.92%** risk of disease.
- **Age:** Density plots revealed that the risk of heart disease increases significantly after the age of 50.

### "Doctor AI" Clinic Report
A custom function `check_patient()` was implemented to simulate real-world usage. It takes patient data and outputs a readable report.
> *Example:* ` DANGER! Heart disease risk detected. (Risk: 92.00%)`

### Model Saving
- The trained model is saved as `heart_doctor_model.pkl` using Joblib, making it ready for deployment in a web app or API.
