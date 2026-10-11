# Data files

The raw and processed CSV files are intentionally not committed to this repository because the full-year dataset is large.

## Raw data

Download the four 2019 quarterly Divvy trip CSV files from the [Divvy historical data page](https://divvybikes.com/system-data) or the [Divvy trip-data archive](https://divvy-tripdata.s3.amazonaws.com/index.html). Review the [Divvy Data License Agreement](https://divvybikes.com/data-license-agreement).

Place the extracted CSVs in a local `data/raw/` folder:

- `Divvy_Trips_2019_Q1.csv`
- `Divvy_Trips_2019_Q2.csv`
- `Divvy_Trips_2019_Q3.csv`
- `Divvy_Trips_2019_Q4.csv`

## Processed data

Run `notebooks/bike_share_cleaning.ipynb` to create `data/processed/bike_share_cleaned.csv`, then run `notebooks/bike_share_analysis.ipynb` using that file.

The `raw/` and `processed/*.csv` paths are excluded by `.gitignore`; keep the files locally rather than committing the large CSVs.
