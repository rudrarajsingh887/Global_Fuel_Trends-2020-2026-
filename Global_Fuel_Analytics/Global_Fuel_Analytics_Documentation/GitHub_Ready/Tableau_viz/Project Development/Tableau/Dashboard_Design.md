# Tableau Dashboard Design

## Layout and visuals
- KPI strip summarizes average diesel, LPG and petrol prices plus average tax percentage.
- Geographic maps compare country-level petrol and diesel values.
- Line charts cover petrol, diesel, LPG and Brent crude indicators.
- Tax visualization compares regional tax-percentage averages.
- Bar charts support ranked country comparisons.
- Diagnostic worksheets remain available in the workbook but do not need to occupy the main dashboard.

## Visual design
The dashboard uses a light-blue panel theme, clear chart titles and compact labels. The KPI strip is positioned first, followed by maps, time-series charts and regional/country comparisons.

## Interactive behaviour tested by owner
- Date: updated correctly.
- Region: updated correctly.
- Income Level: updated correctly.
- Subsidy Level: updated correctly.
- Country and Measure/Fuel Type: not visible during a separate filter test; verify the exact final published view before claiming these are dashboard filters.

## Performance observations
Initial load: 5 seconds; single-filter response: approximately 4 seconds; two-filter response: approximately 5 seconds. The owner observed all visible charts updating and no blank charts/errors in that session.

## Sample displayed default indicators
The supplied screenshot shows diesel average 2.135 USD/L, LPG average 1.715 USD/L, petrol average 2.285 USD/L, and average tax percentage 26.77%. These are snapshot values for that displayed state.

## Publish URL
https://public.tableau.com/app/profile/rudraraj.singh/viz/Global_Fuel_Prices_and_Taxation_Trends/GlobalFuelPricesandTaxationTrendsfinal
