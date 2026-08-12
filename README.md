# Online Retail Big Data Analytics

## Project Overview

This project analyses the **Online Retail II** dataset using two different data-processing approaches:

* **Python Pandas** as the conventional approach
* **Apache Spark using PySpark and Spark SQL** as the Big Data Analytics approach

The project focuses on comparing both approaches while analysing sales performance and customer purchasing behaviour.

## Project Objectives

1. To process a large online retail dataset using Apache Spark SQL.
2. To identify sales patterns and customer purchasing behaviour.
3. To analyse revenue across countries and products.
4. To compare Apache Spark with Python Pandas.

## Research Questions

* Which countries generate the highest revenue?
* Which products sell the most?
* Which products generate the highest revenue?
* Which customers spend the most?
* How does monthly revenue change?
* How many cancelled transactions exist?

## Dataset

**Dataset:** Online Retail II
**Source:** UCI Machine Learning Repository
**Worksheet used:** `Year 2009-2010`
**Number of records:** 525,461 transactions

The dataset contains information such as invoice number, product code, product description, quantity, invoice date, price, customer ID, and country.

Dataset link:
`Insert UCI dataset URL here`

## Files

```text
online-retail-big-data-analysis/
│
├── pandas_analysis.ipynb
├── spark_analysis.ipynb
└── README.md
```

### pandas_analysis.ipynb

Contains:

* data exploration
* preprocessing using Pandas
* data transformation
* business analysis
* execution-time measurement

### spark_analysis.ipynb

Contains:

* PySpark environment setup
* Spark DataFrame preprocessing
* data transformation
* Spark SQL / PySpark analysis
* execution-time measurement
* visualisations

## Data Preprocessing

Equivalent preprocessing rules were applied in both Pandas and PySpark, including:

* duplicate removal
* missing-value handling
* identification of cancelled transactions
* removal of invalid completed-sales records
* data type conversion
* revenue calculation
* extraction of date and time variables

After preprocessing, both approaches produced **400,916 valid sales records**.

## Analysis

The project analyses:

* revenue by country
* top-selling products
* highest-revenue products
* highest-spending customers
* monthly revenue trends
* cancelled transactions

## Pandas vs PySpark Comparison

Both implementations produced consistent preprocessing and analytical outputs.

| Approach | Preprocessing Time |
| -------- | -----------------: |
| Pandas   |       3.90 seconds |
| PySpark  |      32.14 seconds |

Pandas performed faster for the dataset used in this project because the data could fit within available memory. PySpark, however, provides a scalable processing framework designed for larger and distributed workloads.

## Technologies Used

* Python
* Pandas
* Apache Spark
* PySpark
* Spark SQL
* Google Colab
* Matplotlib

## Running the Notebooks

The notebooks were developed using **Google Colab**.

1. Open the required `.ipynb` notebook in Google Colab.
2. Make the Online Retail II dataset available to the notebook.
3. Update the dataset file path if necessary.
4. Run the notebook cells sequentially.
