# Builind_Permit_data_cleaning

Use dirty data from kaggle and Clean the data

# Overview

This project cleans a real-world building permit dataset from Kaggle - Building Permit Applications to make it suitable for analysis.
The focus is on handling missing value, fixing data types and removing duplicates.

## Cleaning Steps

- Dropped very sparse columns "Street Number Suffix", "Unit Suffix", "Structural Notification".
- Converted all permit-related date fields (`Permit Creation Date`, `Filed Date`, `Issued Date`, `Completed Date`, etc.) to proper datetime types.
- Imputed key numeric fields ("Existing Units", "Proposed Units", "Existing Construction Type", "Proposed Construction Type", "Number of Existing Stories", "Number of Proposed Stories") using the median.
- Added boolean flags `Is_Completed` and `Has_Expiration_Date` to capture completion and expiration status instead of forcing date imputations.
- Removed Duplicate records based on "Record ID".

## Example Insights

- Using the `Is_Completed` flag, it is easy to compare how many permits are completed vs still open.
- With cleaned `Filed Date`, permits filed per year can be visualized to see how construction activity changes over time.

## Files

- 'date/raw/Building_Permits.csv' - Original data from Kaggle.
- 'date/clean/Building_Permits_Cleaned.csv' - Cleaned Dataset.
- 'notebooks/building_permits_cleaning.ipynb' - cleaning and exploratory analysis.

## Author

**Min Khant Zaw**
Software Engineering Student | TAMK

## Connect with me

- LinkedIn: https://www.linkedin.com/in/minzaw
- GitHub: https://github.com/mkzaw25101999
