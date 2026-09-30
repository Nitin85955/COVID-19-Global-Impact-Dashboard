# GitHub Upload Guide — Task 32

## Suggested repository name
`Task-32-COVID19-Global-Impact-Dashboard`

## 1. Create repository
1. Open GitHub.
2. Click **New repository**.
3. Enter the repository name above.
4. Select **Public**.
5. Create the repository.

## 2. Upload the project
Upload the **contents** of the ZIP, not the ZIP file itself, if the portal expects a normal project repository.

Recommended structure:

```text
Task-32-COVID19-Global-Impact-Dashboard/
├── README.md
├── requirements.txt
├── notebook/
│   └── COVID19_Global_Impact_Dashboard.ipynb
├── data/
│   └── owid_snapshot_preview.csv
├── outputs/
│   ├── 01_vaccination_at_least_one_dose.png
│   ├── 02_full_vaccination_protocol.png
│   ├── 03_confirmed_deaths_per_million_context.png
│   ├── 04_analytics_pipeline.png
│   └── 05_dashboard_preview.png
├── dashboard/
│   └── covid_dashboard.html
└── report/
    ├── COVID19_Executive_Summary.pdf
    └── COVID19_Detailed_Report.pdf
```

## 3. Commit
Use a natural commit message such as:

`Complete COVID-19 Global Impact Dashboard project`

## 4. Final repository check
Open the repository in an incognito/private browser window and verify that:
- README opens correctly
- notebook is visible
- PDFs open
- output images are visible
- dashboard HTML is present
- no private/personal files were uploaded

## 5. Submission
Copy the public GitHub repository URL and submit that URL through the Veda internship portal.
