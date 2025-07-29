# Adidas Sales Analysis

This project provides an end-to-end workflow for analyzing Adidas sales data, leveraging Excel (Power Query) for robust data cleaning and transformation, and Power BI for building dynamic, interactive dashboards powered by DAX formulas. The objective is to empower stakeholders with actionable insights, enabling smarter decisions across products, regions, and overall sales performance.

## 📁 Table of Contents
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

## 🔍 Overview
Transform raw Adidas sales data into actionable business intelligence by:
- Cleaning and standardizing data in Excel using Power Query
- Visualizing key trends and metrics in Power BI dashboards
- Calculating KPIs (e.g., total revenue, units sold, sales growth) with DAX formulas

## 🔄 Workflow
1. Import raw sales data into Excel
2. Clean and transform data using Power Query
3. Export the cleaned data to Power BI
4. Build interactive dashboards—filters, drill-throughs, time-series analysis
5. Create DAX measures for dynamic KPIs and trends
6. Generate insights into sales, regional, and product performance

## 📊 Dataset
- **Format:** CSV or Excel
- **Fields:** Date, Region, Product, Units Sold, Revenue, Price, and more
- **Location:** See the `data/` folder for sample files

## 🧹 Data Cleaning & Preparation (Excel Power Query)
**Key Steps:**
- Remove duplicates
- Standardize date and numeric formats
- Address missing or invalid values
- Merge and group data where required

**How To:**
- Open Excel → Data > Get & Transform Data
- Use Power Query Editor to clean and shape your data
- Export the result as `.xlsx` or `.csv` for Power BI import

## 📈 Power BI Dashboards
**Dashboards include:**
- **Sales Overview:** Total revenue, units sold, profit trends
- **Top Products & Regions:** Performance rankings
- **Time-Series Analysis:** Monthly, quarterly, and yearly comparisons
- **Filters & Drill-throughs:** Deep-dives by category or region
- **Custom Visuals:** Slicers, tooltips, cards for interactive analysis

Check the `dashboards/` folder for `.pbix` files or screenshots.

## 📊 DAX Formulas
Sample DAX measures used in Power BI:

```dax
Total Sales = SUM('Sales'[Revenue])
Units Sold = SUM('Sales'[Units Sold])
Average Sales = AVERAGE('Sales'[Revenue])
Yearly Sales Growth = CALCULATE([Total Sales], DATESYTD('Sales'[Date]))
Top Product = CALCULATE(
    MAX('Sales'[Product]),
    FILTER('Sales', 'Sales'[Revenue] = [Total Sales])
)
```
Find additional measures and dynamic KPIs in the `dax/` folder.

## ✅ Results & Insights
This analysis reveals:
- Top-performing regions and product categories
- Periods with sales drop-offs or spikes
- Opportunities for inventory planning and marketing optimization
- Recommendations to focus on high-margin regions and bundled offers

## 🚀 How to Use
1. Clone the repository or download as ZIP
2. Place your raw sales file in the `data/` folder
3. Open `Adidas_Sales_Cleaning.xlsx` and clean data using Power Query
4. Load the cleaned data into `Adidas_Sales_Analysis.pbix`
5. Explore dashboards and DAX measures for insights

## 🤝 Contributing
Contributions are welcome! You can:
- Add sample datasets
- Suggest improved visuals or KPIs
- Report or fix data transformation bugs

## 📜 License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

**Author:** Deepak Veerelli  
**Repository:** [Adidas Sales Analysis](https://github.com/DeepakVeerelli/Adidas-Sales-Analysis)
