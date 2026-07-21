# Exploratory Data Analysis — Online Retail

Exploratory data analysis of a real UK-based online retailer's transaction data, covering revenue patterns, geographic distribution, seasonality, top products, and returns. Built as part of my data analytics portfolio.

## Data Source

- **Dataset:** Online Retail — UCI Machine Learning Repository
- **Citation:** Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33
- **License:** CC BY 4.0
- **Coverage:** All transactions from a UK-based, registered non-store online retailer between 01/12/2010 and 09/12/2011
- **Size:** 541,909 transactions, 8 columns

## Tools

- Python (Pandas, Matplotlib)
- Google Colab / Jupyter Notebook

## Structure

notebooks/
  eda_online_retail.ipynb
data/
  Online Retail.xlsx

## Analysis Steps

1. Initial inspection — structure, data types, missing values
2. Data quality check — identified negative values in Quantity and UnitPrice, split transactions into Sale, Return, and Adjustment instead of discarding them
3. Revenue analysis — total revenue, by country, by month, by product
4. Returns analysis — top returned products, volume check

## Key Findings

- Total revenue (sales only): £10,666,684.54
- The UK accounts for the large majority of revenue; excluding it, the Netherlands, EIRE, and Germany lead international markets
- Revenue peaks sharply in November, consistent with holiday-season stocking
- "PAPER CRAFT, LITTLE BIRDIE" appears both as a top-revenue product and as the single largest return (-80,995 units) — same magnitude as the negative-quantity outlier flagged during data quality review, suggesting one abnormal transaction rather than a genuine return pattern

## Skills Demonstrated

- Data cleaning and quality assessment without discarding informative outliers
- Aggregation and grouping (groupby, resample)
- Time series analysis (monthly revenue trend)
- Data visualization (bar, horizontal bar, line charts)
- Critical interpretation of results (cross-checking outliers across analyses)

## Status

Complete
