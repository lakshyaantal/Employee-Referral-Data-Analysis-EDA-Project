# Employee-Referral-Data-Analysis-EDA-Project
Project Objective
The objective of this analysis is to predict whether a referred candidate will join the organization or not. The goal is to identify key parameters that influence the decision of referred candidates to join, helping HR teams optimize recruitment strategies and referral programs.

📁 Dataset Overview
File Name: Referral_Join_Prediction.csv

Total Records: 499

Features: 19 (both independent and dependent)

Target Variable: referral_status – whether the referral joined or not

🔍 End-to-End Exploratory Data Analysis (EDA)
1. 📦 Data Loading
Imported essential libraries: numpy, pandas, matplotlib, seaborn.

Loaded the CSV into a Pandas DataFrame.

Performed .head(), .tail(), .shape, .info(), .describe() to understand the basic structure and types.

2. 📊 Data Inspection & Quality Checks
Identified issues:

Missing values in columns like referral_exp_in_years, referral_current_salary, referral_10_th_marks, etc.

Data type mismatches: numerical fields stored as object due to invalid characters (?).

Invalid entries like -1 in marks columns.

3. 🧹 Data Cleaning & Preprocessing
Replaced "?" with NaN and converted affected columns to appropriate data types.

Imputed missing values using mean/median where appropriate.

Treated anomalous entries (e.g., replaced -1 values in marks columns with appropriate estimates).

Checked for duplicates and removed if any.

4. 📈 Univariate Analysis
Distribution plots for numerical features (salary, marks, scores).

Count plots for categorical features (education level, gender, domain).

Analyzed skewness, outliers, and overall spread of data.

5. 📊 Bivariate Analysis
Examined relationships between key features and the target (referral_status):

Candidates with higher post-grad and graduation marks were more likely to join.

Salary expectations and academic performance played a crucial role in join decisions.

Domain-specific trends were observed.

6. 🧠 Insights from the Data
Education matters: Higher education scores (10th, 12th, Graduation, Post-Grad) are positively correlated with the likelihood of joining.

Salary expectations vs. Offer: Referral candidates are more likely to join when offered salaries closer to or higher than their current salaries.

Reasoning & Numerical aptitude scores also showed mild influence on the joining decision.

Work experience had moderate correlation – experienced candidates seemed more likely to accept offers.

Gender and domain had minimal direct impact.

💡 Tools and Libraries Used
Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook


 Next Steps (Optional)
Feature engineering for ML modeling

Building a logistic regression or decision tree model for prediction

Dashboarding in Power BI or Tableau

