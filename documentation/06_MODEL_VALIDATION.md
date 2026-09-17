# NEXORA Model Validation

## Source validation — executed against the supplied CSV source package

| Check | Result |
|---|---:|
| Dimension primary keys unique | PASS |
| Dimension primary keys non-null | PASS |
| FactSales foreign keys valid | PASS |
| FactInventory foreign keys valid | PASS |
| FactTargets foreign keys valid | PASS |
| DimDate continuous | PASS |
| DimDate unique | PASS |
| Revenue row reconciliation | PASS |
| Cost row reconciliation | PASS |
| Gross Profit row reconciliation | PASS |
| Margin row reconciliation | PASS |

## Source totals

| Metric | Expected |
|---|---:|
| Total Revenue | 886406692.3955 |
| Total Cost | 714027271.83 |
| Gross Profit | 172379420.5655 |
| Total Orders | 15000 |
| Completed Orders | 13968 |
| Units Sold | 45404 |
| Customers | 2000 |
| Target Revenue | 982636174.55 |
| Inventory Value | 1521265497.16 |
| Stock On Hand | 95164 |

## Status logic

- Completed: normal positive revenue and cost.
- Returned: negative revenue, positive cost.
- Cancelled: zero revenue and zero cost.

## Power BI acceptance criteria

- Tables = 11
- Relationships = 12
- Production measures = 43
- Problems = 0
- No duplicate relationships
- No duplicate tables
- No undefined measure references
- QA_QUERY_01 deltas = 0 within rounding tolerance
- QA_QUERY_02 mismatch counts = 0