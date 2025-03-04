# School Performance Analysis 📊

## Overview
This project involved analyzing school performance based on academic scores (math and reading), school spending, school size, and type. The goal was to understand the factors influencing student performance and surface insights that could help improve educational strategies. The analysis was performed independently, using SQL, Python (Pandas), and Excel to clean, manipulate, and visualize data, ultimately leading to actionable recommendations for administrators and policymakers.

## Data Acquisition
The dataset was sourced from multiple school performance databases containing variables like student scores, school budgets, enrollment, and more. Data was integrated into a single comprehensive dataset through the merging of school and student data using Python’s Pandas library.
``` python
school_data_complete = pd.merge(student_data, school_data, how="left", on=["school_name", "school_name"])
```
This allowes us to perform cross-analysis between various factors affecting performance, such as spending and school size.

## Data Preparation
### Data Cleaning
* **Handling Missing Values**: Missing values were identified and addressed by either imputing with the mean/median or excluding incomplete data where necessary to maintain integrity.
* **Data Transformation**: School-related metrics like budget and enrollment were normalized and categorized to allow easy comparison across school types.
### Data Manipulation
* Aggregate Metrics
* Per-School Analysis
* Passing Rates by School

## Data Analytics
With the data cleaned and manipulated, I used advanced analytics to extract key insights
### Key Findings:
1. Overall Performance:
* The overall passing rate for math and reading combined is **65.17%**, which indicates that a significant portion of students is struggling to meet the passing criteria in both subjects.
* **74.98%** of students passed math, while 85.81% passed reading. This suggests that students generally perform better in reading compared to math, and that more support and resources on math may be necessary to improve student outcomes in that subject.
2. School Spending:
* A **positive correlation** was found between **school spending** and **student performance**, especially in math scores. This implies that schools with higher budgets tend to have better performance in math, possibly due to more resources available for educational tools, extracurricular activities, and teacher development.
* This suggests that more funding can improve the learning environment and student opportunities, but other factors like teaching quality and student backgrounds also play a role.
3. School Size:
* 
