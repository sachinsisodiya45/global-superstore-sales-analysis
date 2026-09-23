# Global Superstore 2016 --- Sales & Profit Analysis

## Project Overview

This project performs exploratory data analysis and business analysis on
the Global Superstore 2016 dataset. The analysis focuses on sales,
profit, orders, customers, products, markets, categories, customer
segments, shipping performance and returned orders.

## Dataset

The project uses the Global Superstore 2016 Excel dataset.

Dataset link:
https://raw.githubusercontent.com/hshariq/Global-Superstore-2016-Power-BI/main/global_superstore_2016.xlsx

The supplied workbook contains: - **Orders** --- transaction-level sales
data - **Returns** --- returned order information - **People** ---
regional manager information

## Dataset Size

-   Orders: 51,290 rows and 28 columns
-   Returns: 1,079 rows and 3 columns
-   People: 24 rows and 2 columns
-   Order date range: 2012-01-01 to 2015-12-31

## Technologies Used

-   Python
-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   Jupyter Notebook
-   OpenPyXL

## Project Analysis

The notebook covers: 1. Data loading and inspection 2. Missing-value
analysis 3. Date conversion and feature engineering 4. KPI calculation
5. Yearly sales and profit trends 6. Category and sub-category analysis
7. Market and country analysis 8. Customer segment analysis 9. Product
performance 10. Shipping mode and delivery-time analysis 11.
Returned-order analysis 12. Discount vs profit correlation 13. Business
insights and conclusion

## Key Results

-   Total sales: \$12,642,501.91
-   Total profit: \$1,467,457.29
-   Total quantity sold: 178,312
-   Unique orders: 25,728
-   Unique customers: 17,415
-   Unique products: 3,788
-   Overall profit margin: 11.61%
-   Returned orders: 1,079
-   Return rate: 4.19%
-   Discount-profit Pearson correlation: -0.3165

## Setup and Run Instructions

### 1. Install Python

Use Python 3.9 or newer.

### 2. Install dependencies

``` bash
pip install -r requirements.txt
```

### 3. Place the dataset

Place `global_superstore_2016.xlsx` in the same folder as the notebook.

### 4. Start Jupyter Notebook

``` bash
jupyter notebook
```

### 5. Open and run

Open `SachinSisodiya_GlobalSuperstore.ipynb` and run the cells from top
to bottom.

## Project Files

-   `SachinSisodiya_GlobalSuperstore.ipynb` --- complete project code
-   `requirements.txt` --- Python dependencies
-   `SachinSisodiya_GlobalSuperstore_ProjectReport.docx` --- project
    report
-   `README.md` --- project overview and setup instructions
-   `charts/` --- report visualization images

## Important Note

The notebook expects the dataset filename to be
`global_superstore_2016.xlsx`. If your downloaded file has another name,
rename it before running the notebook or update the `file_path` variable
in the first data-loading cell.
