# Project Development — Tableau

## Data source
Tableau workbook source: `global_fuel_prices_Dataset.csv`. Project-reported figures: 27,468 records, 10 attributes, approximately 2.7 MB, January 2020–April 2026, 84 countries and 7 regions. The exact original download URL is not present in the supplied files and should be added before academic submission.

## Source fields
`date`, `country`, `region`, `income_level`, `subsidy_level`, `petrol_usd_liter`, `diesel_usd_liter`, `lpg_usd_liter`, `brent_crude_usd`, `tax_percentage`.

## Data-preparation and diagnostic checks
- Missing-value check across the ten source fields (owner reported no missing values in the inspected dataset).
- Country-date record count and duplicate-country-date flag.
- Distinct region count per country and region-mapping status.
- Categorical-standardization check.
- Outlier review for Brent crude, diesel, LPG, petrol and tax.
- Temporal organization check.
- Confirm units/source definitions before interpreting `brent_crude_usd`.

## Calculated fields in workbook
1. `Rows With Missing Values` — flags any null across the ten source fields.
2. `Country-Date Record Count` — count by country/date (FIXED LOD).
3. `Duplicate Country-Date Flag` — 1 if the country/date count exceeds one.
4. `Distinct Regions per Country` — distinct region count per country.
5. `Region Mapping Status` — `Review` when more than one region is found, otherwise `Consistent`.
6. `Average Fuel Price (USD/L)` — `(petrol_usd_liter + diesel_usd_liter + lpg_usd_liter) / 3`.
7. `Petrol-Diesel Price Difference (USD/L)` — petrol minus diesel.
8. `Unique Countries` — distinct country count.
9. `Unique Dates` — distinct date count.

## Published outputs
- Dashboard: https://public.tableau.com/app/profile/rudraraj.singh/viz/Global_Fuel_Prices_and_Taxation_Trends/GlobalFuelPricesandTaxationTrendsfinal
- Story: https://public.tableau.com/app/profile/rudraraj.singh/viz/Global_Fuel_Prices_and_Taxation_Trends/Story1
- Dashboard screenshot: `../Evidence_Screenshots/tableau_dashboard_published.png`
- Story structure: see `Tableau/Story_Design.md`.

## Notes
The final dashboard was identified as referencing nine distinct visualization worksheets, while the mentor’s description lists ten items but calls them nine. State the count basis clearly. Snowflake-specific source files in the provided template archive are alternatives and are not claimed as implemented.
