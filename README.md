# Healthcare-Patient-Visits-Analysis
Patient Visits Analysis 2019 - 2020
## Overview
#### In this scenario, I'm a new Junior data analyst hired within a hospital. For my first project my manager assigned me to build an interactive dashboard of patient visits and an overall presentation using PowerPoint. He provided me with the dataset with all the information I needed.

Dashboard
Key Performance indicators (KPIs) Requirements:
1. Average Wait Time: Discover how long patients typically wait before their appointments. Uncover patterns and trends that shed light on the efficiency of our healthcare system. 
2. Patient Satisfaction: We'll explore the average satisfaction scores given by our patients. Learn about the factors that contribute to a positive patient experience and how we can enhance it. 
3. Total Patient Visits by Weekday and Month: Get an overview of the ebb and flow of patients through our doors each weekday and month. Understand the dynamics of healthcare demand over time. 
4. Administrative vs. Non-Administrative Appointments: Delve into the data to distinguish between appointments that involve administrative processes and those that don't. Explore the impact on wait times and patient satisfaction. 
5. Referrals and Walk-In Patients: Uncover the balance between patients referred to specific departments and those who walk in without prior referral. How does this impact the overall patient experience? 
6. Patient Visits by Age Group and Race: Explore the distribution of patient visits across different age groups and races. Gain insights into the diversity of healthcare needs and preferences.


## Getting Started
•	Prerequisites: SQL SERVER MANAGEMENT STUDIO (SSMS), POWER BI, MS Office Word / Excel, PowerPoint.

## Usage 

- Understand the business and the problem. 
- Data source: Patients Healthcare dataset.zip - Google Drive
- Data format: The dataset (Hospital ER) is a CSV file and has 9 216 rows and 11 columns.

  
#### Features used in data:
- Date: date and time of the record entry
- Patient_id: Unique identifier for each patient
- Patient_gender: The gender of patient (M: Male, F: Female)
- Patient_age: The age of the patients
- Patient_sat_Score: The satisfaction score of the patients.
- Patient_first_initial: First initial name of the patients
- Patient_last_name: The last name of the patients
- Patient_race: The race of the patients
- Patient_admin_flag: Boolean indicating whether the patient is an admin.
- Patient_waittime: The waiting time of the patients in minutes
- Department_referral: Department in which the patient is referred (if any)



-	Data type: No idea. (It’s important to know if the data along the first-party data, the second-party data, or the third-party data. That could be helpful when dealing with missing values) 


#### Data cleaning and preprocessing
-	The data has 6 699 missing values especially in the Patient_sat_score column. We used =COUNTBLANK(RANGE) using excel to check that. 
-	No duplicates records found.
-	No outliers found.


Everything looks good. It’s time to import the data within the SQL Server Management Studio and perform the following queries. These queries will be used to validate our interactive dashboard.


#### EDA
- In POWER BI, I imported the data from SQL Server.
- I used Power BI for visualization and analysis.
- I built an interactive Dashboard that contains many different charts. 

#### Dashboard Validation
I used SQL queries to validate the dashboard.

After two weeks of work, I delivered the interactive dashboard and the overall presentation to my manager(You can find it within the Finding and insights file under the name of Interactive Dashboard healthcare patient and patient visits presentation).
