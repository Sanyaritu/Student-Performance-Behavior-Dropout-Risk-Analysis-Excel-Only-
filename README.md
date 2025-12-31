# 📊 Student Performance Risk Analysis (Excel-Only Project)

## 📌 Overview
This project focuses on cleaning, preparing, and engineering features from a **real-world unclean student performance dataset** using **Microsoft Excel only**.  
The goal was to transform messy raw data into an **analysis-ready dataset** and build a **rule-based risk classification model** without using Python, SQL, or any external tools.

---

## 📂 Dataset
- **Source:** Kaggle (Dirty Student Performance Dataset)
- **Records:** ~10,000
- **Nature:** Unclean data with missing values, text-formatted numbers, and inconsistent entries

---

## 🧹 Data Cleaning & Preparation
The raw dataset required multiple preprocessing steps before it could be used for analysis.

### Key Cleaning Steps:
- Preserved original data in a `Raw_Data` sheet for reproducibility
- Converted numeric columns stored as text into proper numeric format
- Treated placeholder zeros and empty cells appropriately
- Imputed missing values:
  - Numeric fields → Median
  - Categorical fields → Mode
- Removed duplicate records
- Standardized column names and categories
- Validated numeric ranges for consistency
- Generated a stable `Row_ID` to ensure accurate record counting

All cleaning was performed using **helper columns** and finalized using **Paste as Values** to avoid formula dependencies.

---

## 🛠 Feature Engineering
After cleaning, additional features were created to enrich the dataset and support risk analysis.

### Engineered Features:
- **Performance_Band**
  - Categorizes students into: `Excellent`, `Good`, `Average`, `Poor`
  - Based on the existing `Performance_Index`

- **Risk_Score**
  - A numeric, rule-based score combining academic performance and study behavior
  - Higher score indicates higher academic risk

- **Risk_Category**
  - Derived from `Risk_Score`
  - Classifies students into:
    - `High Risk`
    - `Medium Risk`
    - `Low Risk`

These features simulate a **basic predictive model built entirely in Excel**.

---

## 🧠 Modeling Logic (Rule-Based)
Instead of machine learning, a transparent rule-based approach was used:

- Academic performance was treated as the primary indicator
- Behavioral factors (e.g., study hours) were incorporated into the risk score
- Clear thresholds were defined to ensure interpretability

This approach mirrors real-world scenarios where explainability is more important than model complexity.

---

## 📈 Final Output
The final dataset (`Featured_Engineering` sheet) is:
- Fully cleaned
- Free of duplicates and empty cells
- Enhanced with engineered features
- Ready for analysis, visualization, or dashboarding

---

## 🧰 Tools Used
- Microsoft Excel
  - Formulas
  - Helper columns
  - Data validation
  - Logical functions
  - Paste Special (Values)

---

## 🎯 Skills Demonstrated
- Data cleaning and preprocessing
- Handling messy real-world datasets
- Feature engineering
- Rule-based risk modeling
- Analytical thinking using Excel
- Documentation and reproducibility

---

## 📌 Notes
No Python, SQL, or BI tools were used in this project.  
All transformations and logic were implemented using Excel to demonstrate strong fundamentals in data handling and analysis.

---

## 📎 Files in Repository
- `student_performance_analysis.xlsx`
- `README.md`

