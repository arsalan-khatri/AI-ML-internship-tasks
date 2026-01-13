# Task 1: Iris Flower Data Analysis & Visualization 🌸

## 📌 Project Overview
This project is part of my AI/ML Internship (Task 1). The objective is to perform **Exploratory Data Analysis (EDA)** on the famous **Iris Dataset**. The analysis helps in understanding the underlying structure of the data, detecting outliers, and visualizing relationships between features like Sepal Length and Sepal Width.

**Notebook File:** [task1.ipynb](task1.ipynb)

## 📂 Dataset Details
- **Dataset Name:** Iris Dataset (Loaded via Seaborn)
- **Total Records:** 150 Rows, 5 Columns
- **Features:**
  - `sepal_length`
  - `sepal_width`
  - `petal_length`
  - `petal_width`
  - `species` (Target Class: Setosa, Versicolor, Virginica)

## 🛠️ Tech Stack Used
- **Python**: Core programming language.
- **Pandas**: For data loading, inspection, and statistical summary.
- **Seaborn & Matplotlib**: For data visualization (Scatter plots, Box plots, Histograms).

## ⚙️ Key Steps Performed
In this notebook, I executed the following Data Analysis steps:

### 1. Data Loading & Understanding
- Loaded the dataset utilizing `sns.load_dataset('iris')`.
- Verified the data dimensions using `.shape` (Result: **150 rows, 5 cols**).
- Inspected the first few records using `.head()`.

### 2. Statistical Analysis
- Generated summary statistics (Mean, Std, Min, Max) using `df.describe()`.
- Checked for missing values and data types using `df.info()`.
- **Result:** No null values found; data is clean.

### 3. Data Visualization (EDA)
I created the following plots to analyze the data:

- **Scatter Plot:** Analyzed the relationship between `Sepal Length` and `Sepal Width`, colored by Species. This showed clear clustering of different species.
- **Histograms:** visualized the frequency distribution of all features.
- **Box Plots:** Used to detect outliers in the dataset.

## 📊 Visual Insights
*(Note: These are descriptions of the generated plots)*
1. **Correlation:** The Scatter plot reveals that specific species (like *Setosa*) are easily separable based on sepal dimensions.
2. **Outliers:** The Box plot analysis helps identify slight outliers in the `sepal_width` feature.
