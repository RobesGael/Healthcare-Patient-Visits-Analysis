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
- Data type: No idea. (It’s important to know if the data along the first-party data, the second-party data, or the third-party data. That could be helpful when dealing with missing values) 

  
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




#### Data cleaning and preprocessing
-	The data has 6 699 missing values especially in the Patient_sat_score column. We used =COUNTBLANK(RANGE) using excel to check that. 
-	No duplicates records found.
-	No outliers found.


Everything looks good. It’s time to import the data within the SQL Server Management Studio and perform the following queries. These queries will be used to validate our interactive dashboard.

- Display all the data
  
![1  display all the data](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/699ef05d-66a5-4551-8254-058ecbbc459c)

- Total patients visits

![2  total patient visits](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/1266fde1-94b6-443e-b6cc-3971f79f706a)

- Total patient visits by year

![3  total patients by year](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/b8c5c2c2-7ede-4a42-a44a-14d8172bc761)

- Total patient visits by gender

![4  TP by gender](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/5bde2d55-6d75-4791-a0d6-bb31e3666e8a)

- Percentage of Male

![5  percentage of male](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/fc002153-8ade-4d9a-b7f3-e2910280ccaa)

- Percentage of Female

![6  percentage female](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/28f7950e-10e6-40cf-8e02-2272a1199d9d)

- Percentage of Unknown gender

![7  precentage NC](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/4ef8809b-8792-477c-9b44-2daae0910d54)

- Percentage of None administrative appointment

![8  None admin appoint](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/14698402-613d-43f5-a44f-50ebddd23f86)

- Percentage of administrative appointment

![9  Admin appoint](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/7b4a89e7-023a-4aba-826d-a02b9136e914)

- Percentage of walki-in-patients

![10  walk_in patient](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/a5bc7a36-da35-4539-aaa5-4d404dd9cb3e)

- Percentage pf patients referred

![11  referral patients](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/7f3ea637-30c2-4a8c-857d-061f2836d1dc)

- Total patient visits by department referral

![12  TP BY DPTMENT REFFERRAL](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/9bf96d3a-dc68-40ee-8a66-9f37de6e3de5)

- Total patient visits by race

![13  TP by race](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/4dbd0f19-6655-407a-8f1d-78cef935d54f)

- Average wait time

![14  AVG waitting](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/98f92213-aafe-4bef-8bbc-325b0789b6a2)

- Total patient visits by month

![15  TP BY month](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/c57699d5-b643-441d-8a8f-5d93bd6f9637)

- Total patient visits by weekday

![16  TP BY WEEKDAY](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/6a1b87c0-0824-4895-83ed-a2db83318311)

- Percentage service rated

![17  percentage service rated](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/b98c208a-320d-48ca-8223-aa961f4e7251)

- Percentage service not rated

![18  percentage not rated](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/9b0514f6-a57a-44fd-bca9-4d01ecfd53f9)

- Average patient's satisfaction

![19  AVG PATIENT SATISFACTION](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/2c924622-f4f9-40c3-86a0-337b3a1dd5d0)

- Total patient visits by weekday and weekend

![20  TP BY WD, ww](https://github.com/RobesGael/Healthcare-Patient-Visits-Analysis/assets/155399653/3bbd71f4-5dd0-439b-adec-f9307c01ba26)


#### EDA
- In POWER BI, I imported the data from SQL Server.
- I used Power BI for visualization and analysis.
- I built an interactive Dashboard that contains many different charts. 

#### Dashboard Validation
I used SQL queries to validate the dashboard.

After two weeks of work, I delivered the interactive dashboard and the overall presentation to my manager(You can find it within the Finding and insights file under the name of Interactive Dashboard healthcare patient and patient visits presentation).
