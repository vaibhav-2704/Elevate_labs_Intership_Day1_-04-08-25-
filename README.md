#### **# Medical Appointment No-Show Dataset – Cleaning Project 🩺📊**


**## Objective**

To clean and prepare the raw “Medical Appointment No-Show” dataset by:

\- Handling missing values

\- Removing duplicates

\- Fixing encoding issues in text (e.g., neighbourhood names)

\- Standardizing date formats

\- Renaming columns to consistent, clean names

\- Ensuring all data types are correct



**## Dataset Info**

\- Source: \[Kaggle Dataset](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

\- Size: ~110K records

\- Fields: PatientID, AppointmentDay, Gender, Neighbourhood, No-show, etc.



**## Key Cleaning Steps**

\- Cleaned corrupted neighbourhood encodings (e.g., "Ã‰" → "É")

\- Converted "ScheduledDay" and "AppointmentDay" to proper Excel date format

\- Created additional fields: "Wait Days", "Appointment Date", etc.

\- Standardized columns to "snake\_case" format



## 🔣 Excel Formulas Used for Data Cleaning

Below are the formulas i have applied to clean and transform the dataset using Excel:

| Column Name               | Description                                                  | Formula                                             |
|---------------------------|--------------------------------------------------------------|-----------------------------------------------------|
| 'ScheduleDay_Cleaned'     | Converted 'ScheduledDay' from datetime to 'dd-mm-yyyy'       | '=TEXT(D2, "dd-mm-yyyy")'                           |
| 'AppointmentDay_Cleaned'  | Converted 'AppointmentDay` to 'dd-mm-yyyy' format            | '=TEXT(E2, "dd-mm-yyyy")'                           |
| 'Wait_Days'               | Calculated number of days between scheduled and appointment  | '=G2 - F2' or '=MAX(0, G2 - F2)'                    |
| 'Age_Cleaned'             | Cleaned age value to ensure it's an integer                  | '=INT(H2)'                                          |
| 'Age_Groups'              | Categorized patients into age groups                         | '=IF(I2<13, "Child", IF(I2<60, "Adult", "Senior"))' |
| 'Neighbourhood_Cleaned'   | Standardized neighborhood names to proper case               | '=PROPER(L2)'                                       |
| 'No_Show_Cleaned'         | Converted `No_show` to binary (1=No, 0=Yes)                  | '=IF(T2="Yes", 1, 0)'                               |


**## Final Files**

\- **"KaggleV2-May-2016.xlsx"** – Raw dataset

\- **"medical-no-show-cleaning.xlsx"** – cleaned dataset


**## Tools Used**

\- Microsoft Excel


**## Preview**

<img width="1862" height="340" alt="image" src="https://github.com/user-attachments/assets/1791b86e-ea4f-44a1-87c4-dc430e101f64" />


**## Author**

SALOORA VAIBHAV
