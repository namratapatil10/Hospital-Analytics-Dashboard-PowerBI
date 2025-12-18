Hospital Performance Analytics Dashboard

Project Overview

The Hospital Performance Analytics Dashboard is an end-to-end healthcare data analytics project developed using Microsoft Power BI.
The objective of this project is to analyze patient visits, revenue trends, department performance, demographics, doctor workload, city-wise distribution, and payment preferences to support data-driven decision-making in a multispeciality hospital.

This project demonstrates the complete BI workflow including data cleaning, data modeling, DAX calculations, and professional dashboard design to transform raw healthcare data into meaningful business insights.

Key Insights

Orthopedics records the highest patient visits due to frequent injury and follow-up cases.

Viral Infection contributes the highest revenue among all diagnoses.

Delhi, Mumbai, and Hyderabad are the top-performing cities by patient volume.

Patient visits are highest in the 18–55 age group, while the 56+ group incurs the highest treatment cost.

Doctor workload is uneven, with a few doctors handling a large share of patient visits.

Hospital visits increase during monsoon and winter months.

Cash/Card is the most preferred payment method.

A positive relationship exists between patient age and treatment cost.


Step 1: Dataset Overview

The dataset contains 10,000 hospital visit records representing real-world healthcare activity.

Key Fields

Patient ID

Age

Gender

City

Department

Diagnosis

Doctor Name

Visit Date

Treatment Cost

Payment Method


Total Records: 10,000
File Type: CSV


Step 2: Data Cleaning & Transformation (ETL)

Performed using Power Query in Power BI.

Key Transformations

Removed null and duplicate records

Standardized department, city, and diagnosis names

Converted columns to correct data types

Extracted Year and Month from Visit Date

Created Age Groups (0–17, 18–35, 36–55, 56+)

Cleaned formatting and ensured consistency


Step 3: Data Modeling & DAX Calculations

A structured star schema data model was designed.

Data Model

Fact Table: hospital_visits

Dimension Table: Calendar

Relationship based on Visit Date


Key DAX Measures

Total Visits = DISTINCTCOUNT(hospital_visits[VisitID])
Total Patients = DISTINCTCOUNT(hospital_visits[PatientID])
Total Revenue = SUM(hospital_visits[TreatmentCost])
Avg Cost Per Visit = DIVIDE([Total Revenue], [Total Visits])
Visit YoY % = DIVIDE([Total Visits] - [Visits LY], [Visits LY])

Step 4: Dashboard Design

Clean and professional layout

KPI cards for summary metrics

Clear separation of trends, demographics, and performance

Interactive slicers for Year, Department, Gender, and City

Consistent color theme and typography


Step 5: Visualizations Used

KPI Cards: Total Visits, Total Patients, Total Revenue, Avg Cost

Line Chart: Monthly Visit Trend

Bar Charts: Revenue by Department, Top Cities

Donut Chart: Gender Distribution

Bar Chart: Visits by Age Group

Treemap: City-wise Patient Distribution

Scatter Plot: Age vs Treatment Cost


Step 6: Tools & Technologies

Power BI Desktop

Power Query (ETL)

DAX

Data Modeling (Star Schema)

CSV Dataset


Step 7: Project Outcome

This dashboard helps hospital management to:

Identify high-performing departments

Understand patient demographics

Monitor revenue and seasonal visit trends

Analyze doctor workload distribution

Improve planning, staffing, and operational efficiency


Key Skills Demonstrated

End-to-end data cleaning and transformation

DAX-based KPI and metric creation

Data modeling and relationships

Professional dashboard design

Business insight generation using healthcare data


Conclusion

This project showcases the complete Power BI analytics lifecycle—from raw data to actionable insights.
It highlights how healthcare organizations can leverage data analytics to improve patient care, operational efficiency, and strategic decision-making.
