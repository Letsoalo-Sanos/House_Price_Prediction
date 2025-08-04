# Data Preprocessing for Customer Churn Analysis

## Features

- Loading and displaying customer data
- Checking for missing values and duplicates
- Performing basic statistical analysis
- Visualizing customer churn based on various factors

## Requirements

To run this notebook, you need the following Python libraries:

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`

---

## Data Preprocessing

Steps included:

- Handling categorical variables using One-Hot Encoding
- Dealing with missing or inconsistent values (if any)
- Label encoding for binary yes/no features

---

## Exploratory Data Analysis (EDA)

- Univariate and bivariate analysis using Seaborn and Matplotlib
- Box plots, histograms, KDE plots

---

## Usage

- Load the dataset using pd.read_csv().
- Use df.head() and df.tail() to view the first and last few records.
- Check for missing values with df.isnull().sum().
- Perform statistical analysis using df.describe() and df.info().

## Visualizations

- Churn Count: A count plot visualizing the number of customers who churned versus those who stayed.
- Churn by Gender: A count plot showing churn rates categorized by gender.
- Churn by Geography: A count plot visualizing churn rates based on geographic location.
- Age Distribution by Churn: A kernel density estimate plot showing age distribution for churned and non-churned customers.
