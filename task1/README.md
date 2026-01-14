# Task 1: Iris Dataset Exploratory Analysis

## 1. Task Objective
The objective of this task was to perform **Exploratory Data Analysis (EDA)** on the Iris dataset. The goal was to understand the structure of the data, identify the distribution of features (Sepal/Petal dimensions), detect outliers, and visualize the relationships between different flower species before applying any Machine Learning models.

## 2. Dataset Used
- **Dataset Name:** Iris Dataset (loaded via Seaborn)
- **Dimensions:** 150 Rows, 5 Columns
- **Features:**
  1. `sepal_length`
  2. `sepal_width`
  3. `petal_length`
  4. `petal_width`
  5. `species` (Target: Setosa, Versicolor, Virginica)

## 3. Methodologies Applied
Since this is the analysis phase, the following techniques were used instead of predictive modeling:

* **Data Inspection:** Used `.shape`, `.head()`, and `.info()` to check data structure and types.
* **Statistical Summary:** Used `.describe()` to check mean, standard deviation, and quartiles.
* **Data Visualization (Seaborn & Matplotlib):**
    * **Scatter Plots:** To observe clustering between species based on Sepal dimensions.
    * **Histograms:** To view the frequency distribution of data.
    * **Box Plots:** To identify outliers in the dataset.

## 4. Key Results and Findings
* **Data Quality:** The dataset is clean with **no null values** and contains 150 records.
* **Species Separation:** The Scatter Plot reveals that the **Setosa** species is linearly separable from the other two species (Versicolor and Virginica), making it easy to classify.
* **Outliers Detected:** The Box Plot analysis showed some outliers present in the `sepal_width` feature.
* **Feature Distribution:** The histograms indicate distinct distributions for petal lengths, suggesting that petal features are very important for classification.
