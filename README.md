# Exploratory Data Analysis (EDA) – Code Alpha Internship (Task 2)

## Overview
This repository contains the code and analysis for **Task 2 of my Code Alpha Data Analyst Internship**, which focuses on performing **Exploratory Data Analysis (EDA)** on the `customer_data.csv` dataset.

The primary goals of this task were:
- To ask meaningful questions about the dataset before analysis.
- To explore the structure of the data (variables, data types, etc.).
- To identify trends, patterns, and anomalies.
- To test hypotheses and validate assumptions using statistical measures and visualization.
- To detect and address potential data issues.

## Dataset
The dataset `customer_data.csv` consists of **10,000 records** and **19 columns** related to customer and vehicle information.

### Key Columns:
- **Demographic attributes:** `age`, `gender`, `race`, `education`, `income`
- **Vehicle details:** `vehicle_type`, `vehicle_year`, `annual_mileage`
- **Behavioral data:** `speeding_violations`, `DUIs`, `past_accidents`
- **Target variable:** `outcome`

## Steps Performed

### 1. Data Loading
- Imported libraries such as `pandas` and `numpy`.
- Loaded the dataset using `pd.read_csv()`.

### 2. Data Exploration
- Checked dataset dimensions using `df.shape`.
- Reviewed column names and data types using `df.info()` and `df.columns`.
- Generated descriptive statistics using `df.describe()`.

### 3. Missing Values
- Identified missing values in `credit_score` and `annual_mileage` using `df.isna().sum()`.
- Imputed missing credit scores using group means based on the `income` category.

### 4. Trends & Patterns
- Observed the relationship between `income` classes and `credit_score` using group-by aggregation.
- Studied patterns of `speeding_violations` and `DUIs` in the dataset.

### 5. Data Cleaning
- Filled missing values using custom functions and logical grouping.
## Key Insights
- **Credit Score vs. Income:** Upper-class customers have higher average credit scores compared to other classes.
- **Driving Behavior:** Most customers have zero DUIs and past accidents, but outliers exist with high counts of speeding violations (up to 22).
- **Annual Mileage:** Most vehicles have annual mileage between 10,000 to 14,000 miles.

## How to Run
1. Clone this repository:
   git clone https://github.com/<your-username>/<repo-name>.git
2. Install dependencies:
   pip install pandas numpy matplotlib seaborn
   
3. Run the Jupyter Notebook or Python script to see the EDA process.

## Technologies Used
- **Python Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Python 3.x
## Acknowledgment
This project was completed as part of my **Code Alpha Data Analyst Internship** (Task 2).
I am grateful to **Code Alpha** for providing this opportunity and guidance.
