# Adidas Sales Analysis

This repository contains a comprehensive workflow for analyzing Adidas sales data, from raw Excel data cleaning to advanced dashboarding in Power BI. The project demonstrates best practices in data preparation, transformation, and visualization.

## Table of Contents

- [Overview](#overview)
- [Workflow Summary](#workflow-summary)
  - [1. Excel Data Cleaning](#1-excel-data-cleaning)
  - [2. Power Query Transformation](#2-power-query-transformation)
  - [3. Power BI Dashboarding](#3-power-bi-dashboarding)
- [Project Files](#project-files)
- [Getting Started](#getting-started)
- [License](#license)

---

## Overview

Adidas Sales Analysis is designed to turn raw sales data into actionable insights. It uses Microsoft Excel for initial data cleaning, Power Query for transformation, and Power BI for interactive dashboards.

## Workflow Summary

### 1. Excel Data Cleaning

- **Import Raw Data:** Start with the Adidas sales data in Excel format.
- **Remove Duplicates:** Identify and remove duplicate rows to ensure data integrity.
- **Handle Missing Values:** Use Excel functions to fill or remove missing data.
- **Standardize Formats:** Ensure consistent formatting for dates, currencies, and product names.
- **Basic Calculations:** Add calculated columns (e.g., total sales, profit margins) using formulas.

### 2. Power Query Transformation

- **Load Data into Power Query:** Import the cleaned Excel file into Power Query (via Excel or Power BI).
- **Transform Columns:** 
  - Change data types as needed (dates, text, numbers).
  - Split and merge columns for better structure.
  - Filter irrelevant records.
- **Generate Output Table:** Export the transformed table for Power BI reporting.

### 3. Power BI Dashboarding

- **Import Transformed Data:** Load the Power Query output into Power BI.
- **Model Relationships:** Define relationships between tables (e.g., sales, products, regions).
- **Create Visualizations:** 
  - Sales trends by month, region, and product.
  - Top performing products and regions.
  - Profit and revenue breakdowns.
  - Interactive filters and slicers.
- **Publish and Share:** Deploy dashboards for stakeholder access.

## Project Files

- `/data/Adidas US Sales Datasets.xlsx` —  Cleaned and Transformed Sales Data
- `/powerbi/Adidas_Sales_Dashboard.pbix` — Power BI dashboard.

## Getting Started

1. **Clone the repository:**
   ```
   git clone https://github.com/DeepakVeerelli/Adidas-Sales-Analysis.git
   ```

2. **Open `/data/US Sales Datasets.xlsx` in Excel to review the cleaned and transformed sales data.**  
   (If you want to perform your own cleaning and transformation, start with your raw dataset and follow the steps in the [Workflow Summary](#workflow-summary).)

3. **If you perform your own data transformation using Power Query:**  
   - Open your dataset in Excel or Power BI.
   - Use Power Query to clean, structure, and transform the data as described in the workflow.
   - **Export or save** the transformed dataset as an Excel file (e.g., `/data/US Sales Datasets.xlsx`).

4. **Import the cleaned and transformed data (`/data/US Sales Datasets.xlsx`) into Power BI:**
   - Open Power BI Desktop.
   - Click "Get Data" > "Excel Workbook" and select the cleaned dataset.
   - Load the data and set up relationships if needed.

5. **Build dashboards in Power BI:**
   - Use the imported data to create interactive visualizations.
   - Optionally, reference `/powerbi/Adidas_Sales_Dashboard.pbix` for a sample dashboard layout and visuals.

6. **Publish and share your Power BI dashboard with stakeholders as needed.**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
