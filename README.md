# Cyclistic Bike-Share Analysis 🚴‍♀️

## Project Overview
**Goal:** Design marketing strategies to convert casual riders into annual members by analyzing historical bike trip data.
**Role:** Data Analyst
**Tools:** SQL (Data Cleaning & Analysis), R (Statistical Analysis), Tableau (Visualization)

## 📂 Repository Structure

This project follows a structured data pipeline:

### 1. Data Cleaning (SQL)
Located in: `Analysis/Scripts/SQL/01_cleaning/`
* Raw data from 2019/2020 was imported and standardized.
* Scripts handle null value removal, column renaming, and consistent formatting across quarters.

### 2. Data Merging (SQL)
Located in: `Analysis/Scripts/SQL/02_merge/`
* **`merge_cleaned_tables.sql`**: Combines the cleaned quarterly tables into a single master dataset for analysis.

### 3. Analysis (SQL & R)
* **SQL Analysis:** `Analysis/Scripts/SQL/03_statistical_analysis/`
    * Calculates key metrics: Average ride length, member vs. casual usage by day of week, and monthly trends.
* **R Verification:** `Analysis/Scripts/R/cyclistic_workflow.R`
    * Performs validation checks and advanced statistical summary on the processed data.

## 📊 Final Reports

The complete findings, visualizations, and business recommendations are available here:

* 📄 **Executive Summary (PDF):** [View PDF Report](./Reports/Cyclistic_Analysis_Markdown.pdf)
* 📝 **Technical Report (Markdown):** [View Analysis Log](./Reports/Cyclistic_Markdown.md)

---

### Data Source
*Note: The raw datasets used for this analysis are not included in this repository due to size constraints. The logic provided in the `Scripts` folder assumes the raw data is loaded into a SQL database.*
