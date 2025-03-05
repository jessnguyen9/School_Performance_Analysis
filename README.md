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

![PASSING RATES BY SUBJECTS](https://github.com/user-attachments/assets/84ff5054-6f8d-4ccb-aa1e-2965b0a62319)
2. School Spending:
* A **positive correlation** was found between **school spending** and **student performance**, especially in math scores. This implies that schools with higher budgets tend to have better performance in math, possibly due to more resources available for educational tools, extracurricular activities, and teacher development.
* This suggests that more funding can improve the learning environment and student opportunities, but other factors like teaching quality and student backgrounds also play a role.
3. School Size:
* **Smaller** and **medium-sized** schools generally performed better than larger schools in both math and reading. This finding points to the potential advantages of smaller student-teacher ratios, where students may receive more personalized attention, fostering a more supportive and focused learning environment.
* Larger schools may have challenges with maintaining individual student engagement, which could contribute to lower overall performance.
  
![PERFORMANCE COMPARISON](https://github.com/user-attachments/assets/a23564e0-6fed-4de8-806c-b62911e544f8)
## Insights & Recommendations:
1. Targeted Funding:
* Schools with **lower passing rates**, particularly **larger schools**, would benefit from increased investment in educational resources and programs.
* Schools with **lower scores** in math and reading should receive targeted funding for improving teaching resources, specialized support for struggling students, and enrichment programs.
2. Smaller Class Sizes:
* Given that **smaller schools** tend to show better academic performance, schools should consider strategies that allow for smaller class sizes or more personalized instruction.
* Reducing class sizes in subjects like math, where students are performing at a lower rate, could help close the performance gap and boost overall passing rates.
3. Curriculum Adjustments:
* Based on the **lower passing rate** in math, schools should prioritize enhancing math curriculum and instructional methods. Implementing strategies such as tutoring programs, after-school workshops, or incorporating more hands-on activities can help improve student performance in math.

## Challenges:
* **Missing or Incomplete Data:** Some recods had missing student scores, requiring imputation or removal to maintain data integrity.
* **Data Consistency Issues:** School names and budget data needed standardization to ensure accurate merging and aggregation.
* **Handling Large Data Sets:** Processing nealry 40,000 student records required optimizing calculations for efficiency.
* **Interpreting Correlations:** While trends were observed between school funding and performance, external factors like teaching quality and student demographics made causation unclear.

## What Could Have Been Done Differently?
* **Deeper Analysis on Teaching Quality:** Incorporating teacher-to-student ratios or teacher experience data could provide more insights into performance differences.
* **Longitudinal Data:** Tracking performance over multiple years could show trends and help identify long-term impacts of funding or policy changes.
* **Student-Level Factors:** Analyzing demographic factors, attendance rates, or extracurricular activities could add depth to the insights.
