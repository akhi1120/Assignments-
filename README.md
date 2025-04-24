# Titanic Dataset - Data Cleaning & Preprocessing 🚢

This repository contains the solution for **Task 1** of the AI & ML Internship program, focused on data cleaning and preprocessing using the Titanic dataset.

---

## 📁 Dataset
- **Source**: [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- **File Used**: Titanic-Dataset.csv

---

## 🔧 Tools & Libraries
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

---

## ✅ What I Did

### 1. Data Exploration
- Loaded the dataset using Pandas.
- Used `.info()` and `.describe()` to explore basic data statistics.
- Identified missing values in `Age`, `Cabin`, and `Embarked`.

### 2. Handling Missing Values
- **Age**: Filled missing values with the **median**.
- **Embarked**: Filled with the **mode** (most frequent value).
- **Cabin**: Dropped due to excessive missing data.

### 3. Categorical Encoding
- Converted `Sex` and `Embarked` using **One-Hot Encoding** (`drop_first=True` to avoid dummy variable trap).

### 4. Feature Scaling
- Selected numerical columns: `Age`, `Fare`, `SibSp`, `Parch`.
- Standardized them using **StandardScaler** from Scikit-learn.

### 5. Outlier Detection & Removal
- Visualized outliers using **Boxplots**.
- Removed outliers using the **IQR (Interquartile Range)** method.
- Checked dataset shape before and after — no rows removed, which means no extreme outliers were present after scaling.

---

## 🧠 Learnings
- Handling missing data with appropriate statistical techniques.
- One-hot encoding for categorical variables.
- Standardization for numerical features.
- Outlier detection using IQR method.
- Clean preprocessing pipeline for machine learning readiness.

---

## 📦 Output
- Preprocessed dataset saved as "Titanic-Dataset.csv".
- Jupyter Notebook: `Titanic_datacleaning_preprocessing.ipynb`

---

## 🚀 Author
- Done by me as part of my learning journey during the AI & ML Internship 🚀
