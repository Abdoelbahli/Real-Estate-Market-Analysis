# Real Estate Market Analysis

## Project Overview
This project focuses on analyzing the real estate market around specific ZIP codes to provide insights into home prices, rental values, and potential profits. The main objective was to estimate profits from converting 3-bedroom, 1-bathroom homes into smaller rental units (2-bedroom, 1-bathroom and 1-bedroom, 1-bathroom).

## Key Objectives
1. **Home Price Analysis:** Calculate the average home price for 3-bedroom, 1-bathroom homes.
2. **Rental Market Analysis:** Calculate the average rent for 2-bedroom, 1-bathroom and 1-bedroom, 1-bathroom units.
3. **Profit Estimation:** Estimate potential profits using:
   - Formula: `Estimated Profit = ((AvgRent (2br/1ba) \u00d7 2) + AvgRent (1br/1ba)) - Estimated Mortgage`
   - Fixed mortgage terms: 20% down payment, 7.5% interest rate, 30-year loan.
4. **Predict Missing Values:** Use Machine Learning to predict missing rent prices for ZIP codes without rental data.
5. **Provide Comprehensive Results:** Combine all insights into a single dataset for easy interpretation.

## Data Sources
The data used in this analysis includes:
- **Home Price Data:** Extracted from CSV files named by ZIP code (e.g., `95301.csv`).
- **Rental Data:** Extracted from 2-bedroom and 1-bedroom unit files named in formats like `2bed_1bath_{zipcode}.csv` and `1bed_1bath_{zipcode}.csv`.

## Steps Taken
1. **Data Cleaning:**
   - Removed unnecessary columns.
   - Removed outliers (bottom 10% and top 10% of values) to ensure accuracy.
   - Addressed missing values using Machine Learning for profit estimation.

2. **Data Transformation:**
   - Combined all data into a single DataFrame with the following columns:
     - `ZipCode`
     - `AvgHomePrice (3br/1ba)`
     - `AvgRent (2br/1ba)`
     - `AvgRent (1br/1ba)`
     - `Estimated Profit`
     - `Profit Predicted` (Indicates whether the profit was predicted or calculated).

3. **Machine Learning:**
   - Used a Linear Regression model to predict missing profit values based on trends in available data.

4. **Results Compilation:**
   - Exported the final dataset as an Excel file for easy sharing and visualization.

## Results
The final analysis includes insights for each ZIP code, with calculated or predicted values where necessary. ZIP codes without rental data were handled using Machine Learning to provide estimated profits.

## Deliverables
1. **Excel File:** Contains the final combined dataset with all relevant columns.
2. **Raw Data and Code:** Available upon request, including the raw CSV files and Jupyter Notebook used for analysis.

## How to Use
1. Open the provided Excel file to view the results.
2. Use the `Profit Predicted` column to identify ZIP codes with predicted values.
3. Contact me for access to raw data and code if needed.

## Contact
If you have any questions or need further clarification, feel free to reach out!

- **Prepared by:** Abdellah
- **Date:** December 21st 2024

