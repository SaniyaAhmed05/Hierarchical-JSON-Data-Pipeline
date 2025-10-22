# Hierarchical JSON Data Pipeline
# Overview
I built an end-to-end ETL pipeline to transform complex, nested JSON data from a web API into clean, structured datasets that are ready for analysis.

The journey starts with raw JSON data that can be deeply nested and hard to query. Using Apache Spark, I transformed this data into structured DataFrames, flattening arrays and nested fields to make it easy to work with. The processed data is then stored in AWS S3 in Parquet format, which is not only highly efficient in storage but also significantly faster to query.

To make the pipeline reliable and automated, I orchestrated the workflow using AWS Step Functions, ensuring it can run at scale and recover gracefully from errors. The result is a pipeline that delivers clean, optimized, and ready-to-use data for downstream analytics and business reporting.


# The repository directory structure is as follows:
```hierarchical-json-data-pipeline/
│
├── README.md
│
├── src/
│ └── etl.py # Single file containing Extract, Transform, Load
│
│
├── data/
│ ├── raw/ # Sample raw JSON data from Web API
│
│ └── processed/ # Output examples of flattened data
│
└── images/
└── architecture_web_api.png # Architecture diagram
```
# Tools
To build this project, the following tools were used:
* AWS S3
* Apache Spark
* AWS EMR
* Python
* RDDs
* DataFrames
* AWS Step Functions
* Parquet Format
* Git
* Web API
# Architecture
Following is the architecture of the project.

