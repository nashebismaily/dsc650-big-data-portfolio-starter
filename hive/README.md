# Apache Hive — Managed Table & SQL Validation

## Role in the Pipeline

Apache Hive provides the structured SQL layer between HDFS storage and the Spark MLlib workload. The project data loaded through NiFi into HDFS is used to create and populate a Hive managed table.

## Hive Table Design

**Table name:** `[Enter table name]`

Explain the table schema and the key design choices made for the project dataset, including important column names, data types, and any decisions needed to make the data usable for downstream Spark processing.

## SQL Files

- [`create_tables.sql`](create_tables.sql) — table creation and data-loading SQL
- [`queries.sql`](queries.sql) — validation, exploration, and aggregation queries

## Data Load Verification

Explain how you confirmed that the data was successfully loaded into the managed Hive table.

![Hive Load Results](screenshots/hive-load-results.png)

## Query & Aggregation Verification

Describe the representative queries used to validate the populated table. Include at least one aggregation query and explain what the results demonstrate about the dataset and schema.

![Hive Query Results](screenshots/hive-query-results.png)

The validated Hive table becomes the structured input used by the PySpark MLlib application.
