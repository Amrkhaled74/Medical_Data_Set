
# Medical Dataset ETL Project using Informatica

## Table of Contents

* [Project Overview](#project-overview)
* [Project Workflow](#project-workflow)

  * [Extract](#extract)
  * [Transform](#transform)

    * [Cleaning & Filtering](#cleaning--filtering)
    * [Transformation Logic](#transformation-logic)
  * [Load](#load)
* [Tools & Technologies](#tools--technologies)
* [Example Use Case](#example-use-case)
* [Execution Steps](#execution-steps)
* [Contact](#contact)

---

## Project Overview

This project demonstrates a complete ETL (Extract, Transform, Load) pipeline using **Informatica PowerCenter** to process a medical dataset. The pipeline extracts raw data from a source, performs cleaning and transformation, and loads the processed data into a target system for analytics and reporting.

---

## Project Workflow

### Extract

* **Source Type:** CSV / Flat File
* **Data:** Raw medical records including patient information, diagnosis, treatments, etc.
* **Tool:** Informatica Source Qualifier

### Transform

#### Cleaning & Filtering

* **Cleaning:**

  * Remove null or invalid entries (missing IDs, invalid ages)
  * Standardize formats (date formats, gender values)
* **Filtering:**

  * Include only complete and valid medical records

#### Transformation Logic

* Remove duplicate records
* Drop rows with missing key values (patient ID, date)
* Filter records based on business rules (only active patients)

### Load

* **Target Type:** Relational Database (Oracle) / CSV
* **Destination Table:** `medical_data_set`

---

## Tools & Technologies

* **ETL Tool:** Informatica PowerCenter
* **Source:** Flat file / CSV
* **Target:** SQL Database (Oracle / CSV / Flat file)

---

## Example Use Case

* Identify high-risk patients based on diagnosis history
* Track treatment effectiveness over time
* Generate reports for hospital management

---

## Execution Steps

1. Import source and target definitions in Informatica
2. Create mappings for data cleansing and transformation
3. Configure workflow and session tasks
4. Execute the workflow
5. Verify results in the target database


