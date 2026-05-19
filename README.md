# LifeTechs-Analysis
To dowmnload the dashboard: https://aswu-my.sharepoint.com/:u:/g/personal/hoda_abdallah_stu_agr_aswu_edu_eg/IQAlCg5GZU-mRJjTo51Bi2IEAQ5uUDYqdM9NsUhi8dCe71o?e=GKVwJy

## Turning Business Data into Strategic Insights

A complete Business Intelligence and Data Analysis project developed for a smart home solutions company using Power BI, SQL, Power Query, DAX, and BigQuery.

This project transforms raw CRM and sales data into interactive dashboards and actionable business insights that support strategic decision-making.

---

# Project Overview

LifeTech is a smart home solutions company specializing in:

- Smart Lighting
- Home Cinema
- Smart HVAC
- Full Automation
- Security Systems

The company faced major challenges in:
- Unstructured Excel data
- Missing values
- Duplicate records
- Poor reporting visibility
- Difficulty tracking business performance

This project was built to solve these challenges through a complete Business Intelligence workflow.

---

# Business Objectives

The project aimed to:

- Build a structured analytical environment
- Clean and transform raw business data
- Improve business visibility
- Develop interactive dashboards
- Analyze sales and marketing performance
- Identify customer feedback patterns
- Support forecasting
- Generate strategic business recommendations

---

# Tools & Technologies

- Power BI
- SQL
- Google BigQuery
- Power Query
- DAX
- Excel

---

# Data Sources

The datasets were extracted from the company's CRM system and included:

- Customers Data
- Sales Data
- CRM Feedback
- Sales Team Performance
- Detailed Sales Reports

---

# Data Cleaning Process

The raw data required extensive preprocessing before analysis.

### Main Cleaning Steps:
- Removed duplicate records
- Handled missing values
- Standardized column names
- Unified date and text formats
- Corrected inconsistent values
- Filtered irrelevant records

---

# SQL & BigQuery Processing

SQL queries were used to:

- Merge datasets
- Create analytical views
- Calculate profit metrics
- Filter cancelled orders
- Prepare data for Power BI

Google BigQuery was used for cloud-based data processing.

---

# Power Query Transformations

Power Query was used for:

- Cleaning columns
- Standardizing data types
- Sorting and filtering records
- Creating structured analytical tables
- Preparing fact and dimension tables

---

# Data Modeling

A Star Schema model was created in Power BI.

### Main Components:

## Fact Table
- Sales_Details

## Dimension Tables
- DimCity
- DimLeadSource
- DimHousingType
- DimServiceName
- DimAgent
- Calendar Table
- Feedback Tables

### Benefits:
- Faster analysis
- Better dashboard performance
- Accurate filtering
- Cross-functional business insights

---

# DAX Measures & KPIs

Several DAX measures were created, including:

```DAX
Total Revenue = SUM(Sales_details[ContractValue])

Net Operating Profit = [Total Revenue] - [Total Operational Cost]

Profit Margin % = DIVIDE([Net Operating Profit], [Total Revenue], 0)

Current Year Revenue = TOTALYTD([Total Revenue], Calendar[Date])
