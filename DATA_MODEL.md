# NEXORA Data Model

## Architecture

NEXORA uses a star-schema semantic model with 8 dimension tables and 3 fact tables.

### Dimensions
- DimDate
- DimCategory
- DimSubcategory
- DimRegion
- DimChannel
- DimProduct
- DimCustomer
- DimEmployee

### Facts
- FactSales
- FactInventory
- FactTargets

## Relationships

All 12 documented relationships are one-to-many and single-direction from dimension to fact:

1. FactSales[OrderDate] → DimDate[Date]
2. FactSales[ProductID] → DimProduct[ProductID]
3. FactSales[CustomerID] → DimCustomer[CustomerID]
4. FactSales[EmployeeID] → DimEmployee[EmployeeID]
5. FactSales[RegionID] → DimRegion[RegionID]
6. FactSales[ChannelID] → DimChannel[ChannelID]
7. FactInventory[SnapshotDate] → DimDate[Date]
8. FactInventory[ProductID] → DimProduct[ProductID]
9. FactInventory[RegionID] → DimRegion[RegionID]
10. FactTargets[TargetMonth] → DimDate[Date]
11. FactTargets[RegionID] → DimRegion[RegionID]
12. FactTargets[CategoryKey] → DimCategory[CategoryKey]

## Modeling approach

The model separates descriptive dimensions from transactional, inventory and target facts. This supports reusable DAX measures, consistent filtering and interactive analysis across the five report pages.
