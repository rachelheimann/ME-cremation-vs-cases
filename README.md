# Cook County Cremation and Case Data Analysis

This notebook merges and analyzes Cook County cremation records with medical examiner case data to identify individuals who died while in custody at Cook County Jail. The analysis uses names from cremation records to match case numbers in the ME dataset, revealing decedents whose identities may be obscured in other public records.

## Data Sources

- **Cremation Records**: [Cook County Data Portal](https://datacatalog.cookcountyil.gov/)
- **Medical Examiner Case Data**: [Cook County Data Portal](https://datacatalog.cookcountyil.gov/)

## Methodology

- Standardized `case_number` fields across datasets
- Merged cremation and case data on `case_number`
- Filtered merged dataset using a predefined list of in-custody case numbers
- Selected key columns for review, including:
  - Name
  - Date of Death
  - Age
  - Sex
  - Race
  - Manner and Cause of Death
  - Incident Address

## Purpose

This analysis aims to identify individuals who died while in custody at Cook County Jail by cross-referencing names from cremation records with case numbers in the Medical Examiner’s data. By merging these datasets and filtering for known in-custody deaths, the project reveals the names and details of decedents whose cases may otherwise be obscured or anonymized in public records.

## How to Use

1. Open the notebook in Google Colab or Jupyter
2. Run all cells to reproduce the analysis
3. Modify the `case_list` to explore additional cases

## Author

Rachel Heimann Mercader  
Medill School of Journalism, Northwestern University  
Investigative Reporting & Data Journalism
