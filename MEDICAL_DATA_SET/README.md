📌 Project Overview

This project demonstrates a complete ETL (Extract, Transform, Load) pipeline using Informatica PowerCenter to process a medical dataset. The pipeline extracts raw data from a source, performs cleaning and transformation, and loads the processed data into a target system for analytics and reporting.

🧱 Project Workflow
Extract

Source Type: CSV / Flat File 

Data: Raw medical records including patient information, diagnosis, treatments, etc.

Tool: Informatica Source Qualifier

Transform

Cleaning:

Remove null or invalid entries (missing IDs, invalid ages)

Standardize formats (date formats, gender values)

Filtering:

Include only complete and valid medical records

Transformation Logic:

Remove duplicate records

Drop rows with missing key values (patient ID, date)

Filter records based on business rules (only active patients)

Load

Target Type: Relational Database (Oracle) / csv

Destination Table: medical_data_set

⚙️ Tools & Technologies
ETL Tool: Informatica PowerCenter

Source: Flat file / CSV 

Target: SQL Database (Oracle / csv / Flat file)


📊 Example Use Case
Identify high-risk patients based on diagnosis history

Track treatment effectiveness over time

Generate reports for hospital management

✅ Execution Steps
Import source and target definitions in Informatica

Create mappings for data cleansing and transformation

Configure workflow and session tasks

Execute the workflow

Verify results in the target database

