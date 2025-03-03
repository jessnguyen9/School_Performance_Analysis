# School Performance Analysis 📊

## Overview
This project involved analyzing school performance based on academic scores (math and reading), school spending, school size, and type. The goal was to understand the factors influencing student performance and surface insights that could help improve educational strategies. The analysis was performed independently, using SQL, Python (Pandas), and Excel to clean, manipulate, and visualize data, ultimately leading to actionable recommendations for administrators and policymakers.

## Data Acquisition
The dataset was sourced from multiple school performance databases containing variables like student scores, school budgets, enrollment, and more. Data was integrated into a single comprehensive dataset through the merging of school and student data using Python’s Pandas library.
``` python
school_data_complete = pd.merge(student_data, school_data, how="left", on=["school_name", "school_name"])

## Data Preparation
### Data Cleaning
