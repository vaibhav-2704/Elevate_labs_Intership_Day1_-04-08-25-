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



**## Final Files**

\- **"KaggleV2-May-2016.xlsx"** – Raw dataset

\- **"medical-no-show-cleaning.xlsx"** – cleaned dataset



 

**## Tools Used**

\- Microsoft Excel



**## Author**

SALOORA VAIBHAV



