# EDA-project
# Adult Income Data Analysis — EDA Project

## 📌 Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of the Adult Income dataset using Python.

The main objective of this project is to understand the dataset, clean the data, identify patterns, handle missing values, and visualize relationships between different attributes such as age, education, occupation, working hours, gender, and income.

---

## 📊 Dataset

The dataset contains information about individuals and their demographic and employment characteristics.

### Dataset Size

* **Rows:** 32,561
* **Columns:** 15

### Main Features

| Column         | Description                           |
| -------------- | ------------------------------------- |
| Age            | Age of the individual                 |
| Workclass      | Type of employment                    |
| Final Weight   | Census sample weight                  |
| Education      | Education level                       |
| EducationNum   | Numerical representation of education |
| Marital Status | Marital status                        |
| Occupation     | Type of occupation                    |
| Relationship   | Relationship status                   |
| Race           | Race category                         |
| Gender         | Gender of the individual              |
| Capital Gain   | Capital gain                          |
| Capital Loss   | Capital loss                          |
| Hours per Week | Hours worked per week                 |
| Native Country | Country of origin                     |
| Income         | Income category                       |

---

## 🎯 Objectives

The main objectives of this project are:

* Understand the structure of the dataset
* Perform data cleaning
* Identify missing/null values
* Analyze numerical and categorical variables
* Detect and handle outliers
* Explore relationships between variables
* Create meaningful data visualizations
* Identify patterns related to income
* Perform Exploratory Data Analysis (EDA)

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab
* Jupyter Notebook

---

## 🔍 EDA Process

### 1. Data Loading

The dataset is loaded using Pandas.

```python
import pandas as pd

df = pd.read_csv("adult.csv")

print(df.head())
```

### 2. Understanding the Dataset

Basic dataset information was analyzed using:

```python
df.shape
df.info()
df.describe()
df.columns
```

### 3. Checking Missing Values

Missing/null values were identified using:

```python
df.isnull().sum()
```

### 4. Data Cleaning

The project includes data-cleaning techniques such as:

* Identifying NULL values
* Handling missing values
* Removing unnecessary records/columns when required
* Filling missing values
* Checking duplicate records
* Handling inconsistent data

### 5. Outlier Analysis

Outliers were explored using statistical techniques such as:

* IQR method
* Z-score analysis

Example:

```python
Q1 = df["Age"].quantile(0.25)
Q3 = df["Age"].quantile(0.75)

IQR = Q3 - Q1

print("Q1:", Q1)
print("Q3:", Q3)
print("IQR:", IQR)
```

---

## 📈 Data Visualization

Different charts were used to understand patterns in the dataset.

### Visualizations included

* Bar Chart
* Line Chart
* Area Chart
* Scatter Plot
* Histogram
* Box Plot
* Heatmap
* Stacked Plot

These visualizations help understand relationships between variables and identify trends and distributions.

---

## 📊 Example Analysis

Some of the questions explored in the analysis include:

* What is the distribution of age?
* Which education levels are most common?
* How are individuals distributed across workclasses?
* How many people belong to each income category?
* How does education relate to income?
* How do working hours vary among individuals?
* What is the relationship between age and income?
* How are different occupations distributed?
* Are there outliers in numerical variables?
* Which variables show noticeable relationships with income?

---

## 💡 Key Learning Outcomes

Through this project, I learned how to:

* Load and inspect a real-world dataset
* Perform data cleaning
* Identify and handle missing values
* Analyze numerical and categorical data
* Detect outliers
* Use Pandas for data analysis
* Use NumPy for numerical operations
* Create charts using Matplotlib and Seaborn
* Perform Exploratory Data Analysis
* Extract meaningful insights from data

---

## 📁 Project Structure

```text
Adult-Income-EDA/
│
├── adult.csv
├── Adult_Income_EDA.ipynb
└── README.md
```

---

## ▶️ How to Run the Project

### Using Google Colab

1. Open the `.ipynb` notebook.
2. Upload `adult.csv`.
3. Run the cells sequentially.
4. Check the generated analysis and visualizations.

### Using Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

Then open the notebook:

```bash
jupyter notebook
```

---

## 📌 Conclusion

This project demonstrates the complete **Exploratory Data Analysis process** on the Adult Income dataset, starting from data loading and understanding the data to cleaning, statistical analysis, outlier detection, and visualization.

The project helped me gain practical experience in using Python libraries for **Data Analysis and EDA**.

---

## 👩‍💻 Author

**Vasavi**

### Skills Demonstrated

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Data Analysis` `EDA`
