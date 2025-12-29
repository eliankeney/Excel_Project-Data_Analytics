## 📊 Data Science Salary Dashboard (Excel)
Project Overview

This project is a dynamic, interactive Salary Dashboard built entirely in Excel. It enables users to explore median salaries across various data roles, geographic locations, and employment types. By leveraging advanced Excel functions and data visualization principles, I transformed raw job market data into an actionable decision-making tool.

🔗 [Link to Download/View Excel File](Project_1-Dashboard.xlsx)

## 🛠️ Excel Skills & Technical Implementation

<img width="1486" height="673" alt="Clean version" src="https://github.com/user-attachments/assets/ee3a362a-c1dd-4d07-9d7b-3cf67657d41f" />


This project demonstrates professional-level competency in Excel, specifically focusing on data cleaning, complex logic, and UI/UX design:
- Advanced Formulas (Array Logic): Utilized nested MEDIAN(IF(...)) logic to perform multi-criteria filtering.
- Example: Used Boolean multiplication (logic gates) to filter by Job Title, Country, and Schedule Type simultaneously while ignoring zero-value entries.
- Dynamic Data Filtering: Implemented ISNUMBER(SEARCH(...)) arrays to handle partial text matching within job schedule descriptions.
- Interactive Controls: Integrated Data Validation (Dropdowns) and Slicers to allow real-time dashboard updates without manual data entry.
- Data Modeling: Organized data using Excel Tables (Structured References) to ensure the dashboard remains scalable as new data is added.

## The Logic Under the Hood
To calculate the dynamic KPIs, I used the following array formula structure:

<img width="557" height="242" alt="median salary functions" src="https://github.com/user-attachments/assets/c568df37-9acd-451c-a26c-c61d11178f90" />

📈 Visualizations & Insights
The dashboard features several key visualizations designed for clarity and quick insight:
- Horizontal Bar Charts: Used to rank median salaries by job title, allowing for easy comparison between roles like Senior Data Scientist ($155k) and Data Analyst ($90k).
- Geographic Heat Map: A global map visualization to show the distribution of job opportunities and regional data density.
- Category Comparison: A focused bar chart comparing employment types (Full-time vs. Contractor vs. Internship) to highlight compensation variances.
- KPI Scorecards: Large, high-visibility cards displaying Median Salary, Top Job Platform, and Total Job Count for the selected filters.

## 📂 Data Summary
The data reflects a diverse range of roles in Data Science

<img width="353" height="266" alt="data table for median salary" src="https://github.com/user-attachments/assets/cc8337f1-df9b-4565-830b-a3761ef96787" />

## 💡 Key Takeaways
- Specialization Pays: Senior roles and Machine Learning positions command a significant premium (~60% higher) over general Analyst roles.

- Market Presence: With a job count of over 6,400 for Data Analysts in the US alone, the demand remains robust.

- Platform Dominance: Indeed emerged as the primary source for job listings in this dataset.

## How to Use
1. Clone this repository.
2. Open the Project_1-Dashboard.xlsx File
3. Use the Dropdown menus at the top to filter by Job Title, Country, or Job Type.
4. Watch the charts and KPI cards update instantly!



