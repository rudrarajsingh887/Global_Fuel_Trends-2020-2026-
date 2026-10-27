# Tableau Performance-Test Record

| Test | Observed value | Result |
|---|---|---|
| Initial load | 5 s | Recorded |
| Rendering | All visible | Pass |
| Single-filter response | ~4 s | Recorded |
| Two-filter response | ~5 s | Recorded |
| Two-filter update | Charts updated correctly | Pass |
| Blank charts/errors/spinners | None observed | Pass |
| Date filter | Updated correctly | Pass |
| Region filter | Updated correctly | Pass |
| Income Level filter | Updated correctly | Pass |
| Subsidy Level filter | Updated correctly | Pass |
| Country filter | Not visible in that browser test | Not tested |
| Measure/Fuel Type filter | Not visible in that browser test | Not tested |

Nine calculated fields were found in the workbook. The final dashboard references nine distinct visualization worksheets; the mentor’s supplied list contains a 9-vs-10 wording inconsistency. Reported dataset figures: 27,468 records, 10 attributes, approx. 2.7 MB, January 2020–April 2026, 84 countries, 7 regions.
