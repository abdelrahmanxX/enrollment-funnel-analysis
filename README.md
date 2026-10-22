# Enrollment Funnel Analysis

Portfolio project: tracking a university enrollment funnel (lead → contacted → applied → admitted → enrolled).

**All data is synthetic.** It was generated for this project and contains no real students or institutions. The patterns in it come from my generator's assumptions, so the findings describe this dataset only.

## Contents
- `Enrollment_Funnel_Dashboard.xlsx`: formula-driven Excel dashboard (conversion by source, program and counselor, weekly/monthly reports, 4-week trend forecast, data-quality checks)
- `enrollment_funnel_leads.csv`: raw data (1,605 rows, including 12 deliberately bad records)
- Notebook (`.ipynb`): the same analysis in Python (Pandas, Matplotlib)

## Method
- Removed duplicate IDs, rows with no source and rows with out-of-order dates (12 of 1,605 rows), leaving 1,593 valid leads
- Funnel and conversion rates by source, program and counselor
- Speed-to-contact comparison and a simple linear trend forecast

## Results (on this synthetic data)
- 7.3% of leads enrolled. Walk-in and referral leads converted at about twice that rate.
- Leads contacted within 2 days applied more often than slower-contacted ones (20.6% vs 15.3%).
