# Builind_Permit_data_cleaning

Use dirty data from kaggle and Clean the data

# Overview

This project cleans a real-world building permit dataset from Kaggle - Building Permit Applications to make it suitable for analysis.
The focus is on handling missing value, fixing data types and removing duplicates.

## Cleaning Steps

- Dropped very sparse columns "Street Number Suffix", "Unit Suffix", "Structural Notification".
- Converted permit-related date fields to proper datetime date types.
- Imputed key numeric fields ("Existing Units", "Proposed Units", "Existing Construction Type", "Proposed Construction Type", "Number of Existing Stories", "Number of Proposed Stories") using the median.
- Created Flags: "Is_Completed" and "Has_Expiration_Date" instead of forcing date imputations.
- Removed Duplicate records based on "Record ID".

## Example Insights

- Distribution of completed vs open permits using the "Is_Completed" flag.
- Number of permits fil per year using the cleaned 'Filed Date'.

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
