# Retail Sales Data Analysis Project

This project involves performing data cleaning, exploration, and analysis on a retail sales dataset. The analysis aims to uncover insights into sales performance, customer behavior, profitability, inventory trends, and detect anomalies. Below is a detailed breakdown of the tasks and SQL queries used to clean and analyze the data.

---

## Table of Contents

1. [Data Cleaning](#data-cleaning)
2. [Data Exploration](#data-exploration)
3. [Sales Performance Analysis](#sales-performance-analysis)
4. [Customer Behavior Analysis](#customer-behavior-analysis)
5. [Profitability Analysis](#profitability-analysis)
6. [Inventory and Product Analysis](#inventory-and-product-analysis)
7. [Anomaly Detection](#anomaly-detection)
8. [Sales Trend Analysis](#sales-trend-analysis)
9. [Customer Segmentation](#customer-segmentation)

---

## Data Cleaning

### Checking for NULL Values

The first step in data cleaning is identifying any NULL values in the dataset. This query checks for missing values in the key columns:

```sql
SELECT * FROM retail_sales
WHERE 
    sale_date IS NULL OR sale_time IS NULL OR customer_id IS NULL OR 
    gender IS NULL OR age IS NULL OR category IS NULL OR 
    quantity IS NULL OR price_per_unit IS NULL OR cogs IS NULL;
```
