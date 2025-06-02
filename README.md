# Titanic-EDA-Internship-Task5
EDA of Titanic Dataset using Python libraries (Pandas, Numpy, Seaborn, and Matplotlib) to uncover survival patterns and trends. Internship Task 5.


# 🧠 Data Analyst Internship - Task 5: Exploratory Data Analysis (EDA)


## 🎯 Objective
To explore the Titanic dataset using Python libraries such as **Pandas**, **Matplotlib**, and **Seaborn**, and extract meaningful insights by identifying patterns, trends, and anomalies.

---

## 🛠 Tools and Libraries
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📊 Steps Performed

### ✅ Data Loading and Cleaning
- Loaded the dataset using Pandas.
- Checked for null values and data types using `.info()` and `.describe()`.
- Filled or handled missing values (e.g., in `Age`, `Embarked`).
- Dropped unnecessary columns like `Name`, `Ticket`, and `Cabin`.

### ✅ Univariate Analysis
- Analyzed individual features like `Age`, `Fare`, `Survived` using histograms and boxplots.
- Observed outliers in Fare and age distribution.

### ✅ Bivariate and Multivariate Analysis
- Plotted relationships using:
  - `sns.countplot()` for categorical vs target (`Sex`, `Pclass`)
  - `sns.violinplot()` for age distribution by survival
  - `sns.heatmap()` for correlation
  - `sns.pairplot()` for multivariate relationships

### ✅ Feature Engineering
- Created a new feature `FamilySize = SibSp + Parch + 1` to assess survival based on family size.

---

## 🔍 Key Observations

| Feature         | Insight |
|-----------------|---------|
| **Gender**      | Females had a significantly higher survival rate. |
| **Pclass**      | 1st class passengers survived more than 2nd and 3rd class. |
| **Fare**        | Higher fare correlated with higher survival (likely 1st class). |
| **Age**         | Young passengers (especially children) had slightly higher survival rates. |
| **FamilySize**  | Passengers with 2–4 family members had better chances of survival. |

---

## 📌 Summary of Findings

- **Social status, gender, and group size** were major factors in survival.
- **Age and Fare** showed some influence, but less predictive on their own.
- The dataset is **imbalanced** with more non-survivors than survivors.
- Multicollinearity was low; features had weak to moderate correlation.

---

🔗 Submission This repository contains:

- ✅ `Titanic_EDA.ipynb` (Jupyter Notebook with code and visualizations)
- ✅ `train.csv` (dataset)
- ✅ `README.md` (This file)
