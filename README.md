# NEXORA — Sales & Operations Performance Intelligence

![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Analytics-00A4EF)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-5C2D91)

A five-page Microsoft Power BI portfolio project for analyzing sales, profitability, targets, customers, regions, channels and inventory.

> **Portfolio project:** This repository documents and demonstrates the technical work. It does not represent paid client work or claim business results for a real client.

## Dashboard

### 1. Executive Overview
![Executive Overview](01_Executive_Overview.png)

### 2. Sales Performance
![Sales Performance](02_Sales_Performance.png)

### 3. Operations & Inventory
![Operations & Inventory](03_Operations_Inventory.png)

### 4. Regional & Customer Intelligence
![Regional & Customer Intelligence](04_Regional_Customer_Intelligence.png)

### 5. Management Insights
![Management Insights](05_Management_Insights.png)

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

See [`DATA_MODEL.md`](DATA_MODEL.md) for the relationship map.

## Technical Artifacts

- [`dax/01_FINAL_DAX.dax`](dax/01_FINAL_DAX.dax) — production measures and KPI test output
- [`dax/04_QA_DAX_QUERIES.dax`](dax/04_QA_DAX_QUERIES.dax) — QA/reconciliation queries
- [`tmdl/02_FINAL_TMDL_MODEL.tmdl`](tmdl/02_FINAL_TMDL_MODEL.tmdl) — 12 relationship definitions
- [`tmdl/03_FINAL_TMDL_MEASURES.tmdl`](tmdl/03_FINAL_TMDL_MEASURES.tmdl) — production measure definitions
- [`theme/NEXORA_Cyberpunk_Theme.json`](theme/NEXORA_Cyberpunk_Theme.json) — report theme
- [`powerbi/README.md`](powerbi/README.md) — PBIP/PBIR project notes

## KPI Catalog

See [`KPI_DEFINITIONS.md`](KPI_DEFINITIONS.md) and [`documentation/08_FINAL_MEASURE_CATALOG.md`](documentation/08_FINAL_MEASURE_CATALOG.md).

## QA

See [`QA_VALIDATION.md`](QA_VALIDATION.md) and [`documentation/06_MODEL_VALIDATION.md`](documentation/06_MODEL_VALIDATION.md).

## Documentation

- [`documentation/05_RELATIONSHIP_MAP.md`](documentation/05_RELATIONSHIP_MAP.md)
- [`documentation/06_MODEL_VALIDATION.md`](documentation/06_MODEL_VALIDATION.md)
- [`documentation/07_DASHBOARD_BUILD_ORDER.md`](documentation/07_DASHBOARD_BUILD_ORDER.md)
- [`documentation/08_FINAL_MEASURE_CATALOG.md`](documentation/08_FINAL_MEASURE_CATALOG.md)
- [`documentation/09_FINAL_PORTFOLIO_README.md`](documentation/09_FINAL_PORTFOLIO_README.md)
- [`documentation/10_ONE_HOUR_BUILD_GUIDE.md`](documentation/10_ONE_HOUR_BUILD_GUIDE.md)

## Project Structure

```text
.
├── README.md
├── PORTFOLIO_DESCRIPTION.md
├── GITHUB_PUBLICATION_CHECKLIST.md
├── DATA_MODEL.md
├── KPI_DEFINITIONS.md
├── QA_VALIDATION.md
├── SKILLS_DEMONSTRATED.md
├── 01_Executive_Overview.png
├── 02_Sales_Performance.png
├── 03_Operations_Inventory.png
├── 04_Regional_Customer_Intelligence.png
├── 05_Management_Insights.png
├── dax/
├── tmdl/
├── theme/
├── documentation/
└── powerbi/
```

## Data & Reproducibility

The public package intentionally does **not** include the source Excel workbook. The source dataset remains read-only/source-of-truth material. Before publishing a publicly runnable PBIP, verify that the source data may be shared and update the source connection if necessary.

## Author

**Brian Maobe Onyancha**

Portfolio focus: **Data Analysis • Power BI • DAX • Business Intelligence • Dashboard Development**
