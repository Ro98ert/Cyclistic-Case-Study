# Cyclistic Bike-Share Analysis

## Project Summary
This project analyzes historical Cyclistic bike-share trip data to understand how casual riders and annual members use the service differently. The goal is to generate insights that can support marketing strategies aimed at increasing annual memberships.

## Business Question
How do casual riders and annual members differ in their bike-share usage, and what patterns could help inform member conversion strategies?

## Tools Used
- **SQL** — data cleaning, transformation, and analysis
- **R** — workflow validation and statistical summary
- **R Markdown** — data visualization and reporting

## Project Workflow
This project uses a dual workflow in **SQL** and **R**. The primary cleaning and analysis process was completed in SQL, then reproduced in R to validate the approach and demonstrate the same logic across two analytical environments.

### 1. Data Cleaning
**Location:** [Path](https://github.com/Ro98ert/Cyclistic-Case-Study/tree/10b469c02c310c6bcea0ae902ea914d7bc5f83ab/Analysis/Scripts/SQL/01_cleaning)

- Standardized raw trip data from 2019 and 2020
- Cleaned column names and formats
- Removed incomplete or inconsistent records

### 2. Data Merging
**Location:** [Path](https://github.com/Ro98ert/Cyclistic-Case-Study/blob/10b469c02c310c6bcea0ae902ea914d7bc5f83ab/Analysis/Scripts/SQL/02_merge/merge_cleaned_tables.sql)

- Combined cleaned quarterly tables into a single dataset for analysis

### 3. Analysis
**SQL:** [Path](https://github.com/Ro98ert/Cyclistic-Case-Study/tree/10b469c02c310c6bcea0ae902ea914d7bc5f83ab/Analysis/Scripts/SQL/03_statistical_analysis)  
**R:** [Path](https://github.com/Ro98ert/Cyclistic-Case-Study/blob/10b469c02c310c6bcea0ae902ea914d7bc5f83ab/Analysis/Scripts/R/cyclistic_workflow.R)

The analysis focuses on:
- ride duration
- rider-type differences
- weekday and weekend usage
- monthly and seasonal trends

## Reports
- **Executive Summary (PDF):** [View PDF Report](./Reports/Cyclistic_Analysis_Markdown.pdf)
- **Technical Report (Markdown):** [View Markdown Report](./Reports/Cyclistic_Markdown.md)

## Data Source
The raw datasets are not included in this repository due to file size constraints. The SQL scripts assume the source data has already been loaded into a database.