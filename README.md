# Adidas Sales Analysis

This project provides an end-to-end workflow for analyzing Adidas sales data, leveraging Excel (Power Query) for data cleaning and transformation, and Power BI for building dynamic, interactive dashboards powered by DAX formulas. The objective is to empower stakeholders with actionable insights, enabling smarter decisions across products, regions, and overall sales performance.

## Table of Contents
- [Overview](#overview)
- [Workflow](#workflow)
- [Dataset](#dataset)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Power BI Dashboards](#power-bi-dashboards)
- [DAX Formulas](#dax-formulas)
- [Results & Insights](#results--insights)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

## Overview
Transform raw Adidas sales data into actionable business intelligence by:
- Cleaning and standardizing data in Excel using Power Query
- Calculating KPIs (e.g., total revenue, units sold, sales growth) with DAX formulas
- Visualizing key trends and metrics in Power BI dashboards

## Workflow
1. Import raw sales data into Excel
2. Clean and transform data using Power Query
3. Export the cleaned data to Power BI
4. Create DAX measures for dynamic KPIs and trend
5. Build interactive dashboards,filters, drill-throughs, time-series analysis
7. Generate insights into sales, regional, and product performance

## Dataset
- **Format:** Excel
- **Fields:** Invoice Date,Product, Units Sold and more
- **Location:** See the sample files

## Data Cleaning & Preparation (Excel Power Query)
**Key Steps:**
- Remove duplicates
- Creates related columns
- Standardize date and numeric formats
- Address missing or invalid values
- Merge and group data where required

**How To:**
- Open Excel → Data > Get & Transform Data
- Use Power Query Editor to clean and shape your data
- Export the result as `.xlsx` or `.csv` for Power BI import

## Power BI Dashboards
**Dashboards include:**
- **Sales Overview:** Total revenue, units sold, profit trends
- **Top Products & Regions:** Performance rankings
- **Filters & Drill-throughs:** Deep-dives by category or region
- **Custom Visuals:** Slicers, tooltips, cards for interactive analysis

Check the `PowerBi dashboards/` folder for `.pbix` files or screenshots.

## DAX Formulas
Sample DAX measures used in Power BI:

```dax
Total Customers = COUNTROWS(telecom_combined)
Average MonthlyCharges = AVERAGE(telecom_combined[MonthlyCharges])
Churned customers = CALCULATE(COUNTROWS(telecom_combined),telecom_combined[Churn]="Yes")
Churned Rate = DIVIDE([Churned customers],[Total Customers])
)
```

## Results & Insights
This analysis reveals:
- Top-performing regions and product categories
- Opportunities for inventory planning and marketing optimization
- Recommendations to focus on high-margin regions and bundled offers

## How to Use
1. Clone the repository or download as ZIP
2. Place your raw sales file in the `data/` folder
3. Open `Adidas_Sales_Cleaning.xlsx` and clean data using Power Query
4. Load the cleaned data into `Adidas_Sales_Analysis.pbix`
5. Explore dashboards and DAX measures for insights

## Contributing
Contributions are welcome! You can:
- Add sample datasets
- Suggest improved visuals or KPIs
- Report or fix data transformation bugs

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

**Author:** Deepak Veerelli  
**Repository:** [Adidas Sales Analysis](https://github.com/DeepakVeerelli/Adidas-Sales-Analysis)
