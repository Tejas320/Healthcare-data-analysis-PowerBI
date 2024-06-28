# Health Care Data Driven Decisions Using Power BI
## (EY GDS-AICTE Internship Project)
### Dashboard Link: https://app.powerbi.com/groups/me/reports/89de2836-30ef-4036-bb30-07e73f903ee9/ReportSection?redirectedFromSignup=1&experience=power-bi
## Introduction
The healthcare industry generates vast amounts of data daily, presenting a challenge in transforming this data into actionable insights. Leveraging Power BI, healthcare organizations can harness this data to make informed, data-driven decisions. This approach aims to enhance patient care, streamline operations, and improve overall healthcare outcomes. By visualizing key metrics and trends, stakeholders can identify areas for improvement and implement evidence-based strategies effectively.
## Objectives
1. Disease Analysis basing on Smoking Habit
2. Disease Analysis basing on Alcohol Habit
3. Count of Patients Visit by Week Name
4. Count of Patients by Age Group
5. Percent of Male and Female Patients
6. Average duration of Stay in the Hospital
## Dataset Description
For healthcare data analysis, 2 datasets are used - Admission Details, Patient Details
### Admission details - No. of rows=12,244, No. of columns=2
1. Admission No - Unique admission number assigned to each patient
2. Name - Name of each patient
### Patient Details - No. of rows=14,765, No. of columns=18
1. Admission No - Unique admission number assigned to each patient
2. D.O.A. - Date of Admission of each patient
3. D.O.D. - Date of Discharge of each patient
4. Age - Age of each patient
5. Gender - Gender of each patient (Male, Female)
6. Rural - Whether patient is from city(Urban) or village(Rural)
7. Type of Admission-Emergency/OPD - Whether the patient is in emergency or OPD
8. Duration of Intensive Unit Stay - Duration of a patient in ICU
9. Outcome - Whether the patient is discharged, or discharged against medical advice(DAMA), or the patient expired
10. Smoking - Whether the patient smokes or not
11. Alcohol - Whether the patient drinks alcohol or not
12. DM - Whether the patient has diabetes or not (DM - Diabetes Mellitus)
13. HTN - Whether the patient is suffering from hypertension(HTN) or not
14. CKD - Whether the patient is having chronic kidney disease(CKD) or not
15. Neuro Cardiogenic Syncope - Whether the patient is suffering from Neuro Cardiogenic Syncope or not
16. Cardiogenic Shock - Whether the patient is suffering from Cardiogenic Shock or not
17. Pulmonary Embolism - Whether the patient is suffering from Pulmonary Embolism or not
18. Doctors Note - Doctors note for patients
## Data Cleaning and Preprocessing
1. Created a new column 'Duration of Stay'
   ```bash
   Duration of Stay = ABS(DATEDIFF('Patient Details'[D.O.A],'Patient Details'[D.O.D],DAY))
   ```
## Visualizations
1. Created a decomposition tree showcasing the number of patients who smoke and are having lungs disease, neuro disease and chronic kidney disease (CKD)
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/c6e2fb22-e0bc-4ea7-943b-4d3ec096e759)
2. Created a decomposiion tree showcasing the number of patients who are alcoholic and are having lungs disease, bp problem, having sugar along with their age group
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/b0ff6de2-8852-4648-9c67-7c96cbda8942)
3. Created a line chart showcasing the total number of patients visited the hospital on each day
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/f3f9669a-6a75-43fc-b3f2-fe7bf65d8c80)
4. Created a stacked bar chart showcasing the total patients by age group
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/0bf1e89c-515d-4526-88a7-806e286a4106)
5. Created multile cards showcasing the total number of patients, total number of male and female patients, percentage of male and female patients
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/50945e1d-03df-4ba4-9aa3-f4ba4623d2f4)
6. Created card for showcasing average duration of stay in hosptal and average duration of ICU stay in hospital
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/fe5446ca-8c06-4eab-bb21-4b5042fef12e)
7. Created multiple slicers for Rural(Urban, Rural), Gender(Male, Female), Type of Admission(Emergency, OPD)
   ![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/0162f262-e60d-401c-8094-75c849996902)
## Final Power BI Dashboard
![image](https://github.com/Tejas320/Healthcare-data-analysis-PowerBI/assets/73283098/4e2d64d0-e028-482a-8c4e-83ce44636a22)






