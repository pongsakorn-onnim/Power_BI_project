# Overview
This is an analysis of a fictional employee attrition and performance dataset from Kaggle. The dataset contains features about employee demographics and their work-related data such as age, gender, education, monthly income, job satisfaction, etc.
Understanding attrition factors can help the company address issues that employees might be struggling with and help them retain their talented employees.

# Dataset Structure
The dataset consists of 35 columns and 1470 rows with no missing values. Since the source doesn't provide column details, I've attempted to describe them based on context.
1.	**Age**: Age of the employee.
2.	**Attrition**: Whether the employee has left the company (Yes/No).
3.	**BusinessTravel**: Frequency of business travel (e.g., Travel_Rarely, Travel_Frequently).
4.	**DailyRate**: Daily rate of pay for the employee.
5.	**Department**: Department in which the employee works (e.g., Sales, Research & Development).
6.	**DistanceFromHome**: Distance of the employee's home from the workplace.
7.	**Education**: Level of education attained by the employee (1: 'Below College', 2: 'College', 3: 'Bachelor', 4: 'Master', 5: 'Doctor').
8.	**EducationField**: Field of education of the employee.
9.	**EmployeeCount**: Number of employees (usually constant for all rows).
10.	**EmployeeNumber**: Unique identifier for each employee.
11.	**EnvironmentSatisfaction**: Satisfaction level with the work environment.
12.	**Gender**: Gender of the employee.
13.	**HourlyRate**: Hourly rate of pay for the employee.
14.	**JobInvolvement**: Level of involvement in the job.
15.	**JobLevel**: Level of the employee's job within the company.
16.	**JobRole**: Role or position of the employee.
17.	**JobSatisfaction**: Satisfaction level with the job.
18.	**MaritalStatus**: Marital status of the employee.
19.	**MonthlyIncome**: Monthly income of the employee.
20.	**MonthlyRate**: Monthly rate of pay for the employee.
21.	**NumCompaniesWorked**: Number of companies the employee has worked for.
22.	**Over18**: Whether the employee is over 18 years old (Y/N).
23.	**OverTime**: Whether the employee works overtime (Yes/No).
24.	**PercentSalaryHike**: Percentage increase in salary for the employee.
25.	**PerformanceRating**: Performance rating of the employee.
26.	**RelationshipSatisfaction**: Satisfaction level with work relationships.
27.	**StandardHours**: Standard number of working hours per week.
28.	**StockOptionLevel**: Level of stock options granted to the employee.
29.	**TotalWorkingYears**: Total number of years the employee has worked.
30.	**TrainingTimesLastYear**: Number of training sessions attended by the employee last year.
31.	**WorkLifeBalance**: Perceived balance between work and personal life.
32.	**YearsAtCompany**: Number of years the employee has been with the company.
33.	**YearsInCurrentRole**: Number of years the employee has been in their current role.
34.	**YearsSinceLastPromotion**: Number of years since the employee's last promotion.
35.	**YearsWithCurrManager**: Number of years the employee has been with their current manager.

The first 5 rows of the dataset

![dataset_structure_01](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/c1dbe446-3e83-4d3c-9e34-6245dc8988a2)
![dataset_structure_02](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/5f57bf6d-9bd9-462f-b485-74502a9cc866)
![dataset_structure_03](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/8d14c097-de31-45e6-a531-24ef9ce13e7b)


# Data Transformation
1.	Created Dax Measures to calculate attrition rate, number of active/inactive employees, average monthly income, and total number of employees. We will use these measures to create insightful visualizations.
![02_dax_measuresjpg](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/bc3cd3cf-1a34-43ad-8406-192b8fa29313)

2.	Created age and monthly income bin columns, as the original columns had too many different values. Grouping them into bins helps us better see insights across different age and income groups.
![03_age_ _monthly_bins](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/75bdc641-20af-4973-aee5-1959e0527a6d)


# Data visualization and dashboard making
## Overview analysis
![04_overview](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/fcc45f52-71d4-4510-b19c-1cc285019181)
- The total number of employees is 1470 with 1233 active and 237 inactive employees. The attrition rate is **16.12%**. 
- **The R&D department has the highest number of employees** which takes up around 67.15% of total active employees followed by sales, and the HR department
- **The top three job roles by number of employees** are sales executive, research scientist, and laboratory technician.


## Demographics analysis
![05_demographics](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/70f7bd99-2f1a-4907-8668-47cbe5938131)
- **45.78% of employees are married**, 31.97% single, and 22.24% divorced.
- Most of the employees in the company are in **the 31-40 age range**, with 619 employees.


# Attrition analysis
![06_attrition](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/0aee18f9-eebb-4243-b81c-b9165069d1d3)
-	Employees **under 20 years old** have the highest attrition rate, at 58.82%.
-	Employees with a **monthly income below $5,000** have the highest attrition rate, at 21.76%.
-	Employees who **frequently travel for business** have the highest attrition rate, at 24.91%.
-	Employees who **work overtime** have a higher attrition rate than those who don't, at 30.53%.
- **The sales department has the highest attrition rate** with 20.63% followed by human resources at 19.05%, and research & development at 13.84%.
- Employees who **live farther from the company have a higher chance of leaving**.

# Recommendations
**Target younger employees (under 20) with engagement programs:**
This age group has the highest attrition rate. Consider mentorship programs, social events, or clear career development paths to increase their engagement and retention.

**Promote work-life balance:**
Consider offering flexible work arrangements or remote work options to improve work-life balance, which could be a factor for employees who work overtime or have a long commute.

**Review workload and travel frequency:**
Employees who frequently travel for business and those who work overtime have a higher attrition rate. Explore ways to reduce workload or overtime, or offer additional compensation/benefits for those who travel extensively.

  



