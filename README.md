# Table-Design-Creation
🩺 CardioHealthDB
A structured SQL database for managing and analyzing cardiovascular health data.

📘 Table of Contents

Overview
Database Structure
Tables and Relationships
Data Integrity & Constraints
Sample Data
How to Run
Use Cases

🧬 Overview

CardioHealthDB is a SQL Server–based database designed to store, organize, and analyze medical information related to cardiovascular health.
It includes patient demographics, medical measurements, lifestyle factors, clinical status, and heart‑disease diagnoses.
This structure is suitable for:
Medical research
Data analysis
Machine learning projects
Academic assignments
SQL practice

🗂 Database Structure

The database contains five core tables:
Patients – Basic demographic and physical data
Measurements – Periodic medical measurements
Medical_Status – Cholesterol and glucose levels
Lifestyle – Smoking, alcohol, and physical activity
Diagnosis – Cardiovascular disease indicator

📊 Tables and Relationships

Patients
Stores essential patient information.
Fields:
PatientID (Primary Key)
Gender (1 = Male, 2 = Female)
BirthDate
Height (120–250 cm)
Weight (30–250 kg)
Measurements
Contains periodic medical measurements.
Fields:
SystolicBP
DiastolicBP
BMI
MeasureDate
Relationship:
1:N with Patients (each patient can have multiple measurements)
Medical_Status
Includes basic clinical indicators.
Fields:
Cholesterol (1–3)
Glucose (1–3)
Relationship:
1:1 with Patients
Lifestyle
Tracks lifestyle habits.
Fields:
Smoking
Alcohol
PhysicalActivity
Relationship:
1:1 with Patients
Diagnosis
Stores cardiovascular disease diagnosis.
Fields:
CardioDisease (0 = No, 1 = Yes)
Relationship:
1:1 with Patients

🔒 Data Integrity & Constraints

The database enforces strict validation rules, including:
SystolicBP > DiastolicBP
Valid ranges for height, weight, BMI, and blood pressure
Controlled categorical values (Gender, Cholesterol, Glucose)
Foreign key constraints linking all tables to Patients
These ensure clean, reliable, and medically consistent data.

🧪 Sample Data

The script includes:
20 patients
Measurements for each patient
Medical status, lifestyle, and diagnosis entries
All sample data is inserted automatically.

▶️ How to Run

Open the script in SQL Server Management Studio (SSMS).
Execute the script to create the database CardioHealthDB.
All tables, constraints, and sample data will be created automatically.

🎯 Use Cases

This database is ideal for:
Cardiovascular risk analysis
Machine learning model training
SQL exercises and demonstrations
Academic research
Data visualization projects
