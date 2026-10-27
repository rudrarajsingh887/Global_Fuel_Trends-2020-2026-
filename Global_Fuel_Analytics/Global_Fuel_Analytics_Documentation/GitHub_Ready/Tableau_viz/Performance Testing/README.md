# Performance Testing — Tableau

## 1. Amount of data rendered
- Dataset: project-reported 27,468 records, 10 attributes, approximately 2.7 MB.
- Coverage: Jan 2020–Apr 2026, 84 countries, 7 regions (reported).
- Initial load: **5 seconds**.
- Visualizations: **all visible after loading**.
- Single-filter response: **approximately 4 seconds**.
- Two-filter response: **approximately 5 seconds**.
- Two-filter update: **yes, charts updated correctly**.
- Blank charts / errors / endless spinners: **none observed** in the tested session.

## 2. Utilization of filters
| Filter | Result |
|---|---|
| Date | Updated correctly |
| Region | Updated correctly |
| Income Level | Updated correctly |
| Subsidy Level | Updated correctly |
| Country | Not visible during the recorded individual filter test |
| Measure/Fuel Type | Not visible during the recorded individual filter test |

## 3. Calculated fields
Nine unique calculated fields are defined in the workbook: Rows With Missing Values; Country-Date Record Count; Duplicate Country-Date Flag; Distinct Regions per Country; Region Mapping Status; Average Fuel Price (USD/L); Petrol-Diesel Price Difference (USD/L); Unique Countries; Unique Dates.

## 4. Visualization count
Nine visualization worksheets were identified as referenced by the final dashboard. The mentor’s description says “9 distinct visualization types” but enumerates 10 bullet items. The count above refers to worksheets referenced by the final dashboard, not unique chart families.

## 5. Story design
Seven scenes. The owner confirmed all scenes were navigable.

## Testing caveat
Times are from one browser session, not a repeatable benchmark; actual performance varies by network, browser and device. Dataset row count and file size are project-reported. The workbook XML proves field names and calculations but does not prove the loaded row count. See the performance-test doc included in this pack for more detail.
