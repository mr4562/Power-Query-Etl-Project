# Power Query Healthcare Claims Transformation Project
## Overview
This project demonstrates how Power Query can be used to clean, transform, and consolidate healthcare claims data.
The source dataset contains multiple claim rows for the same patient encounter. Using Power Query transformations, CPT codes and Modifiers are grouped and merged into consolidated fields.
## Problem Statement
The original dataset contains multiple records for the same patient and account:
| Patient | CPT |
|----------|----------|
| ALEKSOSKI VASIL | J0665 |
| ALEKSOSKI VASIL | J3301 |
| ALEKSOSKI VASIL | 20610 |
| ALEKSOSKI VASIL | J7324 |
| ALEKSOSKI VASIL | 20610 |
| ALEKSOSKI VASIL | 99213 |
The requirement was to transform the data into a single summarized record.
---
## Solution
Using Power Query:
- Imported raw claim data
- Grouped records by patient and account
- Combined CPT values
- Combined Modifier values
- Removed duplicates
- Generated a consolidated output table
---
## Before Transformation
![Original Data](Screenshots/Original_Data.png)
---
## After Transformation
![Final Output](Screenshots/Final_Output.png)
---
## Transformation Logic
### Group By
Grouped data using:
- Insurance Company
- DOS
- Account
- Patient Name
- Policy Number
### Aggregations
#### CPT Codes
Example:
J0665, J3301, 20610, J7324, 20610, 99213
#### Modifiers
Example:
*, JZ, 50, 25
---
## Tools Used
- Microsoft Excel
- Power Query
- Data Transformation
- ETL Process
---
## Business Benefits
- Reduces duplicate records
- Improves reporting accuracy
- Simplifies claim analysis
- Creates summarized datasets
- Saves manual processing time
---
## Project Files
| File | Description |
|--------|-------------|
| NJOI_Original_Data.xlsx | Raw input data |
| NJOI_Final_Output.xlsx | Final transformed data |
| Original_Data.png | Source data screenshot |
| Final_Output.png | Final output screenshot |
---
## Author
Mitesh Rana
Data Analyst | Excel Automation | Power Query Developer
