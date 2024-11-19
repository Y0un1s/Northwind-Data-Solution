# Northwind-ETL-and-Analytics

## Overview
The **Northwind-ETL-and-Analytics** project is a robust data warehouse implementation for the Northwind Traders dataset. It is designed to provide insights into business operations, focusing on sales, inventory, and customer behavior, using well-structured data models, automated ETL pipelines, and interactive dashboards.
## Demo Video
[![Watch the video](https://user-images.githubusercontent.com/74038190/235294007-de441046-823e-4eff-89bf-d4df52858b65.gif)](https://github.com/Y0un1s/Northwind-Data-Solution/blob/main/Northwind%20Data%20Solution%20Demo.mp4)

## Features
- **Data Modeling**:
  - Conceptual, logical, and physical models implemented for organizing data.
  - Snowflake schema design for flexibility and optimized storage.
- **ETL Process**:
  - Automated pipelines using SSIS (SQL Server Integration Services) for extracting, transforming, and loading data.
  - Scheduled jobs for daily updates to ensure data consistency.
- **Analytics and Reporting**:
  - Power BI dashboards to visualize business performance metrics like sales trends, inventory levels, and customer insights.

## Components
### 1. **Fact Table**
- **Fact_Orders**: Contains transactional data, such as order details, shipping, and discounts.

### 2. **Dimension Tables**
- **Dim_Product**: Details about products.
- **Dim_Category**: Product categorization data.
- **Dim_Customer**: Customer profiles and demographics.
- **Dim_Employee**: Employee details, roles, and regional information.
- **Dim_Supplier**: Supplier data.
- **Dim_Shipper**: Shipping company details.
- **Dim_Territory**: Information on territories and regions.
- **Dim_Date**: A time dimension for tracking trends over days, months, and years.

### 3. **ETL Process**
- **ODS (Operational Data Store)**: A temporary area for raw data before processing.
- **Staging Area**: Data is cleaned, filtered, and transformed to align with the warehouse schema.
- **Data Warehouse**: Final, structured storage using a snowflake schema.

## Architecture
1. **Data Integration**: Data is extracted from the Northwind OLTP database, transformed to match the snowflake schema, and loaded into the warehouse.
2. **ETL Automation**: SSIS packages automate the data refresh process, ensuring timely updates.
3. **Analytics**: Power BI dashboards provide dynamic visualizations of key performance indicators.

## Key Design Decisions
- **Normalized Dimensions**: Dimensions are separated to avoid redundancy and ensure flexibility in querying.
- **Column Optimization**: Unnecessary columns (e.g., `Picture` and `HomePage`) were removed to streamline the data warehouse.

## Analytics Dashboards
- **Sales Trends**: Analyze sales data over time.
- **Inventory Management**: Monitor stock levels and product performance.
- **Customer Insights**: Segment and analyze customer behavior.
- **Employee Performance**: Evaluate order management efficiency by employees.

## Project Workflow
| **Task**              | **Assigned Members**            | **Priority** | **Status**    | **Start Date** | **End Date**   |
|-----------------------|----------------------------------|--------------|---------------|----------------|----------------|
| Business Requirements | Ahmed Fawzy                    | P0           | Completed     | 2024-09-29     | 2024-09-29     |
| Data Modeling         | Ahmed Fawzy, Ahmed Younis      | P0           | Completed     | 2024-09-29     | 2024-09-30     |
| ETL Development       | Ahmed Younis, Ebrahim Ayman    | P0           | Completed     | 2024-10-01     | 2024-10-04     |
| Analysis              | Ahmed Fawzy, Fouad Khaled      | P1           | Completed     | 2024-10-03     | 2024-10-04     |

## How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Y0un1s/Northwind-Data-Solution.git
