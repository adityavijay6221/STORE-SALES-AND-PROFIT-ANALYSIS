# Superstore Sales Forecasting & Analysis

## Overview
This project involves exploratory data analysis, forecasting, and optimization using the **Sample - Superstore** dataset.  
The experiments and results are documented in the `experiments.ipynb` file.

## Dataset
- **Source**: Sample - Superstore dataset  
- **Features**: Order Date, Ship Date, Segment, Category, Sub-Category, Sales, Quantity, Discount, Profit, etc.  
- **Objective**: Forecast sales/demand and analyze category-level performance trends.

## Data Preprocessing
- Converted `Order Date` to datetime format and set as index for time series analysis.  
- Handled missing and duplicate entries.  
- Created aggregated time-series data for forecasting (e.g., monthly/weekly sales).  
- Differencing applied to remove trend and achieve stationarity before ARIMA modeling.

## Exploratory Data Analysis (EDA)
- Visualized sales distribution across **categories, regions, and segments**.  
- Identified **seasonal trends and monthly patterns** in sales data.  
- Correlation analysis between `Sales`, `Discount`, and `Profit`.  
- Detected potential high-performing and low-margin product segments.


## Key Insights
- Sales show strong **seasonal and upward trends** during Q4 (November–December).  
- Profitability varies significantly across categories; **Furniture** has lower profit margins compared to **Technology**.  
- Discounts are negatively correlated with profit, suggesting over-discounting reduces margins.  



## Project Structure
```
├── experiments.ipynb        # Main analysis notebook
├── Sample - Superstore.csv  # Dataset used for analysis
├── README.md                # Project documentation
└── requirements.txt         # Dependencies (pandas, numpy, matplotlib, statsmodels, scikit-learn)
```
