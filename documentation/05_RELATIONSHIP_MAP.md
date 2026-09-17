# NEXORA Relationship Map

## Star schema

### FactSales
1. FactSales[OrderDate] -> DimDate[Date]
2. FactSales[ProductID] -> DimProduct[ProductID]
3. FactSales[CustomerID] -> DimCustomer[CustomerID]
4. FactSales[EmployeeID] -> DimEmployee[EmployeeID]
5. FactSales[RegionID] -> DimRegion[RegionID]
6. FactSales[ChannelID] -> DimChannel[ChannelID]

### FactInventory
7. FactInventory[SnapshotDate] -> DimDate[Date]
8. FactInventory[ProductID] -> DimProduct[ProductID]
9. FactInventory[RegionID] -> DimRegion[RegionID]

### FactTargets
10. FactTargets[TargetMonth] -> DimDate[Date]
11. FactTargets[RegionID] -> DimRegion[RegionID]
12. FactTargets[CategoryKey] -> DimCategory[CategoryKey]

All 12 are intended to be active, one-to-many, single-direction relationships from the dimension/one side to the fact/many side.

## Important modeling note
DimCategory is intentionally connected to FactTargets, not directly to DimProduct, because the supplied project specification explicitly defines 12 relationships. For sales category visuals, use DimProduct[Category] (or DimProduct[Subcategory]) rather than assuming DimCategory filters FactSales.