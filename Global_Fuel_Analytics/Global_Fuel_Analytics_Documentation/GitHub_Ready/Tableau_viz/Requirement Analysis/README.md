# Requirement Analysis

## Intended user journey
1. **Discover:** open the project website and read About the Data.
2. **Explore:** open the Tableau dashboard and change filters to compare measures, dates and categories.
3. **Understand/share:** navigate the seven-scene Story, review conclusions and share the public links.

## Functional requirements
| ID | Requirement | Acceptance criterion | Priority |
|---|---|---|---|
| FR-1 | Connect the CSV source to Tableau | Ten expected fields are available in the workbook | High |
| FR-2 | Review data quality | Missing values, country-date duplicates, region mapping, standardization, outliers and temporal ordering are checked | High |
| FR-3 | Calculate analytical measures | Price average/difference and unique country/date counts are available | High |
| FR-4 | Create visual outputs | Maps, trends, tax and country comparisons, KPI cards and Story are available | High |
| FR-5 | Allow filtering | Date, Region, Income Level and Subsidy Level update relevant charts | High |
| FR-6 | Publish and share | Dashboard and Story open on Tableau Public and are linked from the website | High |

## Non-functional requirements
- **Usability:** clear titles, labels, units and navigation.
- **Security:** Tableau Public content is public; confidential data must not be published.
- **Reliability:** charts and filters should render/update without blank or error states.
- **Performance:** measured in one browser session: 5 s initial load, ~4 s single-filter response, ~5 s two-filter response.
- **Availability:** network access is required for hosted Tableau views.
- **Scalability:** current solution is student-scale; future growth may require a governed data source and optimized hosting.

## Data-flow diagram in text
`Source CSV → data-quality checks / standardization → Tableau Desktop calculations and visualizations → Tableau Public dashboard + Story → Flask/HTML presentation page or direct public link → viewer.`

## User stories
- As a viewer, I can open the dashboard and see fuel-price/taxation indicators.
- As a viewer, I can change Date and Region filters and see relevant charts update.
- As a viewer, I can change Income Level and Subsidy Level to compare categories.
- As a viewer, I can navigate all seven Story scenes.
- As a reviewer, I can open both published views through direct links.
- As the project owner, I can maintain the page, links and evidence files.

## Technology stack
- Source data: `global_fuel_prices_Dataset.csv` (CSV; original download URL not provided in current materials).
- Analysis and visualizations: Tableau Desktop.
- Hosting: Tableau Public.
- Website presentation: Flask / HTML / CSS / JavaScript, as present in the local project.
- Repository: https://github.com/rudrarajsingh887/Tableau_viz.
- **Not part of current implementation:** Snowflake, MySQL, a separate SQL warehouse or a production ETL pipeline.
