# TTTC3213 Assignment 1: Data Profiling (EDA) Report

**Topic:** Hotel Booking Demand: diagnosing and fixing data quality issues

| Name | Matric No. |
|---|---|
| ZHANG LEZHI | A213960 |
| ZHU ZANLIN | A214008 |
| LU JIAYI | A214042 |
| LUO NA | A214087 |

## Scenario
A hotel revenue team wants to use past booking records to study cancellations and set room prices (ADR). The booking data has missing values, outliers, inconsistent categories, quasi-identifiers and unbalanced guest groups. We check whether the data can be trusted for this job.

## Data source
Hotel Booking Demand dataset (Antonio, Almeida & Nunes, 2019, *Data in Brief* 22, 41–49, https://doi.org/10.1016/j.dib.2018.11.126), downloaded as CSV from
https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-02-11/hotels.csv
(also on Kaggle: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand). A copy is in `data/hotels.csv`.

## Files
- `assignment1_data_profiling.ipynb`: the report (scenario, data source, profiling, charts, PII/bias, conclusion)
- `data/hotels.csv`: raw data
- `requirements.txt`: Python libraries

## How to run
```bash
pip install -r requirements.txt
jupyter notebook assignment1_data_profiling.ipynb
```
Then choose **Kernel → Restart & Run All**. The notebook runs from top to bottom. If `data/hotels.csv` is missing, it is downloaded automatically.

Note: Section 5 hashes the agent ID with a secret salt. The salt is read from the `HASH_SALT` environment variable; if it is not set, a random salt is used, so no secret is stored in this repository.
