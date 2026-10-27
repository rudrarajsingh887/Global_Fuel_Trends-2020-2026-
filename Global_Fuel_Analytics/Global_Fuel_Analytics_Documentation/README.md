# Global Fuel Analytics — Documentation Pack

**Project:** Global Fuel Prices and Taxation Trends: A Comprehensive Global Performance Intelligence Report
**Owner:** Rudraraj Singh Bhati
**Prepared:** 25 October 2026

## What's included
- `07_Project_Documentation/Final_Project_Report.docx` — report structured to the supplied Final Report Template headings.
- Tableau-specific completed templates for ideation, requirements, design, planning, business questions, dashboard/story design, and performance testing.
- Standalone completed requirements-analysis and demonstration sheets corresponding to supplied PDF templates.
- `08_Project_Demonstration/End_to_End_Recording_Script.docx` — narration plan for a 5–7 minute screen-share video.
- `Evidence_Screenshots/` — screenshots and map asset included as supporting evidence.
- Snowflake-specific forms are marked N/A because the confirmed implementation uses a CSV source and Tableau, not Snowflake.

## Confirmed project facts used
- Workbook source filename: `global_fuel_prices_Dataset.csv` (workbook connection points to a local Windows path).
- Project-reported scope: 27,468 records, 10 attributes, approx. 2.7 MB, January 2020–April 2026, 84 countries, 7 regions.
- Workbook contains 9 unique calculated fields and multiple diagnostic worksheets.
- Dashboard: https://public.tableau.com/app/profile/rudraraj.singh/viz/Global_Fuel_Prices_and_Taxation_Trends/GlobalFuelPricesandTaxationTrendsfinal
- Story: https://public.tableau.com/app/profile/rudraraj.singh/viz/Global_Fuel_Prices_and_Taxation_Trends/Story1
- GitHub repository: https://github.com/rudrarajsingh887/Tableau_viz
- User-observed performance: initial load 5 seconds; single-filter update approx. 4 seconds; two-filter update approx. 5 seconds; all visible charts updated correctly and no rendering errors were observed in that session.

## Important unresolved items before final submission
1. Add the original dataset source URL and licensing/attribution information; it was not supplied in the materials available for this pack.
2. Verify the dashboard time axis: supplied screenshot labels trend views through 2027, while the reported dataset coverage ends in April 2026.
3. Reconcile filter controls: the live filter test reported Date, Region, Income Level and Subsidy Level work; Country and Measure/Fuel Type were not visible in that test, although a separate screenshot shows similarly named controls.
4. Team ID was not supplied; completed sheets use “Individual project; official Team ID not provided”. Replace with the official ID if required.
5. Historical sprint dates and actual velocity were not supplied; the plan marks them as not recorded and treats story points as retrospective estimates.
6. Check screenshots and current website before claiming a feature is demonstrated.

## Uploading to GitHub
The public repository currently contains the phase directories but inspected entries such as `IdeationPhase` and `Performance Testing` are placeholder files with 0 lines and around 1–2 bytes. This archive has **not** been pushed to GitHub. After review, upload the populated files to the matching phase folders and remove the zero-byte placeholder files. Do not upload private credentials, secrets, or a confidential dataset.
