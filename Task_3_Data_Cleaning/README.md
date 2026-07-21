# 🧹 Task 3: Data Cleaning & Pre-processing Pipeline

**Internship Program:** Oasis Infobyte (OIBSIP)  
**Track:** Data Analytics

---

## 🎯 Project Objective

The objective of this project is to build a robust data cleaning and preprocessing pipeline using the Titanic dataset. The project focuses on improving data quality by handling missing values, removing duplicate records, standardizing data formats, and treating outliers to prepare the dataset for Exploratory Data Analysis (EDA) and Machine Learning applications.

---

## 📂 Dataset

- **Dataset:** Titanic Dataset
- **Records:** 1,309
- **Features:** 14

---

## 🛠️ Data Cleaning Workflow

### ✅ Initial Data Quality Assessment
- Examined dataset structure
- Identified missing values
- Checked duplicate records
- Verified data types

### ✅ Duplicate Removal
- Removed **107 duplicate records** to improve data consistency.

### ✅ Missing Value Handling
- Filled missing values in the **Age** column using the median.
- Filled missing values in the **Embarked** column using the mode.
- Removed the **Deck** column due to a high percentage of missing values (>77%).

### ✅ Data Standardisation
- Converted text columns to lowercase.
- Standardized categorical values.
- Converted appropriate columns to categorical data types.

### ✅ Outlier Detection & Treatment
- Detected outliers using the **Interquartile Range (IQR)** method.
- Visualized outliers using boxplots.
- Capped extreme values in the **Fare** column to reduce the impact of outliers.

---

## 📈 Final Outcome

After preprocessing, the dataset became:

- ✅ Free from duplicate records
- ✅ Missing values handled appropriately
- ✅ Standardised and consistent
- ✅ Outliers detected and treated
- ✅ Ready for Exploratory Data Analysis (EDA) and Machine Learning

---

## 📁 Repository Contents

- `Task_3_Data_Cleaning_Oasis.ipynb` – Complete data cleaning notebook
- `titanic_raw.csv` – Original dataset
- `titanic_cleaned.csv` – Cleaned dataset
- `README.md`

---

## 💻 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## 📚 Key Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Missing Value Handling
- Duplicate Detection & Removal
- Data Standardisation
- Outlier Detection & Treatment
- Data Validation
- Exploratory Data Analysis (EDA) Preparation

---

## 📌 Conclusion

This project demonstrates a complete data cleaning and preprocessing workflow by transforming a raw dataset into a structured, consistent, and analysis-ready dataset. The final cleaned data can be confidently used for further exploratory analysis, visualization, and predictive modeling.
