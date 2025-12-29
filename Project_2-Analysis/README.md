## 🎯 Project Objective
This project was designed to answer four critical questions for data professionals navigating the current job market:

- The Skill Premium: Does a larger skill set directly correlate to higher pay?

- Geographic Variance: Which regions offer the highest median compensation?

- Market Demand: What are the most requested skills in the industry today?

- The "High-Value" Skills: Which specific skills command the highest salary?


## 🛠️ Technical Implementation (The ETL Pipeline)
1. Data Transformation (Power Query)
I used Power Query to handle the Extraction, Transformation, and Loading (ETL) process.

data_jobs_salary sheet
<img width="1918" height="993" alt="Screenshot 2025-12-29 155202" src="https://github.com/user-attachments/assets/047a7d1c-a8de-48f2-8a8e-d264c8522f2b" />
data_jobs_skills sheet
<img width="1918" height="991" alt="Screenshot 2025-12-29 155226" src="https://github.com/user-attachments/assets/074ed798-08a0-4dcb-80a6-881bd9ac6af8" />

Data Cleaning: Removed duplicates, standardized "Job Schedule Types," and filtered out entries with missing salary data.

Unpivoting Skills: Since skills were often lumped into a single string, I used Power Query to split and unpivot them, creating a granular model where each skill/job pairing is a unique row.

2. Data Modeling & DAX (Power Pivot)
To provide more depth than a standard Pivot Table, I utilized Power Pivot to create a relational data model.

DAX Measures: I authored DAX (Data Analysis Expressions) to calculate the Median Salary, ensuring the analysis remained statistically robust against outliers (unlike simple averages).

Formula Logic: Used MEDIAN and CALCULATE to allow the dashboard to update dynamically based on user-selected slicers.

Created a relationship between the two tables using job_id column.

<img width="817" height="603" alt="Screenshot 2025-12-29 155336" src="https://github.com/user-attachments/assets/23738d1d-48da-4307-91e7-b4f42d011109" />

## Q1: Skill Count vs. Pay
By using a Scatter Plot and Trendline, I analyzed if "more is better."

The Verdict: While there is a baseline increase, the data shows "Quality over Quantity." Mastering 3 high-value skills (like Python, AWS, and Spark) often leads to higher pay than 10 entry-level skills.

<img width="720" height="392" alt="Do more Skills equal more Pay Pic Scatter Plot" src="https://github.com/user-attachments/assets/0b428f4c-d930-4f4b-8dde-62c60311c8a9" />

## Q2: Regional Salary Distribution

- I created a PivotTable using the Data Model I created with Power Pivot
- I moved the job_title_short to the rows and the salary_year_avg into the values area
- Then I added the measure to calculate the median salary for the United States and Non-United States

<img width="882" height="337" alt="Screenshot 2025-12-29 155426" src="https://github.com/user-attachments/assets/27a6da08-7902-4cdc-8edc-338ee1becbc9" />

Insights: 
- Jobs like Senior Data Engineer and Data Scientist command higher salaries in the U.S. and internationally.
- The disparity between US and Non-US roles mainly stems from the high-tech jobs

## Q3 & Q4: The Top 10 Skills & Their Worth

I utilized Sorted Bar Charts and Pivot Tables to cross-reference popularity with profitability.

<img width="1071" height="353" alt="Top 10 Skills Pay Pic" src="https://github.com/user-attachments/assets/381103ed-acaf-493b-876b-50f7e8f6ef87" />

Market Leaders: SQL and Python are the most demanded (appearing in over 50% of postings).

Insights:
- The chart demonstrates that the importance of investing time in learning high-value skills like Python and SQL, which are tied to higher-paying roles, will ultimately help job seekers to maximize their salary in the tech industry.

## Conclusion
This project allowed me to master the end-to-end analytical workflow by transforming raw job data into a polished, interactive business intelligence tool. Through the integration of Power Query for ETL and DAX for complex modeling, I developed the technical discipline required to maintain data integrity while calculating sophisticated metrics like multi-criteria medians. I gained critical experience in UI/UX design by utilizing slicers and dynamic charts to ensure complex salary trends remain accessible and actionable for any stakeholder. Ultimately, this journey sharpened my ability to bridge the gap between technical data engineering and visual storytelling.










