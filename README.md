# ETL_Pipeline
## Automated ETL Pipeline for Monthly Sales Data
This project implements a fully automated ETL (Extract, Transform, Load) pipeline that processes monthly sales data, ensures data quality, eliminates duplicates, and automatically refreshes Power BI reports. The solution leverages Microsoft Fabric Lakehouse, Dataflows, Power BI Desktop and Service, and Pipelines to automate data ingestion, transformation, and loading processes.

### Table of Contents
Overview

*Features

*Challenges Addressed

*Technologies Used

*Architecture

*ETL Process

*Power BI Integration

*Automation with Fabric Pipelines

*Setup Instructions

*Contributing


### Overview
The goal of this project is to build a robust, automated, and scalable ETL pipeline for handling and processing monthly sales data. The pipeline performs the following functions:

Automatically ingests CSV files stored in a Microsoft Fabric Lakehouse.

Transforms the data by appending multiple CSV files into a single dataset and removing duplicate records.

Loads the cleaned dataset into Power BI for visualization and reporting.

Automates the entire workflow with Fabric Pipelines for seamless updates.

### Features
Data Ingestion: Monthly sales data files are stored in a structured folder within the Microsoft Fabric Lakehouse.

#### Dataflows:

Appender: Appends CSV files into a single dataset.

Duplicate Removal: Removes duplicate records to ensure clean, consistent data.

#### Power BI Integration:

Connects Power BI Desktop directly to the cleaned dataset for report creation.

Publishes the report to Power BI Service for sharing and online access.

#### Automation:

Automatically refreshes Dataflows and the Power BI Semantic Model using Fabric Pipelines whenever new data is added to the Lakehouse.

Challenges Addressed
Data Silos: Aggregating data from multiple separate files each month.

Manual Data Refresh: Reducing the manual effort required to update Power BI.

Duplicate Records: Eliminating duplicates from different CSV files to ensure data consistency.

Scalability: Designing a system that can handle increasing volumes of sales data.

Automation: Minimizing human intervention and reducing errors.

### Technologies Used
Microsoft Fabric Lakehouse

Dataflows

Power BI Desktop & Service

Pipelines

Architecture

### The architecture involves the following components:

Lakehouse: Stores the monthly sales data files in an organized, structured manner.

Dataflows:

Appends CSV files into a unified dataset.

Cleanses the data by removing duplicates.

#### Power BI:

Visualizes the cleaned data.

Publishes reports to Power BI Service.

Fabric Pipelines: Automates the ETL workflow, including data ingestion, transformation, and report refresh.

ETL Process
Extract: Ingest CSV files containing monthly sales data from the Lakehouse.

#### Transform:

Append the data from different CSV files into one unified dataset.

Remove any duplicate records to ensure data integrity.

Load: Load the cleaned data into Power BI for visualization.

Power BI Integration
Power BI Desktop is directly connected to the cleaned dataset for building interactive dashboards and KPIs.

The report is then published to Power BI Service for online access and sharing with stakeholders.

Automation with Fabric Pipelines
The entire ETL process is automated with Microsoft Fabric Pipelines.

Each new file added to the Lakehouse triggers an automatic refresh of the dataflows and the Power BI report, ensuring that the data is always up-to-date without manual intervention.

### Setup Instructions
Prerequisites
Microsoft Fabric account

Power BI account

Access to Fabric Lakehouse and Pipelines

#### Steps
Data Storage: Upload monthly sales data CSV files to the Lakehouse.

Create Dataflows:

Create Dataflow 1 (Appender) to combine the CSV files into one dataset.

Create Dataflow 2 (Duplicate Removal) to cleanse the data.

Power BI Integration:

Connect Power BI Desktop to Dataflow 2 for reporting.

Publish the report to Power BI Service.

Set Up Pipelines:

Create a Fabric Pipeline to automate the refresh process.

### Test: Verify that each new file triggers the ETL process and refreshes the Power BI report.

## Contributing
Feel free to fork this repository and submit issues or pull requests. Contributions are welcome to improve the system and add new features.
