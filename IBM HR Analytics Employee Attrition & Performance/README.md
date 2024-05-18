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

Data Transformation
1.	Created Dax Measures to calculate attrition rate, number of active/inactive employees, average monthly income, and total number of employees. We will use these measures to create insightful visualizations.
![02_dax_measuresjpg](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/bc3cd3cf-1a34-43ad-8406-192b8fa29313)

2.	Created age and monthly income bin columns, as the original columns had too many different values. Grouping them into bins helps us better see insights across different age and income groups.
![03_age_ _monthly_bins](https://github.com/pongsakorn-onnim/Power_BI_project/assets/87061596/75bdc641-20af-4973-aee5-1959e0527a6d)

  



