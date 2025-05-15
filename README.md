# Student Performance Analysis

## Project Overview
This Jupyter notebook analyzes a student grading dataset to explore academic performance patterns, validate data integrity, and build a predictive model. The analysis includes data exploration, outlier detection, statistical testing, and machine learning using LightGBM.

## Dataset
**File:** `Students_Grading_Dataset.csv`  
**Features (23 columns):**
- Student metadata: `Student_ID`, `First_Name`, `Last_Name`, `Email`, `Gender`, `Age`, `Department`
- Academic metrics: `Attendance (%)`, `Midterm_Score`, `Final_Score`, `Assignments_Avg`, `Quizzes_Avg`, `Participation_Score`, `Projects_Score`, `Total_Score`, `Grade`
- Lifestyle factors: `Study_Hours_per_Week`, `Extracurricular_Activities`, `Internet_Access_at_Home`, `Parent_Education_Level`, `Family_Income_Level`, `Stress_Level (1-10)`, `Sleep_Hours_per_Night`

## Key Steps
1. **Data Exploration**  
   - Checked data structure, missing values, and unique counts.
   - Identified missing values in `Attendance (%)`, `Assignments_Avg`, and `Parent_Education_Level`.

2. **Data Integrity & Consistency**  
   - Validated grade assignments against total scores.
   - Detected outliers in features like `Study_Hours_per_Week` using box plots.

3. **Statistical Analysis**  
   - Performed t-tests, ANOVA, and chi-square tests to analyze relationships between variables (e.g., gender vs. scores, stress levels vs. grades).

4. **Predictive Modeling**  
   - Built a LightGBM regression model to predict `Total_Score`.
   - Achieved an **RMSE of 5.23** on the test set.

## Usage
### Dependencies
- Python 3.7+
- Libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`, `lightgbm`, `scipy`

### Installation
```bash
pip install pandas numpy seaborn matplotlib scikit-learn lightgbm scipy
