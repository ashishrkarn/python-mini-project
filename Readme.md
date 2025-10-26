# Healthcare Data Analysis – EDA in Python

## Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on a healthcare dataset consisting of 60,000 patient records. The goal is to clean, preprocess, and analyze patient, medical, and hospital information to uncover patterns in billing, demographics, stay durations, and treatment outcomes.

---

## Dataset Description

**File Name:** healthcare_dataset.csv  
**Size:** 60,000 rows × 15 columns

The dataset includes:

- **Demographic Info:** Name, Age, Gender, Blood Type
- **Medical Info:** Medical Condition, Medication, Test Results
- **Administrative Info:** Doctor, Hospital, Insurance Provider, Room Number, Admission Type
- **Time Data:** Date of Admission, Discharge Date
- **Financial Info:** Billing Amount

---

## Objectives

- Perform data profiling and cleaning.
- Handle missing, duplicate, and inconsistent data efficiently.
- Analyze distributions and relationships among hospital and patient variables.
- Generate powerful visual insights using Python’s visualization libraries.
- Classify new derived fields for analytic insights such as:
  - **Age Group (Young, Middle-aged, Senior)**
  - **High Billing (> ₹30,000)**
  - **Long Stay (> average duration)**
  - **Hospital Flag (Smith Affiliated)**

---

## Technologies Used

- **Language:** Python 3
- **Libraries:**
  - Data manipulation: `Pandas`, `NumPy`
  - Visualization: `Matplotlib`, `Seaborn`
  - Notebook environment: `Jupyter`

---

## Steps in Analysis

1. **Data Loading and Inspection**

   - Viewed structure, shape, and types.
   - Converted necessary columns to dates or categorical types.

2. **Data Cleaning**

   - Handled missing values in _Blood Type_, _Insurance Provider_, _Billing Amount_.
   - Removed duplicates using unique signatures.
   - Normalized inconsistent casing in _Name_ and _Hospital_ fields.

3. **Feature Engineering**

   - Created new columns: `Age_Group`, `Long_Stay`, `High_Bill`, and `has_smith_hospital`.
   - Converted Room Number to categorical for accurate analysis.

4. **Exploratory Analysis**

   - Descriptive statistics for numeric columns.
   - Visualized key patterns using histograms, KDE plots, heatmaps, pairplots, and boxplots.

5. **Categorical Relationships**
   - Compared Gender vs Medical Condition and Admission Type.
   - Used heatmaps to analyze Test Results by Medical Condition.

---

## Key Insights

- Dataset equally represents **Male (50.04%)** and **Female (49.96%)**.
- **Average Age:** 51.5 | **Avg Billing Amount:** ₹25,528 | **Avg Stay Duration:** 15.5 days.
- **Billing amounts** are evenly spread, showing fair pricing alignment between treatment types.
- **No major correlation** found among numerical features (Age, Billing, Stay Duration).
- About **4.3%** of patients are linked with hospitals containing “Smith” in their name.

---

## Visualizations Included

- Distribution of Age, Gender Pie Chart.
- KDE of Billing Amount and Boxplots by Admission Type & Condition.
- Heatmap of Test Results by Medical Condition.
- Pairplot of numerical values (Billing, Age).
- Trend line for Stay Duration across time (2019–2024).

---

## Conclusion

- The dataset is **balanced, clean, and highly suited for healthcare insight generation.**
- No significant bias detected in cost or test results across genders.
- Serves as a strong base for **predictive modeling or cost-optimization studies** in hospital management systems.

---

## Future Enhancements

- Implement predictive modeling on billing or stay duration using ML algorithms.
- Build interactive dashboards with **Plotly** or **Power BI**.
- Automate anomaly detection for irregular billing or extended stays.

---

**Author:** Group 8 – Healthcare Data Analytics (Python EDA Project)
