# zordering-medallion-pipeline
End-to-end Databricks Medallion Architecture project implementing Bronze, Silver, and Gold layers for employee, department, and salary data using PySpark and Delta tables.
This project demonstrates an end-to-end Medallion Architecture implementation in Databricks using PySpark.

## Architecture

Bronze Layer
- departments_raw
- employee_raw
- salaries_raw

Silver Layer
- employee_salary_summary

Gold Layer
- department_salary_summary
- monthly_salary_summary
- department_kpi

## Transformations

- Joined employee, department, and salary datasets
- Removed invalid employee records
- Imputed missing salaries using 70% of average salary
- Calculated department-wise salary benchmarks
- Generated bonus and final salary metrics
- Built Gold-layer business aggregations for reporting
