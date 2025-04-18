# House Price Prediction - EDA & Data Cleaning

This project focuses on cleaning, preprocessing, and analyzing real estate data to gain insights and prepare it for machine learning modeling. The dataset includes features like location, price, transaction type, area, and ownership status of various properties.

---

## Project Objectives

- Handle missing values and inconsistent formats.
- Clean and transform complex fields like price and area.
- Perform exploratory data analysis (EDA) to uncover trends.
- Prepare the dataset for machine learning models.

---

## Tools & Technologies Used

- **Python**
- **Pandas**, **NumPy** – for data handling and preprocessing
- **Matplotlib**, **Seaborn** – for visualizations
- **Scikit-learn** – for future modeling

---

## Dataset Overview

The dataset includes columns like:

- `Price`
- `Amount (in rupees)`
- `Carpet Area`
- `Bathroom`
- `Furnishing`, `Transaction`, `Facing`, `Ownership`, etc.

---

## Key Preprocessing Steps

### 1. Data Cleaning
- Removed columns with over 50% missing values.
- Handled inconsistent formats in:
  - `Amount(in rupees)` – converted "Lac"/"Cr" to numeric.
  - `Carpet Area` – extracted and unified units (sqft).
- Replaced unknowns with appropriate values or dropped them.
- Cleaned `Bathroom`, `Price`, and `Amount` columns.
- Standardized column names.

### 2. Feature Engineering
- Extracted numerical floors from strings like “2 out of 4”.
- Created a clean dataset (`df3`) ready for visualization and modeling.

---

## Exploratory Data Analysis (EDA)

Visualizations were created to analyze feature distributions:

### Numeric Columns:
- **Box plots** and **histograms** for:
  - `Amount_in_rupees`
  - `Price_in_rupees`
  - `Carpet_Area_in_sqft`
  - `Bathroom`

### Categorical Columns:
- **Bar plots** for:
  - `Transaction`, `Furnishing`, `Facing`, `Ownership`, etc.

---

## Insights Gathered

- Significant outliers were found in `Amount`, `Price`, and `Carpet Area`.
- Majority of transactions were **resale**.
- Most properties were **semi-furnished** and **freehold**.
- Many properties were **north-east facing**.

---

