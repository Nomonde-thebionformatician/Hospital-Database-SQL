# Hospital-Database-SQL
HospitalDB is a SQL Server mini‑project that designs and implements a hospital management database. It includes Patients, Doctors, Appointments, and Treatments tables with primary/foreign keys, sample records, and queries to demonstrate relational integrity and data analysis.

## Overview
This project is a mini‑project for database design and implementation using Microsoft SQL Server.  
It demonstrates the creation of a hospital management database (HospitalDB) with tables for Patients, Doctors, Appointments, and Treatments, including sample data and relationships.

## Objectives
- Design and create a relational database in SQL Server
- Define primary keys and foreign key relationships
- Insert meaningful sample records
- Execute queries to retrieve and analyze data
- Export the complete database as a .sql file

## Database Schema
Tables:
- Patients: patient_id, name, doctor_id, diagnosis, contact_number
- Doctors: doctor_id, doctor_name, hospital_units
- Appointments: appointment_id, patient_id, doctor_id, appointment_date
- Treatments: treatment_id, diagnosis, prescription, cost, appointment_id

Relationships:
- Patients linked to Doctors via doctor_id
- Appointments linked to Patients and Doctors
- Treatments linked to Appointments

## Sample Data
Patients: Mary Ndlovu, Anna Motha, Gary Zimela, Anita Houwer, Bella Hadid  
Doctors: Siyabonga Dlamini, Tebello Ntene, Anelisiwe Qetuka, Siyabonga Dladla, Kundai Gwembere  
Treatments: Tamiflu, Paracetamol, Antihistamine, Nasal spray, Vitamin C supplements

## How to Run
1. Open SQL Server Management Studio (SSMS).
2. Run the script file: HospitalDB.sql
3. The database will be created with tables, constraints, and sample records.
4. Execute queries to:
   - Display all records from each table
   - Use JOINs to combine patient, doctor, and appointment details
   - Show treatment details including costs

## Academic Context
This project was completed as part of a school assignment in SQL Server.  
It demonstrates practical skills in database
