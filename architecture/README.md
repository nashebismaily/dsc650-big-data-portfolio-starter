# Architecture

The project architecture follows the required DSC 650 end-to-end pipeline:

**Source Data → Apache NiFi → HDFS → Apache Hive → Apache Spark MLlib → Apache HBase**

Spark workloads are submitted and managed through **YARN**.

The architecture diagram is stored at:

[`architecture-diagram.png`](architecture-diagram.png)

The diagram provides the high-level view of the pipeline, while the component directories contain the implementation code, written explanations, and execution evidence for each stage.
