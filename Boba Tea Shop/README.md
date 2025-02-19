# Boba CSV Data Cleanup

## Overview
This repository contains a cleaned-up version of a boba shop dataset stored in a Google Sheet CSV file. The dataset originally included duplicate entries, inconsistent rating values, and combined latitude-longitude coordinates.

## Columns in the Dataset
- `id`: Unique identifier for each boba shop
- `name`: Name of the boba shop
- `rating`: Customer rating (originally contained values above 5)
- `address`: Street address of the boba shop
- `city`: City where the shop is located
- `lat-long`: Combined latitude and longitude coordinates

## Data Cleanup Process
### 1. Removing Duplicates
Used Google Sheets' **Data Cleanup** feature to remove duplicate rows based on the `id`, `name`, and `address` columns.

### 2. Standardizing Ratings
- Used `COUNTIF` to find all ratings above `5`:
  ```excel
  =COUNTIF(C2:C, ">5")
  ```
- Sorted the dataset by `rating` to easily identify values above `5`.
- Manually replaced any rating above `5` with `5`.

### 3. Splitting Latitude and Longitude
- Used the **SPLIT** function in Google Sheets to separate `lat-long` into two columns:
  ```excel
  =SPLIT(F2, ",")
  ```
- Renamed the new columns as `latitude` and `longitude`.

## Final Dataset
After cleaning, the dataset now contains:
- Unique entries with no duplicates.
- Ratings capped at `5`.
- Separate `latitude` and `longitude` columns for better geospatial analysis.

## Usage
This cleaned dataset can be used for further data analysis, visualization, or integration into applications such as mapping tools.
