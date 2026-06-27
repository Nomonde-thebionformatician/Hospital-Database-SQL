# HospitalDB

HospitalDB is a sample SQL Server database project designed to simulate a hospital information system. It demonstrates relational database design, table creation, foreign key constraints, and sample queries for managing doctors, patients, appointments, and treatments.

## Project Overview
This project models a fictional hospital database with four core entities:
- Doctors – medical staff with specialties
- Patients – individuals receiving care
- Appointments – scheduled visits linking patients and doctors
- Treatments – prescriptions and procedures linked to appointments

The database is built for educational purposes, showcasing:
- Schema design with primary and foreign keys
- Referential integrity between tables
- Sample data insertion
- Analytical queries for reporting

## Database Schema

Tables:
- `Doctors(doctor_id, doctor_name, hospital_units)`
- `Patients(patient_id, name, doctor_id, diagnosis, contact_number)`
- `Appointments(appointment_id, patient_id, doctor_id, appointment_date)`
- `Treatments(treatment_id, diagnosis, prescription, cost, appointment_id)`

Relationships:
- Patients → Doctors (many-to-one)
- Appointments → Patients & Doctors (many-to-one)
- Treatments → Appointments (many-to-one)

## Setup Instructions
1. Run the provided `HospitalDB.sql` script in SQL Server Management Studio (SSMS).
2. The script will:
   - Drop any existing `HospitalDB` database
   - Create a fresh `HospitalDB`
   - Build all tables with constraints
   - Insert sample data
