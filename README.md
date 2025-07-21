
# 🎨 Artworks Dataset - Data Quality & Exploration

## 📄 Project Overview

This project focuses on preparing, cleaning, validating, and exploring an **artworks dataset** extracted from four sources:
- **Museum of Modern Art (New York)**
- **Tate Museums (London)**
- **Rijksmuseum (Amsterdam)**
- **Interpol Stolen Artworks List**

The dataset required significant cleaning to ensure it was reliable and consistent for analysis. The work was conducted in **Python**, using **pandas**, **numpy**, **matplotlib**, and **missingno** for data cleaning, validation, and visualization.

The objective of this project is to demonstrate my approach to handling data quality challenges, preparing datasets for further exploration, and conducting initial exploratory analysis.

---

## 🛠️ Key Tasks Completed

### 📊 Data Cleaning
- Handled inconsistencies in column types (converted to appropriate `int`, `float`, `datetime`, `string` formats).
- Corrected misplaced data where museum names had shifted into artist columns.
- Removed invalid URLs and correctly reassigned links to the `artwork_link` column.
- Cleaned columns to ensure `Width`, `Height`, and `Depth` contain only numeric values.
- Replaced invalid entries like `'Blank Blank'` or `'Untitled'` with `"Not Available"`.
- Standardized missing data representations (`NaN` vs. "Not Available").
- Parsed date columns into proper `datetime` types.

### 🧐 Data Validation
Defined clear validation rules to ensure data quality:
- **Numeric columns** (`Width`, `Height`, `Depth`) contain valid positive numbers.
- **Date columns** are parsed as valid dates.
- **URLs** only present in the `artwork_link` column.
- Reassigned incorrect data placement between columns.

### 📈 Data Exploration
- Created visualizations to assess data completeness and patterns using `missingno`.
- Produced line plots to examine artwork dimensions across the dataset.
- Prepared for potential deeper exploration (e.g., acquisition trends, century comparisons).

---

## 📐 Example Visualizations
- **Missing Data Matrix** (before & after cleaning)
- **Height vs. Width Line Plot** to observe scale distributions

---

## 🚩 Project Structure
```
├── data/                # (optional) raw datasets
├── notebooks/           # Jupyter notebooks with cleaning & analysis
├── .gitignore
├── README.md            # This file
├── requirements.txt     # Python dependencies
├── cleaned_data.csv     # (optional) clean output
├── your_notebook.ipynb  # Your main notebook
```

---

## 📥 How to Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/artworks-data-quality.git
   cd artworks-data-quality
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook in VS Code or Jupyter Lab:
   ```bash
   jupyter lab
   ```

---

## ✅ Tools & Libraries
- Python 3.11+
- pandas
- numpy
- matplotlib
- missingno
- re (regex)

---

## 💡 Reflections
This project simulates real-life data cleaning challenges:
- Data misalignment between columns
- Incorrect data types
- Missing and inconsistent values
- Preparing datasets for robust analytics

Through this exercise, I reinforced best practices in cleaning, documenting, and validating datasets before analysis.

---

## 📌 Next Steps (If Extended)
- Build a **data quality dashboard** for monitoring key metrics over time.
- Explore deeper analysis on **museum trends** and **acquisition patterns**.
- Compare **19th vs. 20th-century artworks** in detail.
- Explore classification and medium trends per institution.

---

## 🤝 Acknowledgments
Dataset provided as part of a **Data Quality Case Study** exercise.
