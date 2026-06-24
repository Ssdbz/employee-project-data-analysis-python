# Employee Project Analytics using Python

## Overview

This project demonstrates an end-to-end data analysis workflow using Python, Pandas, and NumPy on an employee-project management dataset.

The objective was to transform raw organizational data into actionable insights by performing data cleaning, missing value treatment, feature engineering, business rule implementation, and employee performance analysis.

The project simulates a real-world business environment where employee records, project information, and designation hierarchies are maintained across multiple datasets and must be integrated to support decision-making.

---

## Business Problem

Organizations often maintain employee, project, and hierarchy information in separate systems. Incomplete records, missing project costs, inconsistent naming conventions, and performance-based designation updates can make reporting difficult.

This project addresses these challenges by:

* Cleaning and standardizing employee records
* Handling missing project cost information
* Integrating data from multiple sources
* Automating bonus calculations
* Evaluating employee performance based on project outcomes
* Tracking designation promotions and demotions
* Generating employee-level project cost summaries

---

## Dataset Information

The analysis is based on three datasets:

### Employee Dataset

Contains employee demographic information.

| Column | Description         |
| ------ | ------------------- |
| ID     | Employee Identifier |
| Name   | Employee Name       |
| Gender | Gender              |
| City   | Employee Location   |
| Age    | Employee Age        |

### Project Dataset

Contains project-level information.

| Column  | Description         |
| ------- | ------------------- |
| ID      | Employee Identifier |
| Project | Project Name        |
| Cost    | Project Cost        |
| Status  | Project Status      |

### Seniority Dataset

Contains employee designation hierarchy.

| Column            | Description         |
| ----------------- | ------------------- |
| ID                | Employee Identifier |
| Designation Level | Organizational Rank |

---

## Project Workflow

### Data Preparation

* Created structured DataFrames from raw tabular data
* Exported datasets into CSV format
* Loaded datasets using Pandas

### Missing Value Treatment

Project cost information contained missing values.

Implemented a Running Average Imputation technique using Python loops to estimate missing project costs while preserving dataset consistency.

### Data Transformation

Performed multiple transformation operations including:

* Splitting employee names into First Name and Last Name
* Standardizing employee naming conventions
* Creating honorific prefixes (Mr./Mrs.)

### Data Integration

Merged Employee, Project, and Seniority datasets into a consolidated analytical dataset for reporting and business analysis.

### Feature Engineering

Generated new analytical attributes including:

* Employee Bonus
* Updated Designation Level
* Total Project Cost
* Employee Performance Indicators

---

## Business Rules Implemented

### Bonus Calculation

Employees who successfully completed projects received:

Bonus = 5% × Project Cost

### Designation Demotion

Employees associated with failed projects were penalized by reducing their designation hierarchy.

### Promotion Policy

Employees older than 29 years were promoted according to predefined business rules.

### Eligibility Check

Employees whose designation level exceeded the permissible threshold were removed from the active employee dataset.

---

## Analytical Outcomes

The project produced:

* Cleaned and standardized employee records
* Consolidated reporting dataset
* Employee bonus calculations
* Designation adjustment reports
* Employee-wise project expenditure analysis
* Location-based employee filtering

---

## Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook

---

## Repository Structure

```text
employee-project-data-analysis-pandas/
│
├── data/
│   ├── Employee.csv
│   ├── Project.csv
│   └── Seniority.csv
│
├── notebooks/
│   └── Employee_Project_Analysis.ipynb
│
├── outputs/
│   ├── Final.csv
│   └── TotalProjCost.csv
│
├── README.md
└── requirements.txt
```

## Skills Demonstrated

* Data Cleaning
* Data Wrangling
* Missing Value Imputation
* Feature Engineering
* Data Integration
* Business Rule Implementation
* Exploratory Data Analysis
* Pandas Data Manipulation
* Python Programming
* Reporting Automation

---

## Key Learnings

Through this project, I strengthened my understanding of:

* Real-world data preprocessing techniques
* Data transformation workflows
* Employee performance analytics
* Aggregation and reporting using Pandas
* Business-driven decision logic implementation
* Building reproducible data analysis pipelines

---

## Future Enhancements

* Interactive Power BI Dashboard
* SQL Database Integration
* Automated Reporting Pipeline
* Employee Performance KPI Dashboard
* Data Visualization using Matplotlib and Seaborn

---

### Author

**Souvik Sen**
