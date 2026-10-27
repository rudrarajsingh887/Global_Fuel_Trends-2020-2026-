# Scalability and Future Plan

## Current limitations
- CSV source is a local-file connection; data refresh and republishing are manual unless otherwise configured.
- Tableau Public content is publicly accessible and should contain no confidential data.
- Performance timing is from one browser session.
- Dataset provenance/source URL needs to be added.
- The displayed trend axis should be checked because a supplied screenshot labels values through 2027 while reported coverage ends April 2026.

## Potential upgrades
| Area | Future improvement | Benefit |
|---|---|---|
| Data governance | Document source URL, license, date and data dictionary | Reproducibility and provenance |
| Refresh | Define a repeatable refresh and republish procedure | Clearer data freshness |
| Performance | Repeat measurements on multiple browser/network conditions | More robust test evidence |
| Analytics | Add appropriate context variables and statistical methods if required | More careful interpretation |
| UX | Validate labels, filters and mobile layout with viewers | Better accessibility and usability |
