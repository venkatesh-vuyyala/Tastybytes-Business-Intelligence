# Tastybytes-Business-Intelligence
 ### Interactive Data Visualization and Insights with Snowflake and Tableau

## Project Overview
This project involves creating a data pipeline for Frostbyte Tasty Bytes, leveraging Snowflake for data warehousing and Tableau for data visualization. The pipeline includes data ingestion, transformation, analysis, enrichment, and visualization, providing comprehensive insights into the company's sales data.

## Architectute

![Tastybytes_Architecture](https://github.com/user-attachments/assets/7589cf04-2886-4b4d-863f-48a6a643d641)

## Data Ingestion

### Loading Data from S3 to Snowflake

1. Stage Setup:
- Configure Snowflake stages to connect to Amazon S3.
- Set up file formats to correctly interpret CSV data.

2. Copy Data:
- Used Snowflake's COPY INTO command to load data from S3 into Snowflake tables.

## Data Transformation

### Creating Raw Zone Tables

1. POS Data:
- Created a raw table for Point of Sale (POS) data.
- Loaded data into the POS table from the staged files.
  
2. Customer Data:
- created a raw table for customer data.
- Loaded data into the customer table from the staged files.

### Creating Harmonized Views

1. POS Harmonized View:
- Created a view to standardize and harmonize the POS data.

2. Customer Harmonized View:
- Created a view to standardize and harmonize the customer data.

### Creating Analytics Views

1. Sales Summary View:
- Created a view to summarize sales data, including total quantity sold and total amount sold.
- Joined POS data with customer data for enriched analytics.

## Data Analysis

### Investigating Zero Sales Days
1. Zero Sales Days View:
- Created a view to identify days with zero sales across stores.
- Aggregated and analyzed the zero sales data to determine patterns or issues.

## Data Enrichment

### Integrating Weather Data

1. Acquire Weather Data:
- Obtained weather data from the Snowflake Marketplace.
- Created a view to include weather data alongside sales data for comprehensive analysis.
  
2. Integrate Geospatial Data:
- Obtained geospatial data to include latitude and longitude of stores from snowflake marketplace
- Created a view to combine geospatial data with sales data for enhanced geographic analysis.

## Data Visualization

### Tableau Integration

- Developed various visualizations, such as bar charts, line charts, and maps.
- Combined visualizations into interactive dashboards.

  <img width="1001" alt="Tastybytes_dashboard" src="https://github.com/user-attachments/assets/c981c141-6ba7-4549-a95b-318045c4a430">

  
