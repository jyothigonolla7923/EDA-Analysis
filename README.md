# Titanic Dataset - Exploratory Data Analysis (EDA)

This repository contains a Jupyter Notebook that explores and analyzes the Titanic dataset from Kaggle using Python. The goal is to understand the data, identify patterns related to survival, and prepare for future modeling.

## 📁 Dataset

- Source: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data?select=train.csv&utm_source=chatgpt.com)
- File used: `train.csv`

## 📊 What This EDA Covers

The `EDA.ipynb` notebook includes:

### ✅ Data Loading & Setup
- Imported essential libraries: `pandas`, `numpy`, `matplotlib.pyplot`, `seaborn`
- Loaded the dataset using `pd.read_csv()`
- Displayed dataset shape, info, and first few rows using:
  - `df.shape`
  - `df.info()`
  - `df.head()`

### ✅ Missing Data Analysis
- Used `isnull().sum()` to identify missing values
- Visualized missing data using:
  - `sns.heatmap()` for null value distribution

### ✅ Univariate Analysis
- Count plots for categorical features like:
  - `Sex`
  - `Pclass`
  - `Embarked`
  - `Survived`
- Distribution plots for numerical features like:
  - `Age`
  - `Fare`
  - Used `sns.histplot()` and `sns.boxplot()`

### ✅ Bivariate Analysis
- Analyzed survival rate against features:
  - `Sex` vs `Survived` (countplot & percentages)
  - `Pclass` vs `Survived`
  - `Age` distribution with survival overlay
- Grouped data to explore patterns:
  - `df.groupby(['Sex', 'Survived'])`


### ✅ Correlation & Heatmap
- Generated correlation matrix with `df.corr()`
- Visualized it using `sns.heatmap()`

---


