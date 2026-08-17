# DSC 650 Final Project — GitHub Submission Checklist

Complete this checklist before submitting your repository URL.

## Repository

- [ ] My final project is in a repository under my own GitHub account.
- [ ] I did not submit changes or a pull request to the instructor's starter repository.
- [ ] The instructor can access my repository.
- [ ] I kept the required folder structure.
- [ ] The root `README.md` renders correctly.

## Objective 1 — NiFi → HDFS

- [ ] `nifi/flow-definition.json` contains my final NiFi flow.
- [ ] `nifi/README.md` explains the data source, processors, processor roles, and HDFS destination.
- [ ] `nifi/screenshots/nifi-flow.png` shows my final flow design.
- [ ] `nifi/screenshots/nifi-running.png` shows the flow running with data visible in queues.
- [ ] `nifi/screenshots/hdfs-ingestion-verification.png` shows `hdfs dfs -ls` confirming ingestion.

## Objective 2 — Hive

- [ ] `hive/create_tables.sql` contains my table creation / load SQL.
- [ ] `hive/queries.sql` contains my representative validation and aggregation queries.
- [ ] `hive/README.md` explains my schema design and what the queries demonstrate.
- [ ] `hive/screenshots/hive-load-results.png` shows successful loading.
- [ ] `hive/screenshots/hive-query-results.png` shows query and aggregation results.

## Objective 3 — Environment Setup

- [ ] `docs/screenshots/package-installation.png` shows the required package installation.
- [ ] `docs/screenshots/hbase-thrift-server.png` shows the HBase Thrift server running.
- [ ] `docs/project-summary.md` explains why the packages and Thrift server are required.

## Objective 4 — HBase Table Creation

- [ ] `hbase/commands.txt` contains my HBase table-creation commands.
- [ ] `hbase/README.md` explains my row key and column-family design.
- [ ] `hbase/screenshots/hbase-empty-scan.png` shows the empty table before Spark writes metrics.

## Objective 5 — PySpark MLlib

- [ ] My complete working PySpark MLlib source code is in `spark/`.
- [ ] Spark reads the project data from Hive.
- [ ] My code trains and evaluates an MLlib model.
- [ ] My code generates model-performance metrics for HBase.
- [ ] `spark/README.md` explains the algorithm, rationale, input data, transformations, and evaluation results.
- [ ] `spark/screenshots/spark-training-output.png` shows successful training.
- [ ] `spark/screenshots/spark-ml-evaluation.png` shows the evaluation metric(s).

## Objective 6 — Spark Submit / YARN

- [ ] `spark/README.md` includes my `spark-submit` command.
- [ ] `spark/screenshots/spark-submit-output.png` shows successful execution/log output through YARN.

## Objective 7 — HBase Verification

- [ ] `hbase/screenshots/hbase-populated-scan.png` shows the populated table after Spark runs.
- [ ] `hbase/README.md` explains the metrics written by Spark and how the scan verifies the pipeline.

## Overall Documentation

- [ ] `architecture/architecture-diagram.png` is present.
- [ ] `docs/project-summary.md` includes my implementation summary.
- [ ] I documented what worked and what did not.
- [ ] I documented meaningful challenges and how I addressed them.
- [ ] I summarized the final results.
- [ ] I included lessons learned.
- [ ] I explained what I would change for a production deployment.
- [ ] My dataset is my own and is not a course-provided example dataset.
- [ ] My direct GitHub dataset URL is documented.

## Security

- [ ] No passwords are committed.
- [ ] No API keys or access tokens are committed.
- [ ] No private keys or certificates are committed.
- [ ] No sensitive or restricted data is committed.
- [ ] No personally identifiable information is exposed.
- [ ] No instructor solution material is included.
- [ ] My screenshots do not expose credentials or sensitive environment information.

## Final Submission

- [ ] All starter placeholders have been replaced with my own work.
- [ ] All required images display correctly in GitHub.
- [ ] All links in the repository work.
- [ ] My repository is complete.
- [ ] I submitted the GitHub repository URL in the Week 11 Final Project assignment area.
