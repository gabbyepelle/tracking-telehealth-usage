# Medicare Telehealth Utilization Analysis

## Overview
Analysis of Medicare telehealth utilization patterns across the United States using CMS (Centers for Medicare & Medicaid Services) data from 2020-2024. This project explores how telehealth usage varies by geography, demographics, and patient characteristics following the COVID-19 pandemic expansion of telehealth services.

## Key Findings
- Medicare entitlement status is the strongest predictor of telehealth use — ESRD and Disabled beneficiaries use telehealth at significantly higher rates
- Younger beneficiaries use telehealth more, with usage declining consistently across older age groups
- Rural beneficiaries use telehealth 6.3% less than urban counterparts
- Sex has no statistically significant effect on utilization
- Geographic variation is substantial, with some states showing 2x the telehealth usage of others

## Data Source
[CMS Medicare Telehealth Trends](https://data.cms.gov) — publicly available aggregate data covering Medicare fee-for-service beneficiaries from 2020-2024.

## Methods
- Data cleaning and filtering of multi-dimensional demographic dataset
- Interactive choropleth maps by state using Folium and Plotly
- Demographic trend analysis across race, age, sex, rurality, and entitlement status
- OLS regression to identify significant predictors of telehealth utilization

## Libraries Used
- `pandas` — data cleaning and filtering
- `folium` — interactive choropleth maps
- `plotly` — animated and interactive charts
- `scipy` / `statsmodels` — statistical testing and regression
- `requests` — GeoJSON data retrieval

## Caveats
Data is aggregated at the state/national level rather than individual patient records, limiting causal inference. Results cover Medicare beneficiaries only and may not generalize to broader populations.

## How to Run
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Download the data from [CMS](https://data.cms.gov) and place in the root directory
4. Run `jupyter notebook` and open the `.ipynb` file
