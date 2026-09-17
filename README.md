# NEXORA — Sales & Operations Performance Intelligence

![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Analytics-00A4EF)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-5C2D91)

A five-page Microsoft Power BI portfolio project for analyzing sales, profitability, targets, customers, regions, channels and inventory.

> **Portfolio project:** This repository documents and demonstrates the technical work. It does not represent paid client work or claim business results for a real client.

## Dashboard

### 1. Executive Overview
![Executive Overview](screenshots/01_Executive_Overview.png)

### 2. Sales Performance
![Sales Performance](screenshots/02_Sales_Performance.png)

### 3. Operations & Inventory
![Operations & Inventory](screenshots/03_Operations_Inventory.png)

### 4. Regional & Customer Intelligence
![Regional & Customer Intelligence](screenshots/04_Regional_Customer_Intelligence.png)

### 5. Management Insights
![Management Insights](screenshots/05_Management_Insights.png)

## Project Scope

The report provides:

- Revenue and gross-profit analysis
- Gross margin and AOV
- Target achievement and target variance
- Revenue growth
- Regional and category analysis
- Channel and sales-representative performance
- Product performance
- Customer segmentation and value analysis
- Inventory value and stock-on-hand analysis
- Low-stock and stockout monitoring
- Inventory risk
- Fast and slow movers
- Management-oriented insight views

## Technical Skills Demonstrated

### Power BI
- Interactive multi-page reporting
- KPI dashboards
- Slicers and visual interactions
- Executive dashboard design

### DAX
- Aggregation measures
- `CALCULATE`
- `DIVIDE`
- `DISTINCTCOUNT`
- `DATEADD`
- `ADDCOLUMNS`
- `VALUES`
- `FILTER`
- Filter-context management

### Data Modeling
- Star-schema architecture
- Fact/dimension modeling
- Date dimension
- Product, customer, employee, region, channel and category dimensions
- One-to-many relationship modeling

### Data Analysis
- Sales
- Profitability
- Targets
- Customers
- Regions
- Products
- Channels
- Inventory

### Data Quality
- Transaction-level reconciliation
- KPI validation
- Date validation
- Order-status validation

## Model

The semantic model contains 11 tables:

**Dimensions**
- DimDate
- DimCategory
- DimSubcategory
- DimRegion
- DimChannel
- DimProduct
- DimCustomer
- DimEmployee

**Facts**
- FactSales
- FactInventory
- FactTargets

See [`documentation/Data_Model.md`](documentation/Data_Model.md) for the relationship map.

## KPI Catalog

See [`documentation/KPI_Definitions.md`](documentation/KPI_Definitions.md).

## QA

See [`documentation/QA_Validation.md`](documentation/QA_Validation.md).

## Project Structure

```text
.
├── README.md
├── PORTFOLIO_DESCRIPTION.md
├── GITHUB_PUBLICATION_CHECKLIST.md
├── screenshots/
├── powerbi/
├── dax/
└── documentation/
```

## Data & Reproducibility

The public package intentionally does **not** include the source Excel workbook.

The PBIP uses a local Excel source during development. Before publishing a publicly runnable PBIP, verify that the source data may be shared and update the source connection if necessary.

## Author

**Brian Maobe Onyancha**

Portfolio focus: **Data Analysis • Power BI • DAX • Business Intelligence • Dashboard Development**
