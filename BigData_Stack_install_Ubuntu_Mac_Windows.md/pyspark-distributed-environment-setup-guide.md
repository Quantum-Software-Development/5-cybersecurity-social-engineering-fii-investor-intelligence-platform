# PySpark Distributed Environment Setup Guide

## Objective

Create a distributed data processing environment using Apache Spark and PySpark for analytics, ETL pipelines, and Data Engineering workflows.

## Prerequisites

- Java installed
- Apache Spark installed
- Python installed

## Create a Virtual Environment

```bash
python3 -m venv pyspark-env
```

### Linux/macOS

```bash
source pyspark-env/bin/activate
```

### Windows

```cmd
pyspark-env\Scripts\activate
```

## Install PySpark

```bash
pip install pyspark
```

Verify installation:

```bash
python -c "import pyspark; print(pyspark.__version__)"
```

## Create a Spark Session

```python
from pyspark.sql import SparkSession

spark = SparkSession.builder \
    .appName("BigDataLab") \
    .getOrCreate()
```

## Create a Sample DataFrame

```python
data = [
    ("FII_A", 100),
    ("FII_B", 200)
]

df = spark.createDataFrame(
    data,
    ["Fund", "Value"]
)

df.show()
```

## Read a CSV File

```python
df = spark.read.csv(
    "funds.csv",
    header=True,
    inferSchema=True
)
```

## Read Data from MinIO

```python
spark.read.format("csv").load(
    "s3a://bigdata-lake/funds.csv"
)
```

## Perform a Simple Aggregation

```python
df.groupBy("Fund").sum("Value").show()
```

## Stop the Spark Session

```python
spark.stop()
```

## Validation Checklist

- PySpark installed
- Spark session created
- DataFrame created
- CSV file loaded
- MinIO integration tested
- Aggregation executed successfully

## Summary

PySpark provides distributed processing capabilities for large-scale datasets, enabling ETL pipelines, analytics, reporting, and machine learning workflows across Data Lake and Hadoop-based environments.
