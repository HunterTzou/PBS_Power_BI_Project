# PBS_Power_BI_Project
Hosting the files for the PBS Power BI project

## Caveats & Disclaimers

### Data
- All data used in this report was provided by PBS Distribution for the purposes of this project. The dataset covers January 2023 through December 2025 and represents entirely actuals per stakeholder confirmation.
- `total_streams` values have been rounded to the nearest whole number. Per the stakeholder, decimal values are the result of internal data transformations and do not reflect partial stream counts.
- `Total Subs` is an end-of-period metric. The `Date` column represents the first day of the reporting month as a labeling convention, not a literal snapshot date.
- A known discrepancy exists in the PBS Documentaries 2025 budget — the Net Adds budget (60,000) combined with the December 2024 baseline (~680,000) implies an ending subscriber count of approximately 740,000, falling short of the stated EOY target of 800,000. This has been flagged per stakeholder guidance and is noted in the report.
- Churn rate spikes reaching approximately 23% in certain months reflect known business events per stakeholder confirmation and are not data errors.

### Methodology
- Subscriber counts shown in the report represent end-of-period values, not cumulative totals or averages.
- Budgeted growth percentages are calculated using December 2024 ending subscriber counts as the baseline against the 2025 EOY budget target.
- Stream peaks and subscriber growth are shown together for exploratory purposes only. Correlation between content performance and subscriber acquisition does not imply direct causation.
- The PBS Documentaries 2025 growth target of approximately 18% is intentionally aggressive relative to other channels and reflects a stronger content investment slate per stakeholder guidance.

### Design
- PBS Sans, the official PBS brand typeface, is not natively available in Power BI. Segoe UI has been used as a substitute throughout the report.
- The PBS Distribution logo and brand assets are the property of PBS and are used here solely for the purposes of this portfolio project.
- This report was built as a technical assessment project and is not intended for commercial use or public distribution.

### Technical
- Data is sourced from CSV files hosted on GitHub. In a production environment these would connect to a live data source such as SharePoint or a SQL database.
- All DAX measures are designed to be year-agnostic and will update automatically when new data is added without requiring manual edits to the report.
- The report was built and tested on Power BI Desktop version March 2025. Some visual formatting may render differently on older versions.
