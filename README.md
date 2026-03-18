# Cyclistic Bike-Share Analysis

## Project Summary
This project analyzes historical Cyclistic bike-share trip data to compare how casual riders and annual members use the service. The goal is to identify behavioral patterns that could help inform marketing strategies aimed at increasing annual memberships.

## Business Question
How do casual riders and annual members differ in their bike-share usage, and what patterns could support member conversion strategies?

## Tools Used
- **SQL** — data cleaning, transformation, and analysis
- **R** — analysis support, validation, and summary work
- **R Markdown** — reporting and project presentation

## Workflow
This project uses a dual workflow in **SQL** and **R**. The main cleaning and analysis process was completed in SQL, then reproduced in R to confirm the approach and demonstrate the same analytical logic across two environments.

## Repository Contents

### 1. SQL Cleaning
**Location:** [`Analysis/Scripts/SQL/01_cleaning/`](./Analysis/Scripts/SQL/01_cleaning/)

This folder contains the quarterly cleaning scripts used to standardize the raw trip data:
- [`clean_2019_q1.sql`](./Analysis/Scripts/SQL/01_cleaning/clean_2019_q1.sql)
- [`clean_2019_q2.sql`](./Analysis/Scripts/SQL/01_cleaning/clean_2019_q2.sql)
- [`clean_2019_q3.sql`](./Analysis/Scripts/SQL/01_cleaning/clean_2019_q3.sql)
- [`clean_2019_q4.sql`](./Analysis/Scripts/SQL/01_cleaning/clean_2019_q4.sql)
- [`clean_2020_q1.sql`](./Analysis/Scripts/SQL/01_cleaning/clean_2020_q1.sql)

Main tasks:
- standardized column names and formats
- cleaned inconsistent or incomplete records
- prepared each quarter for merging

### 2. SQL Merge
**Location:** [`Analysis/Scripts/SQL/02_merge/merge_cleaned_tables.sql`](./Analysis/Scripts/SQL/02_merge/merge_cleaned_tables.sql)

This script combines the cleaned quarterly datasets into a single table for analysis.

### 3. SQL Analysis
**Location:** [`Analysis/Scripts/SQL/03_statistical_analysis/`](./Analysis/Scripts/SQL/03_statistical_analysis/)

This folder contains SQL queries used to analyze rider behavior:
- [`avg_ride_length.sql`](./Analysis/Scripts/SQL/03_statistical_analysis/avg_ride_length.sql)
- [`monthly_rides.sql`](./Analysis/Scripts/SQL/03_statistical_analysis/monthly_rides.sql)
- [`time_of_day.sql`](./Analysis/Scripts/SQL/03_statistical_analysis/time_of_day.sql)
- [`trips_per_member_type.sql`](./Analysis/Scripts/SQL/03_statistical_analysis/trips_per_member_type.sql)

The analysis focuses on:
- ride duration
- member versus casual usage
- time-of-day behavior
- monthly ride trends

### 4. R Workflow
**Location:** [`Analysis/Scripts/R/cyclistic_workflow.R`](./Analysis/Scripts/R/cyclistic_workflow.R)

This script supports the analysis by reproducing the workflow in R and summarizing key patterns.

## Key Findings
- Casual riders generally take longer rides than annual members.
- Casual rider activity is higher on weekends and during warmer periods.
- Members use the service more consistently on weekdays.
- Usage patterns suggest different purposes for each rider type.

## Reports
- **Executive Summary (PDF):** [`Reports/Cyclistic_Analysis_Markdown.pdf`](./Reports/Cyclistic_Analysis_Markdown.pdf)
- **Technical Report (Markdown):** [`Reports/Cyclistic_Markdown.md`](./Reports/Cyclistic_Markdown.md)

## Data Source
The analysis uses publicly available Cyclistic (Divvy) trip data. Raw source files are not included in this repository due to size constraints. The SQL scripts assume the original data has already been loaded into a database environment.

## Limitations
This analysis is based on trip history data only. It does not include demographic information or direct evidence of rider motivation, so interpretations about commuting or leisure behavior should be treated as informed usage patterns rather than confirmed intent.

## Notes
AI tools were used selectively for brainstorming, editing, and improving documentation clarity. All analysis logic, SQL/R workflows, interpretation, and final conclusions were reviewed and validated by me.
