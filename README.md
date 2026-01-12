# 🚀 AI & Machine Learning Internship Tasks

Welcome to my AI/ML Internship repository! This collection features three key projects focusing on Data Analysis, Time Series Forecasting, and Medical Diagnostic Classification. These tasks demonstrate my proficiency in Python, Data Visualization, and Scikit-Learn.

---

## 👨‍💻 Author
**Arsalan Khatri** *Founder, AK Deep Knowledge* *BS(AI) Graduate & Developer*

---

## 📂 Table of Contents
1. [Task 1: Iris Dataset Exploration](#task-1-exploring-and-visualizing-a-simple-dataset)
2. [Task 2: Stock Price Prediction](#task-2-predict-future-stock-prices-short-term)
3. [Task 3: Heart Disease Prediction](#task-3-heart-disease-prediction)

---

## 📊 Task 1: Exploring and Visualizing a Simple Dataset

### 🎯 Objective
To load, inspect, and visualize the classic Iris dataset to understand underlying data trends, feature distributions, and potential outliers.

### 🛠️ Tech Stack
* **Libraries:** `Pandas`, `Matplotlib`, `Seaborn`
* **Dataset:** Iris Dataset (CSV)

### 📝 Key Steps Implemented
1.  **Data Loading:** Loaded the dataset using Pandas and inspected structure using `.shape`, `.head()`, and `.info()`.
2.  **Statistical Summary:** Used `.describe()` to analyze mean, standard deviation, and quartiles.
3.  **Visualization:**
    * **Scatter Plots:** To observe relationships between Sepal/Petal dimensions.
    * **Histograms:** To visualize the distribution of values across classes.
    * **Box Plots:** To identify outliers in the dataset.

---

## 📈 Task 2: Predict Future Stock Prices (Short-Term)

### 🎯 Objective
To build a regression model that predicts the next day's closing price of a stock based on historical market data.

### 🛠️ Tech Stack
* **Libraries:** `yfinance`, `Pandas`, `Scikit-Learn`, `Matplotlib`
* **Model:** Linear Regression / Random Forest
* **Dataset:** Real-time data fetched via Yahoo Finance API (e.g., Apple/Tesla)

### 📝 Key Steps Implemented
1.  **Data Fetching:** Retrieved historical stock data using the `yfinance` API.
2.  **Feature Engineering:** Used features like `Open`, `High`, `Low`, and `Volume` to predict the target `Close` price.
3.  **Model Training:** Trained the model on historical trends.
4.  **Evaluation:** Plotted **Actual vs. Predicted** prices to visualize the model's accuracy on unseen data.

---

## 🩺 Task 3: Heart Disease Prediction

### 🎯 Objective
To develop a binary classification model that assesses whether a person is at risk of heart disease based on medical indicators.

### 🛠️ Tech Stack
* **Libraries:** `Pandas`, `Scikit-Learn`, `Seaborn`
* **Model:** Logistic Regression / Decision Tree Classifier
* **Dataset:** Heart Disease UCI Dataset (Kaggle)

### 📝 Key Steps Implemented
1.  **Data Cleaning:** Handled missing values and preprocessed the data.
2.  **Exploratory Data Analysis (EDA):** Analyzed correlations between age, cholesterol levels, and heart disease risk.
3.  **Modeling:** Trained a classification model to predict risk (1 = Risk, 0 = No Risk).
4.  **Evaluation Metrics:**
    * **Accuracy Score**
    * **Confusion Matrix:** To minimize false negatives.
    * **ROC Curve:** To check model performance thresholds.

---

## ⚙️ How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/arsalan-khatri/AI-ML-Internship-Tasks.git](https://github.com/arsalan-khatri/AI-ML-Internship-Tasks.git)
