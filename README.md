# Global Superstore 2016 — Sales & Profit Analysis

## Project Overview

This project performs exploratory data analysis and business analysis on the Global Superstore 2016 dataset. The analysis focuses on sales, profit, orders, customers, products, markets, categories, customer segments, shipping performance and returned orders.

The project has two deliverables:

1. **Python analysis** — a Jupyter notebook and written report covering the full analysis (sales, profit, markets, segments, shipping, returns).
2. **Excel dashboard** — a one-page sales performance dashboard (`Global_Superstore_Sales_Performance_Dashboard.xlsx`) that presents the headline revenue results visually for a non-technical audience.

## Dataset

The project uses the Global Superstore 2016 Excel dataset.

Dataset link:
https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2Fhshariq%2FGlobal-Superstore-2016-Power-BI%2Fmain%2Fglobal_superstore_2016.xlsx&wdOrigin=BROWSELINK

The supplied workbook contains:

- **Orders** — transaction-level sales data
- **Returns** — returned order information
- **People** — regional manager information

## Dataset Size

- Orders: 51,290 rows and 28 columns
- Returns: 1,079 rows and 3 columns
- People: 24 rows and 2 columns
- Order date range: 2012-01-01 to 2015-12-31

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- OpenPyXL
- Microsoft Excel (dashboard workbook)

## Project Analysis

The notebook covers:

1. Data loading and inspection
2. Missing-value analysis
3. Date conversion and feature engineering
4. KPI calculation
5. Yearly sales and profit trends
6. Category and sub-category analysis
7. Market and country analysis
8. Customer segment analysis
9. Product performance
10. Shipping mode and delivery-time analysis
11. Returned-order analysis
12. Discount vs profit correlation
13. Business insights and conclusion

## Key Results

- Total sales: $12,642,501.91
- Total profit: $1,467,457.29
- Total quantity sold: 178,312
- Unique orders: 25,728
- Unique customers: 17,415
- Unique products: 3,788
- Overall profit margin: 11.61%
- Returned orders: 1,079
- Return rate: 4.19%
- Discount-profit Pearson correlation: -0.3165

## Excel Dashboard

**File:** `Global_Superstore_Sales_Performance_Dashboard.xlsx`

The dashboard is a single-page summary of sales performance built from the Orders data. It has two sheets:

| Sheet | Contents |
|---|---|
| **Dashboard** | KPI cards, three summary tables and three charts |
| **Orders** | The full transaction-level data (51,290 rows, 25 columns, including an added `Year` column) that the dashboard figures are based on |

### KPI cards

| KPI | Value |
|---|---|
| Total Revenue | $12,642,501.91 |
| Top Category | Technology |
| Top Category Revenue | $4,744,557.50 |
| Top Sub-Category | Phones |

### Charts

| Chart | Type | What it shows |
|---|---|---|
| Revenue by Category | Bar | Sales split across Technology, Furniture and Office Supplies |
| Yearly Sales Trend | Line | Total sales for each year from 2012 to 2015 |
| Revenue by Sub-Category | Bar | Sales for all 17 sub-categories, ranked highest to lowest (titled "Department-Wise Revenue" on the sheet) |

### Dashboard findings

**Sales by category**

| Category | Sales | Share of total |
|---|---|---|
| Technology | $4,744,557.50 | 37.5% |
| Furniture | $4,110,451.90 | 32.5% |
| Office Supplies | $3,787,492.51 | 30.0% |

**Yearly sales trend**

| Year | Sales | Change vs previous year |
|---|---|---|
| 2012 | $2,259,450.90 | — |
| 2013 | $2,677,438.69 | +18.5% |
| 2014 | $3,405,746.45 | +27.2% |
| 2015 | $4,299,865.87 | +26.3% |

- Sales grew every year, and 2015 sales were about 90% higher than 2012.
- Technology is the largest category, but the three categories are fairly close (about 8 percentage points separate first from last).
- Phones is the top sub-category at $1,706,824 (13.5% of total sales).
- The top four sub-categories (Phones, Copiers, Chairs, Bookcases) together bring in about $6.18M, roughly 49% of total sales, and they come from just two categories: Technology and Furniture.
- The smallest sub-categories are Labels ($73,350), Fasteners ($89,495) and Envelopes ($169,217).

### How to use the dashboard

1. Download `Global_Superstore_Sales_Performance_Dashboard.xlsx` and open it in Microsoft Excel (or a compatible spreadsheet application).
2. The **Dashboard** sheet opens with the KPI cards at the top and charts below.
3. Use the **Orders** sheet to check any figure against the source rows.

### Dashboard limitations

- The dashboard reports **revenue (sales) only**. Profit, margin, market, segment, shipping and return analysis are covered in the Python notebook and report, not the dashboard.
- The KPI cards and summary tables contain **static values**, not formulas or pivot tables, and there are no slicers or filters. If the Orders data changes, these values need to be updated manually.
- The Orders sheet in the workbook contains 25 columns (the `Year` column was added), while the original dataset has 28. The Returns and People sheets are not included.
- All dashboard figures were cross-checked against the Orders sheet and match the totals reported in the Key Results above.

## Setup and Run Instructions

### Python notebook

#### 1. Install Python

Use Python 3.9 or newer.

#### 2. Install dependencies

```bash
pip install -r requirements.txt
```

#### 3. Place the dataset

Place `global_superstore_2016.xlsx` in the same folder as the notebook.

#### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

#### 5. Open and run

Open `SachinSisodiya_GlobalSuperstore.ipynb` and run the cells from top to bottom.

### Excel dashboard

No setup is needed. Open `Global_Superstore_Sales_Performance_Dashboard.xlsx` directly in Excel.

## Project Files

- `SachinSisodiya_GlobalSuperstore.ipynb` — complete project code
- `requirements.txt` — Python dependencies
- `SachinSisodiya_GlobalSuperstore_ProjectReport.docx` — project report
- `Global_Superstore_Sales_Performance_Dashboard.xlsx` — Excel sales performance dashboard
- `README.md` — project overview and setup instructions
