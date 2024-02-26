# HR Attrition-Analysis

## Table of Contents

- [Project Objective](#project-objective)
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#results/findings)
- [Limitations](#limitations)
- [References](#references)

### Project Objective:
- Review Current Employee Demographics
- Analyze Work Status factors contributing to attrition
- Review the effects of certain Work Conditions that instigate attrition
- Determine areas that can be improved in employee wellness to reduce attrition
  
### Project Overview

The HR Attrition Analysis comprises of four Dashboards showing the attrition trends at each specific employee condition

![HR_Attrition_Dashboard](https://github.com/bcpatino/HR-Attrition-Analysis/assets/159120303/defed131-29a6-4e26-9e56-c8c2c40a8c0c)


### Data Sources

[Meriskill](https://www.linkedin.com/company/meriskill/)

### Tools

- Analysis: Microsoft Power Query 
- Visualization: Microsoft Power BI

### Data Cleaning and Preparation

1. Changed Column Names for uniformity (Business Travel, Daily Rate, Distance from Home, Employee Count, Employee Number, Environment Satisfaction, Hourly Rate, Job Involvement, Job Level, Job Role, Job Satisfaction, Marital Status, Monthly Income, Monthly Rate, Num Companies Worked, Over 18, Over Time, Percent Salary Hike, Performance Rateing, Relationship Staisfaction, Standard Hours, Stock Option Level, Total Working Years, Training Times Last Year, Work Life Balance, Years in Company, Years in Current Role, Years since last Promotion, Years with current Manager) – added space in column names
2.	Removed '_' in Business Travel
3.	Removed irrelevant columns: (Education Column, Employee Count, Employee number, Hourly Rate, Job Involvement(vague numerical value), Job Level (vague numerical value), Monthly Income, Monthly Rate, Over 18, Relationship Satisfaction, Standard Hours, Total Working Years, Years in current role)
4.	Created Bins for: Age, Years at company, Daily Rate, Distance from Home, Environment Satisfaction, Job Satisfaction, % Salary Hike, Performance Rating and Work-Life Balance Rating.

### Exploratory Data Analysis (Questions you asked)

1.	Employee Demographics: What is the current overall profile of our employees?
2.	Attrition by Work Status: 
   - Which Department has the highest attrition?
   - Do Business Travels contribute to attrition?
   - What does Tenureship records show in terms of employee attrition?
   - Which of the employees tend to leave fast, high, middle or low level of salary?

3.	Attrition by Work Condition: 
   - Are those leaving farthest from work tend to leave the company faster?
   - Do investment opportunities of employees in the company keep employees?
   - Does Training exposures help in lowering attrition?
   - What does Employee-Manager relationship show in preventing employees to leave?
   - How significant is career growth in employee retention?
   - Do employees who had more previous experiences with other companies leave faster? 

4.	Attrition by Employee Wellness:
   - Which Environment Satisfaction Rating showed the highest attrition?
   - Which Job Satisfaction Rating showed the highest attrition?
   - Which Performance Rating showed the highest attrition?
   - Which Work-Life Balance Rating showed the highest attrition?
   - Does the % Salary increase level matter to employees leaving?

### Data Analysis
```Power BI - Measure
 %Attrition = DIVIDE ('HR-Employee-Attrition'[Attrition_Y], COUNTA('HR-Employee-Attrition'[Attrition]))

```

### Results/Findings

1. Employee Demographics:
   - Total Employee Count: 1470
   - Attrition Rate: 16.12% (237 pax)
   - Male: 60%  Female: 40%
   - There are 811 (majority) of employees aged 31-45. Average age is 37.
   - Research and Devt Department has teh most number of employees.
   - Top Educational Background of Employees is Life Sciences.
   - Majority of employees live near the workplace, farthest travels 29km daily.
   - 45% are married, 32% are single and 23% are divorced.  

2. Attrition by Work Status:
   - Sales Representatives has the highest turnover with 39.76%.
   - Consequently, Sales Department has the highest attrition rate at 20.63%.
   - Those who travel frequently for business tend to leave the most (52.04%).
   - Employees receiving the lowest daily wage rate leave fastest with 19.26% attrition rate.
   - Employees working 30 years and more has the highest attrition rate at 50%.
     
3. Attrition by Work COndition:
   - Employees who have worked with 5-10 previous companies tend to leave more, with 23% -25% attrition rate.
   - 66.98% attrition rate for employees with to stock availment options
   - The highest attrition rates was observed with employees-manager relationships of 1 year or less and 11 years up.
   - There is no specific trend but teh lowest attritions can be seen on years near the 5th, 10th and 15th year, then spikes up the year after.
   - Those travelling farthest has the highest attrition rate of 22.06%.
   - Employees who received 0 training has the highest attrition rate at 27.78%.
     
4. Attrition by Employee Wellness:
   - Only 2 performance scores were recorded, Excellent and Good. Both have equal attrition rates of 50%.
   - Single employees leave the company most at 53.08% attrition.
   - Employees given the highest salary increase percentage eventually leaves the company more.
   - Employees who gave BAD ratings on Environment Satisfaction, Job Satisfaction and Work-Life Balance resulted to a consequent high attrition rate.

### Limitations
- the study tackles descriptive analysis of attrition rate and did not go further into correlation factors of areas affecting attrition.
   
### References

