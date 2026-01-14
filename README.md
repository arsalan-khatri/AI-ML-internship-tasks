# AI & Machine Learning Internship Portfolio
[DevelopersHub Corporation©](https://www.linkedin.com/company/developershub-corporation)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## Overview
Welcome to my AI/ML Internship repository! This collection showcases three distinct projects ranging from **Exploratory Data Analysis (EDA)** to **Predictive Modeling** using Regression and Classification algorithms. 

The goal of these tasks was to solve real-world problems by applying data science techniques, data visualization, and machine learning model deployment.

## Tech Stack Used
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Joblib
- **Tools:** Jupyter Notebook

---

## Project Highlights

| # | Project Name | Domain | Description | Key Result | Link |
|:--:|:---|:---|:---|:---|:--:|
| **1** | **Iris Flower Analysis** | **EDA & Viz** | A deep dive into the Iris dataset to understand feature distributions and species clustering using visualizations. | Identified clear linear separability in Setosa species. | [Task 1](./task1) |
| **2** | **Stock Price Prediction** | **Regression** | Built a model to forecast Apple (AAPL) stock prices based on 5 years of historical data using Linear Regression. | Achieved **97.15%** Accuracy. | [Task 2](./task2) |
| **3** | **Heart Disease Prediction** | **Classification** | Developed a "Doctor AI" system to detect heart disease risk based on patient vitals using Random Forest. | Achieved **88.52%** Accuracy with high recall. | [Task 3](./task3) |

---

## Detailed Summaries

### Task 1: Iris Data Analysis
* **Objective:** Perform EDA to detect outliers and feature correlations.
* **Technique:** Used Box plots, Histograms, and Scatter plots.
* **Insight:** Detected outliers in `sepal_width` and confirmed that petal dimensions are the strongest differentiators between species.

### Task 2: Stock Market Forecasting
* **Objective:** Predict the *Next Day's* closing price.
* **Technique:** Linear Regression with Time-Series splitting (`shuffle=False`).
* **Feature Engineering:** Created Moving Averages (MA50) and Lag features (`shift(-1)`).
* **Visualization:** Plotted actual vs. predicted trends to validate model performance.

### Task 3: Heart Disease Classification ("Doctor AI")
* **Objective:** Classify patients as Healthy or At-Risk.
* **Technique:** Random Forest Classifier with stratified splitting.
* **Feature:** Built a custom function `check_patient()` that simulates a doctor's report, providing a risk percentage for individual patients.

---

## How to Run Locally
1. **Clone the repository:**
   ```bash
   git clone https://github.com/arsalan-khatri/AI-ML-internship-tasks.git
