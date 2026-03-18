# Cyclistic Bike-Share Analysis

## Project Summary
This project analyzes historical Cyclistic bike-share trip data to examine how casual riders and annual members use the service differently. The objective is to identify behavioral patterns that can support marketing strategies aimed at increasing annual memberships.

## Business Question
How do casual riders and annual members differ in their bike-share usage, and what patterns could help inform member conversion strategies?

## Tools Used
- **SQL** — data cleaning, transformation, and analysis
- **R** — workflow validation and statistical summaries
- **R Markdown** — reporting and project presentation

## Project Workflow
This project uses a dual workflow in **SQL** and **R**. The main cleaning and analysis process was completed in SQL, then reproduced in R to validate the approach and demonstrate the same analytical logic across two environments.

### 1. Data Cleaning
**Location:** [SQL cleaning scripts](./Analysis/Scripts/SQL/01_cleaning)

- Standardized raw trip data from 2019 and 2020
- Cleaned column names and formats
- Removed incomplete or inconsistent records

### 2. Data Merging
**Location:** [SQL merge script](./Analysis/Scripts/SQL/02_merge/merge_cleaned_tables.sql)

- Combined cleaned quarterly tables into a single dataset for analysis

### 3. Analysis
**SQL:** [Statistical analysis scripts](./Analysis/Scripts/SQL/03_statistical_analysis)  
**R:** [R workflow script](./Analysis/Scripts/R/cyclistic_workflow.R)

The analysis focuses on:
- ride duration
- rider-type differences
- weekday and weekend usage
- monthly and seasonal trends

## Key Insights
- Casual riders tend to take longer rides than annual members.
- Casual rider usage is higher on weekends and during warmer months.
- Members show more consistent weekday usage, suggesting more routine travel behavior.

## Reports
- **Executive Summary (PDF):** [View PDF Report](./Reports/Cyclistic_Analysis_Markdown.pdf)
- **Technical Report (Markdown):** [View Markdown Report](./Reports/Cyclistic_Markdown.md)

## Data Source
The raw datasets are not included in this repository due to file size constraints. The SQL scripts assume the source data has already been loaded into a database.