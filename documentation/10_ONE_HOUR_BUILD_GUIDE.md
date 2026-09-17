# NEXORA — ONE-HOUR BUILD GUIDE

## 00–10 min — Import
1. Open Power BI Desktop current release.
2. Import Project_02_Nexora_Sales_Operations_READY.xlsx.
3. Confirm all 11 tables load.
4. Open Model view and inspect automatic relationships.

## 10–20 min — Model + measures
1. Open TMDL View.
2. Paste 02_FINAL_TMDL_MODEL.tmdl.
3. Preview changes.
4. If Power BI already auto-created an identical relationship, keep the existing relationship and do not create the duplicate.
5. Apply only after Problems = 0.
6. Open a new TMDL tab.
7. Paste 03_FINAL_TMDL_MEASURES.tmdl.
8. Preview, verify measure count, Apply.

## 20–25 min — QA
1. Open DAX Query View.
2. Run 04_QA_DAX_QUERIES.dax query by query.
3. QA_QUERY_01 deltas must be 0 within normal floating-point rounding.
4. QA_QUERY_02 mismatch counts must be 0.
5. Confirm 11 tables and 12 relationships.

## 25–50 min — Dashboard
Build the five pages using 08_FINAL_MEASURE_CATALOG.md and 07_DASHBOARD_BUILD_ORDER.md.

## 50–60 min — Polish
1. Apply the approved NEXORA theme.
2. Align visual spacing.
3. Standardize number formats.
4. Add concise page subtitles and insight callouts.
5. Validate slicers.
6. Capture portfolio screenshots.

## One manual modeling action
If DimDate is not already recognized as the model's date table, use Model view > select DimDate > Mark as date table > choose DimDate[Date]. This is the only manual date-table action required.