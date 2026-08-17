# Interview Talking Points

Use this file to prepare a concise explanation of the project for a technical interview.

## 30-Second Overview

> I built an end-to-end distributed data pipeline using Apache NiFi, HDFS, Hive, Spark MLlib, YARN, and HBase. NiFi ingested the source dataset into HDFS, Hive provided a managed SQL layer, Spark MLlib read the Hive data and trained and evaluated a machine learning model, YARN managed the Spark workload, and Spark persisted the model metrics into HBase. The repository preserves the architecture, code, and execution evidence so the implementation can be reviewed without a live cloud environment.

Rewrite this overview in your own words so it reflects your specific dataset and machine learning implementation.

## Be Ready to Explain

### What problem or analytical task did your dataset support?

[Your answer]

### Walk through the complete data flow.

[Your answer]

### Why did you use NiFi?

[Your answer]

### What role did HDFS play?

[Your answer]

### How did you design the Hive table?

[Your answer]

### What data did Spark read from Hive?

[Your answer]

### Which MLlib algorithm did you use and why?

[Your answer]

### How did you evaluate the model?

[Your answer]

### What did YARN do during Spark execution?

[Your answer]

### Why did you write model metrics into HBase?

[Your answer]

### How did the final HBase scan prove the pipeline worked?

[Your answer]

### What was the most difficult technical problem?

[Your answer]

### How did you troubleshoot it?

[Your answer]

### What would you change for production?

[Your answer]
