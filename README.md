# Student Performance Factors Dataset - Data Cleaning with Python

## Project Overview

This project focuses exclusively on cleaning and validating the `StudentPerformanceFactors.csv` dataset using Python.

The dataset contains 6,607 rows and 20 columns relating to student academic performance and associated factors.

## Objectives

- Inspect the raw dataset.
- Identify missing values.
- Check for duplicate records.
- Investigate potential outliers.
- Treat missing categorical values.
- Address an out-of-range exam score under a documented assumption.
- Validate the cleaned data.
- Export a separate cleaned CSV file.

## Tools Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Cleaning Workflow

1. Loaded and inspected the original CSV file.
2. Identified 235 missing cells across three columns.
3. Applied mode imputation to `Teacher_Quality`, `Parental_Education_Level`, and `Distance_from_Home`.
4. Checked for duplicate rows; none were found.
5. Used the IQR method to investigate potential outliers.
6. Treated an exam score of 101 as invalid under an assumed 0–100 range and replaced it using median imputation.
7. Validated the cleaned dataset.
8. Exported the result as `StudentPerformanceFactors_Cleaned.csv`.

## Validation Results

| Check | Result |
|---|---:|
| Rows | 6,607 |
| Columns | 20 |
| Missing values | 0 |
| Duplicate rows | 0 |
| Scores outside assumed range | 0 |

## Output

`StudentPerformanceFactors_Cleaned.csv`

## Key Learning Outcomes

This project strengthened my practical skills in data inspection, missing-value treatment, outlier assessment, data validation, and reproducible file export.

**Important note:** The 0–100 exam-score range was an assumption in the cleaning workflow and should be verified against the dataset's scoring definition.

## Conclusion

The project demonstrates a structured approach to improving data quality and preparing a dataset for subsequent use, while documenting the decisions and assumptions made during cleaning.
