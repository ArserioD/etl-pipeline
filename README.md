This project demonstrates my ability to build scalable, governed, and data-driven pipelines that support accurate reporting, forecasting, and advanced analytics.


## Features

- **Robust Extraction:** Reads data from a CSV file with error handling and verification of the working directory.
- **Comprehensive Transformation:** Includes data cleaning (handling missing values, converting data types), standardization (e.g., lowercasing categorical fields), and enrichment (calculating derived fields like age).
- **Flexible Load Options:** Supports loading the transformed data into a new CSV file or into an SQLite database.
- **Error Handling & Logging:** Demonstrates a modular approach to pipeline design with proper error messages and logging.
- **Scalability & Automation Ready:** Designed with future improvement in mind, allowing easy integration with scheduling/orchestration tools (such as Apache Airflow) and CI/CD pipelines.



## Code Overview

etl_pipeline.py: Contains modular functions for each ETL step with detailed error handling:

extract_data(file_path): Reads and validates the CSV file.

transform_data(df): Cleans and enriches the DataFrame (e.g., fixing missing values, converting data types, creating derived columns).

load_data(df, output_path): Saves the processed data back to a CSV file.

Optional: Functions for loading data into a database (e.g., using SQLite).

Future Enhancements
Cloud Integration: Connecting to cloud storage data sources (S3/Azure Blob) for extraction.

Orchestration: Integrate with Apache Airflow for job scheduling, monitoring, and automated reporting.

Advanced Data Quality Checks: Incorporate automated validation checks and logging mechanisms.

Extended Data Sources: Combine additional datasets to build comprehensive, multi-dimensional analytical models.
