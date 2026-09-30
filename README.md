# COVID-19 Global Impact Dashboard

Veda Technology — Major Project

## Project objective
Analyze publicly available COVID-19 data across countries and time, normalize country comparisons by population, derive 7-day rolling averages, case fatality rate and doubling time, and communicate the findings through charts and an interactive dashboard.

## Focus
The analysis uses a focused question:

> How did COVID-19 waves and vaccination rollout differ across countries, and what patterns can be observed when cases and deaths are normalized by population?

The vaccination/death relationship is treated as exploratory association rather than causal inference.

## Deliverables
- `notebook/COVID19_Global_Impact_Dashboard.ipynb` — complete reproducible analysis
- `data/owid_snapshot_preview.csv` — sourced snapshot used for the static preview
- `outputs/` — clean portfolio-ready preview charts
- `dashboard/covid_dashboard.html` — interactive browser dashboard that loads OWID data
- `report/COVID19_Executive_Summary.pdf` — one-page submission summary
- `report/COVID19_Detailed_Report.pdf` — detailed portfolio report
- `requirements.txt` — Python dependencies

## Data source
Our World in Data COVID-19 compact dataset:
https://catalog.ourworldindata.org/garden/covid/latest/compact/compact.csv

Documentation:
https://docs.owid.io/projects/etl/api/covid/

OWID's COVID-19 technical documentation explains that the compact dataset consolidates relevant COVID-19 indicators and provides separate cases/deaths and vaccination datasets.

## Important snapshot note
The included preview dataset combines:
- vaccination coverage snapshot dated August 12, 2024; and
- a separate current OWID confirmed-death-per-million context from July 19, 2026.

These are clearly separated in the file and report. The full time-series analysis should be run from the notebook, which downloads the current OWID compact dataset.

## How to run
1. Install Python 3.10+.
2. Install dependencies:
   `pip install -r requirements.txt`
3. Open the notebook.
4. Run all cells.
5. The notebook downloads the OWID dataset, cleans it, derives metrics, creates charts and exports a cleaned focus-country CSV.

Internet access is required for the live OWID download.

## Key methodology
- Date standardization
- Duplicate country-date removal
- Conservative missing-value handling
- 7-day rolling averages
- Cases/deaths per million
- Crude reported case fatality rate
- Seven-day growth-based doubling time
- Simple wave peak detection
- Country comparison with transparent limitations

## Suggested GitHub repository name
`Task-32-COVID19-Global-Impact-Dashboard`

## License / attribution
Data are sourced from Our World in Data and its underlying providers. Follow the source licenses and attribution requirements described by OWID.
