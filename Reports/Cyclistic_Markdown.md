# Cyclistic Bike-Share Analysis

## Project Overview
This project examines behavioral differences between casual riders and annual members using Cyclistic bike-share trip data. The objective is to identify usage patterns that could support marketing decisions focused on increasing annual memberships.

## 1. Business Task
Analyze how annual members and casual riders use Cyclistic bikes differently in order to identify patterns that could support membership growth strategies.

## 2. Data Source
The analysis uses 12 months of publicly available trip data from the Cyclistic (Divvy) bike-share system.

The dataset includes:
- ride IDs
- ride start and end times
- station names
- bike types
- rider types

Personal identifiers were removed in the original source data, making it suitable for behavioral analysis.

## 3. Data Preparation
**Tools used:** SQL and R

Main preparation steps:
- imported and standardized quarterly trip files
- aligned column names and data types across tables
- converted timestamps into consistent datetime format
- calculated ride length
- extracted day-of-week values
- removed records with missing key fields
- filtered out negative or unrealistic ride durations
- merged cleaned tables into a single dataset for analysis

## 4. Analysis Approach
The analysis compares casual riders and annual members across:
- ride duration
- weekday versus weekend activity
- monthly ride patterns
- time-of-day behavior
- overall ride volume

This approach helps identify both behavioral differences and broader usage trends over time.

## 5. Key Findings
- Casual riders generally take longer rides than annual members.
- Casual rider activity is higher on weekends.
- Members ride more consistently on weekdays.
- Casual rider activity increases during warmer months.
- Members show more stable usage across the year.

## 6. Interpretation
The results suggest that the two rider groups use the bike-share service differently.

- **Members** appear more likely to use bikes for routine transportation and weekday travel.
- **Casual riders** appear more likely to use bikes for leisure, seasonal outings, or less regular trips.

These differences are reflected in ride duration, weekly usage patterns, and seasonal trends.

## 7. Recommendations
1. Increase membership promotion during periods of higher casual rider activity, especially in warmer months.
2. Emphasize the practical value of membership for riders who use the service regularly, particularly around convenience and cost.
3. Test introductory offers or short-term membership trials for casual riders who show repeat usage patterns.
4. Tailor marketing messages by use case, separating weekday utility-focused messaging from weekend leisure-focused messaging.

## 8. Limitations
This analysis is based on trip history data only. It does not include demographic information or direct evidence of rider motivation, so interpretations about commuting or leisure behavior should be treated as informed patterns rather than confirmed intent.

## 9. Tools Used
- **SQL** for cleaning, filtering, merging, and aggregation
- **R** for validation, transformation, and summary analysis
- **Spreadsheets** for supporting review and inspection