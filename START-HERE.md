# Start Here — DSC 650 Final Project Repository

This repository is the required starting structure for the DSC 650 final project.

Your completed GitHub repository is the **final project submission**.

## 1. Create Your Own Repository

Do not submit work or pull requests to the instructor's starter repository.

1. Download or clone the DSC 650 Big Data Portfolio Starter.
2. Create a **new GitHub repository under your own GitHub account**.
3. Use a professional repository name, such as:
   - `big-data-architecture-project`
   - `distributed-data-pipeline`
   - `nifi-spark-hive-hbase-pipeline`
4. Copy the starter repository contents into your new repository.
5. Push the starter files to your GitHub account.
6. Complete the final project in your own repository.

## 2. Keep the Top-Level README

The provided root [`README.md`](README.md) is already designed as the professional landing page for the project.

You do **not** need to rewrite the root README.

Instead:

- replace the screenshot placeholders with your own final-project screenshots;
- replace the starter source-code files with your own working code;
- complete the written explanations in the component README files;
- complete [`docs/project-summary.md`](docs/project-summary.md).

Because the root README references the required screenshot filenames, your own evidence will automatically appear on the portfolio landing page when you replace the placeholder images using the same filenames.

## 3. Required End-to-End Flow

Your completed implementation must follow:

**Source Data → NiFi → HDFS → Hive → Spark MLlib → HBase**

Spark must be submitted through **YARN** using `spark-submit`.

## 4. Where Your Work Goes

| Objective | Location |
|---|---|
| NiFi → HDFS | `nifi/` |
| Hive managed table | `hive/` |
| Environment setup | `docs/` |
| HBase table creation | `hbase/` |
| PySpark MLlib | `spark/` |
| Spark submit / YARN | `spark/` |
| Final HBase verification | `hbase/` |
| Overall summary / challenges | `docs/project-summary.md` |

## 5. Replace Every Placeholder

Before submission, make sure every placeholder code file and screenshot has been replaced with your own work.

Use the required filenames exactly so the root README displays your evidence correctly.

See [`STUDENT-CHECKLIST.md`](STUDENT-CHECKLIST.md) before submitting.

## 6. Submit

Submit the **GitHub URL for your completed repository** in the Week 11 Final Project assignment area.

Your repository must be complete and accessible to the instructor at the time of submission.
