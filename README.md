# E-commerce Data Analysis Project

A comprehensive data analysis project using BigQuery's public e-commerce dataset to extract business insights, perform customer segmentation, and forecast revenue.

## Overview

This project analyzes e-commerce sales data to derive actionable business intelligence through:

- Product performance analysis
- Customer segmentation using RFM analysis
- Revenue forecasting with time series models

## Data Source

The analysis uses Google BigQuery's public dataset `bigquery-public-data.thelook_ecommerce` with the following tables:

- `orders`
- `order_items`
- `inventory_items`

## Dependencies

- `google-cloud-bigquery`
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`
- `sklearn`
- `tensorflow`
- `statsmodels`
- `prophet`

## Analysis Components

1. **Data Preparation**
   - Fetching data from BigQuery
   - Merging orders, order items, and inventory tables
   - Data cleaning and preprocessing

2. **Product Analysis**
   - Distribution of product costs
   - Daily sales tracking
   - Product category distribution
   - Top 10 products by revenue

3. **Customer Segmentation (RFM Analysis)**
   - Recency: Days since last purchase
   - Frequency: Number of purchases
   - Monetary: Total spending
   - K-means clustering of customers
   - Customer tier classification:
     - Best Customers (1-1-1)
     - High-spending New Customers (1-4-1, 1-4-2)
     - Low-Spending Active Loyal Customers (1-1-3, 1-1-4, 2-1-3, 2-1-4)
     - Churned Best Customers (4-1-1, 4-1-2, 4-2-1, 4-2-2)

4. **Revenue and Income Forecasting**
   - Time series analysis of daily and monthly patterns
   - Revenue, cost, and income trends
   - Stationarity testing for ARIMA modeling
   - Prophet model for daily and monthly forecasting
   - Forecast evaluation and visualization

## Key Insights

- Product-level insights identify top-performing products
- Customer segmentation enables targeted marketing strategies
- Time series forecasting provides revenue predictions
- Monthly forecasts demonstrate better predictive performance than daily models

## Usage

Run the Jupyter notebook (`main.ipynb`) sequentially to reproduce the analysis.