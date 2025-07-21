
# Artworks Dataset - Data Cleaning & Exploration

## Project Overview

This project focuses on preparing, cleaning, validating, and exploring an **artworks dataset** extracted from four sources:
- **Museum of Modern Art (New York)**
- **Tate Museums (London)**
- **Rijksmuseum (Amsterdam)**
- **Interpol Stolen Artworks List**

The dataset (210135 rows × 15 columns) required significant cleaning to ensure it was reliable and consistent for analysis. The work was conducted in **Python**, using **pandas**, **numpy**, **matplotlib**, and **missingno** for data cleaning, validation, and visualization.

The objective of this project is to demonstrate my approach to handling data quality challenges, preparing datasets for further exploration, and conducting initial exploratory analysis.

---

## Key Tasks Completed

### Data Cleaning
- Handled inconsistencies in column types (converted to appropriate `int`, `float`, `datetime`, `string` formats) and also Renamed Columns to more appropiate titles.

  <img width="427" height="434" alt="image" src="https://github.com/user-attachments/assets/6d2003fd-3c42-4782-b655-cbde99e72acc" />

- Corrected misplaced data where museum names had shifted into artist columns.
- Removed invalid URLs and correctly reassigned links to the `artwork_link` column.
- Cleaned columns to ensure `Width`, `Height`, and `Depth` contain only numeric values.
- Replaced invalid entries like `'Blank Blank'` or `'Untitled'` with `"Not Available"`.
- Standardized missing data representations (`NaN` vs. "Not Available").
- Parsed date columns into proper `datetime` types.

### Data Validation
Defined clear validation rules to ensure data quality:
- **Numeric columns** (`Width`, `Height`, `Depth`) contain valid positive numbers.
- **Date columns** are parsed as valid dates.
- **URLs** only present in the `artwork_link` column.
- Reassigned incorrect data placement between columns.

### Data Exploration
- Created visualizations to assess data completeness and patterns using `missingno`.

<img width="1488" height="490" alt="image" src="https://github.com/user-attachments/assets/14b3fcf4-1214-4cf1-9dc3-5dfc6acd3ce8" />

- Produced line plots to examine artwork dimensions across the dataset.

  <img width="859" height="547" alt="image" src="https://github.com/user-attachments/assets/cff7745f-c598-43b6-a202-c4e6ce92e9dc" />

- Created Histograms to display the keyword distribution for the Classification Column for example:
  
  <img width="3237" height="1593" alt="image" src="https://github.com/user-attachments/assets/662a45d3-02c0-4d90-8514-b09a728689b8" />

- Prepared for potential deeper exploration (e.g., acquisition trends, century comparisons).
- Created a Wordcloud to better visualize the keywords in the Artwork Column:

 <img width="211" height="210" alt="image" src="https://github.com/user-attachments/assets/a359faf7-0528-4edc-a32a-7b32d1e01765" />

---

## Tools & Libraries
- Python 3.11+
- pandas
- numpy
- matplotlib
- seaborn
- missingno
- re (regex)
---
Through this exercise, I reinforced best practices in cleaning, documenting, and validating datasets before analysis.
For more info, please contact me at www.linkedin.com/in/patience-buxton-msc
Thank you! 
