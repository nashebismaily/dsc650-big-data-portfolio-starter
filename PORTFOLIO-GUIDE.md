# DSC 650 GitHub Portfolio Guide

## Purpose

The GitHub repository is both the **final-project submission** and a permanent portfolio record of the technical work completed in DSC 650.

The goal is for a reviewer to understand:

> **What was built → How it works → Why the technologies are used → Evidence that it worked**

The live Google Cloud environment is temporary. The repository preserves the implementation after the cloud resources are no longer running.

## Required Pipeline

**Source Data → NiFi → HDFS → Hive → Spark MLlib → HBase**

Spark execution is submitted through **YARN**.

## Required Artifact Mapping

| Objective | Required Repository Evidence |
|---|---|
| Objective 1 — NiFi → HDFS | `nifi/flow-definition.json`, `nifi/README.md`, `nifi/screenshots/nifi-flow.png`, `nifi-running.png`, `hdfs-ingestion-verification.png` |
| Objective 2 — Hive | `hive/create_tables.sql`, `hive/queries.sql`, `hive/README.md`, `hive-load-results.png`, `hive-query-results.png` |
| Objective 3 — Setup | `docs/project-summary.md`, `docs/screenshots/package-installation.png`, `hbase-thrift-server.png` |
| Objective 4 — HBase Creation | `hbase/commands.txt`, `hbase/README.md`, `hbase-empty-scan.png` |
| Objective 5 — PySpark ML | PySpark source in `spark/`, `spark/README.md`, `spark-training-output.png`, `spark-ml-evaluation.png` |
| Objective 6 — Spark Submit | `spark/README.md`, `spark-submit-output.png` |
| Objective 7 — HBase Verification | `hbase/README.md`, `hbase-populated-scan.png` |

## Written Explanations

Project-specific writing belongs in these files:

- `nifi/README.md` — data source, processors, flow roles, and HDFS destination
- `hive/README.md` — schema design, table decisions, and representative queries
- `spark/README.md` — Hive input, transformations, MLlib algorithm, evaluation, `spark-submit`, and HBase output
- `hbase/README.md` — row key, column families, metrics, and before/after scan interpretation
- `docs/project-summary.md` — overall implementation, environment setup, challenges, results, lessons learned, and production considerations

The top-level `README.md` is already the professional portfolio landing page and does not need to be rewritten.

## Screenshot Quality

Screenshots are technical evidence. They should be readable and show the required result clearly.

Crop out unrelated windows, browser tabs, credentials, tokens, private keys, and other sensitive information.

## Cloud Environment

The repository should remain understandable without access to the original Google Cloud environment. Preserve the code, SQL, flow definition, commands, screenshots, architecture, and written explanations before shutting down cloud resources.

## Final Review

Before submitting:

1. replace all screenshot placeholders;
2. replace all starter code with your own implementation;
3. complete the component README files;
4. complete `docs/project-summary.md`;
5. verify all README images render correctly;
6. verify the repository contains no sensitive information;
7. confirm the instructor can access the repository;
8. submit the repository URL.
