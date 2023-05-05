# Home_Sales

## Overview
The file ``Home_Sales.ipynb`` uses PySpark to query a .csv of home sales data. The following operations have been performed:

- CSV is read into a Spark DataFrame
- A temporary table ``home_sales`` is created to perform SQL aggregation queries on the DataFrame using ``spark.sql``
- The temporary table is cached.
- The DataFrame is partitioned on the ``date_built`` field and written to parquet
- The query is re-run on the partitioned parquet file to test runtime.

## Access and Usage
To clone this repository enter the following command

``git clone https://github.com/GPN87/Home_Sales.git``