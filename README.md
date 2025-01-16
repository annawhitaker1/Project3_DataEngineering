# Project3_DataEngineering

## Overview 

This project analyzes global holidays and travel data to explore the relationship between holidays and travel trends. Using two datasets sourced from Kaggle, we built an ETL pipeline to process and load the data into a SQL database for efficient analysis. The project provides insights into how holidays influence global travel behavior, with applications in tourism and travel planning.

## How to interact with this dataset

This project includes these key datasets:

  1. global_holidays.csv: The raw dataset containing global holiday information.
  2. monthly_passengers.csv: The raw dataset containing monthly passenger counts.

The following cleaned datasets were generated:

1. modified_holidays_travel.csv: A cleaned and processed dataset combining global holidays and travel data.
2. modified_monthly_passengers.csv: A cleaned version of the monthly passenger data.
3. modified_merged.csv: A merged dataset prepared for analysis.

## SQL Documentation 

The cleaned data is stored in a SQL database. SQL was chosen for its robust querying capabilities and for its ability to handle structured dat. 

The database consists of the following tables:

1. holidays_travel:
  - country_code: Foreign key linking to the country_code table.
  - date, month_year, name, type: Represent holiday details.
2. monthly_passengers:
  - country_code: Foreign key linking to the country_code table.
  - Passenger details: total_passengers_official, domestic, international, total_passengers_open.
3. country_code:
  - country: The name of the country.
  - country_code: Primary key representing the country.

## ETL Workflow

## Ethical Considerations

## Data Sources 

https://www.kaggle.com/datasets/umerhaddii/global-holidays-and-travel-data?select=global_holidays.csv
