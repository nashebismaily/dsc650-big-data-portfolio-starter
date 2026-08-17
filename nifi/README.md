# Apache NiFi — Data Ingestion into HDFS

## Role in the Pipeline

Apache NiFi provides the ingestion and orchestration layer for this project. The completed flow retrieves the project dataset and writes it into HDFS for downstream processing.

## Source Dataset

**Dataset:** [Enter dataset name]  
**GitHub direct URL:** [Enter the direct/raw GitHub URL used by the NiFi HTTP processor]

Briefly describe what the dataset contains and why it was selected.

## Flow Design

Describe the important processors used in the final NiFi flow and the role each processor performs.

| Processor / Process Group | Role in the Flow |
|---|---|
| [Processor name] | [What it does] |
| [Processor name] | [What it does] |
| [Processor name] | [What it does] |

Explain how data moves from the source URL through NiFi and into HDFS.

## HDFS Destination

**HDFS path:** `[Enter final HDFS path]`

Explain where NiFi writes the dataset and how the destination is used by the next stage of the pipeline.

## Execution Evidence

### Final NiFi Flow

![NiFi Flow](screenshots/nifi-flow.png)

### Running Flow / Queue Activity

![NiFi Running](screenshots/nifi-running.png)

### HDFS Ingestion Verification

![HDFS Verification](screenshots/hdfs-ingestion-verification.png)

The HDFS screenshot should show the `hdfs dfs -ls` output confirming that the project dataset was successfully written into HDFS.
