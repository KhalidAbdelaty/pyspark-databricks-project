# PySpark and Databricks: End-to-End Data Processing Project

## Project Overview

Welcome to my PySpark and Databricks project! This repository contains an end-to-end data processing and analysis pipeline showcasing the capabilities of PySpark within the Databricks environment. Through this project, I demonstrate how to manage, transform, and visualize big data effectively.

## Table of Contents

- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Datasets](#datasets)
- [Steps Taken](#steps-taken)
  - [1. Schema Definition and Data Loading](#1-schema-definition-and-data-loading)
  - [2. Data Transformation](#2-data-transformation)
  - [3. Data Aggregation](#3-data-aggregation)
  - [4. Visualization](#4-visualization)
- [Results and Insights](#results-and-insights)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)

## Introduction

In this project, I utilized PySpark and Databricks to create a comprehensive data processing pipeline. The aim was to demonstrate the power of PySpark for big data processing and the seamless integration of Databricks for data management and visualization.

## Project Objectives

1. **Data Loading and Schema Definition:** Load sales and menu datasets into dataframes with defined schemas.
2. **Data Transformation:** Add columns such as year, month, and quarter to facilitate time-based analyses.
3. **Data Aggregation:** Perform various aggregations to derive insights, such as total amount spent by customers and products.
4. **Visualization:** Display the transformed data and insights using Databricks' visualization capabilities.

## Datasets

The project utilizes two datasets:
- **Sales Data:** Contains details of product sales including `product_id`, `customer_id`, `order_date`, `location`, and `source_order`.
- **Menu Data:** Contains details of products including `product_id`, `product_name`, and `price`.

## Steps Taken

### 1. Schema Definition and Data Loading

I started by defining schemas for both sales and menu datasets using PySpark's `StructType`. Then, I loaded the datasets from CSV files into dataframes.

### 2. Data Transformation

I added new columns to the sales dataframe: `order_year`, `order_month`, and `order_quarter` using PySpark functions to facilitate time-based analyses.

### 3. Data Aggregation

I performed various aggregations:
- Calculated the total amount spent by each customer.
- Aggregated data to find total spending by product, month, year, and quarter.
- Identified the most popular products by count.
- Filtered data to analyze orders from restaurants specifically.

### 4. Visualization

I used Databricks' `display` function to visualize the results at each step, including aggregations by location and source order.

## Results and Insights

Through this project, I extracted valuable insights:
- **Customer Spending Patterns:** Identified high-value customers and their spending habits.
- **Product Popularity:** Recognized the most popular products and their performance over time.
- **Time-based Trends:** Analyzed spending trends across different time periods (monthly, quarterly, yearly).
- **Regional Insights:** Understood how spending varies by location and order source.

## How to Run

To run this project, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/KhalidAbdelaty/pyspark-databricks-project.git
   ```
2. Open the notebook in Databricks.
3. Run each cell to see the data transformation, aggregation, and visualization steps.

## Conclusion

This project demonstrates the power of PySpark and Databricks for end-to-end data processing and analysis. By leveraging these tools, I was able to manage large datasets, perform complex transformations, and derive meaningful insights efficiently.
