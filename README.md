<p align="center">
  <img src="assets/portfolio-banner.png" alt="DSC 650 Big Data Architecture Portfolio" width="900">
</p>

# DSC 650 — Big Data Architecture Final Project

> **Portfolio version:** This repository is designed to preserve and showcase the final DSC 650 implementation after the temporary Google Cloud environment is no longer running.

## What this project demonstrates

This project brings together multiple big-data technologies into a working data pipeline. The final implementation should demonstrate how data is **ingested, stored, queried, processed, and retrieved** using the tools built throughout DSC 650.

The portfolio is centered on four major implementation areas:

- **Apache NiFi** — data ingestion, routing, and flow orchestration
- **Apache Hive** — SQL-based structure and querying over distributed data
- **Apache Spark** — distributed data processing and transformation
- **Apache HBase** — NoSQL storage and record-level retrieval
- **Hadoop/HDFS** — distributed storage supporting the overall environment

The live Google Cloud infrastructure does **not** need to remain online forever. This repository preserves the code, flow definitions, architecture, documentation, and execution evidence so a future employer can still understand what was built.

---

## Architecture

<p align="center">
  <img src="architecture/architecture-diagram.png" alt="DSC 650 reference architecture" width="1000">
</p>

**Important:** Update this diagram or replace it if your final implementation differs.

### Data flow narrative

A portfolio reviewer should be able to understand the project without opening every file.

A typical DSC 650 workflow can be explained at a high level as:

1. **Source data enters the environment.**
2. **NiFi** ingests, routes, and prepares the data.
3. Data is persisted in the distributed environment, including **HDFS** where appropriate.
4. **Hive** provides SQL-accessible tables and queries over the data.
5. **Spark** performs distributed transformations, processing, or analysis.
6. **HBase** provides NoSQL storage and direct retrieval patterns.
7. Screenshots and output files provide evidence that the major components executed successfully.

Replace the description above with the exact flow used in your own project.

---

## Repository structure

```text
DSC650_GitHub_Portfolio_Starter/
│
├── README.md
├── STUDENT-CHECKLIST.md
├── PORTFOLIO-GUIDE.md
├── .gitignore
│
├── assets/
│   └── portfolio-banner.png
│
├── architecture/
│   ├── architecture-diagram.png
│   └── README.md
│
├── nifi/
│   ├── README.md
│   ├── flow-definition.json
│   └── screenshots/
│       └── nifi-flow.png
│
├── hive/
│   ├── README.md
│   ├── create_tables.sql
│   ├── queries.sql
│   └── screenshots/
│       └── hive-query-results.png
│
├── spark/
│   ├── README.md
│   ├── processing.py
│   ├── analysis.py
│   └── screenshots/
│       └── spark-job-results.png
│
├── hbase/
│   ├── README.md
│   ├── commands.txt
│   └── screenshots/
│       └── hbase-scan-results.png
│
├── sample-data/
│   └── README.md
│
└── docs/
    ├── project-summary.md
    └── interview-talking-points.md
```

---

## Apache NiFi

<p align="center">
  <img src="nifi/screenshots/nifi-flow.png" alt="NiFi final flow" width="900">
</p>

NiFi is used to demonstrate the **movement and orchestration of data** through the pipeline.

In your portfolio, explain:

- where the data originated;
- which processors or process groups were important;
- what transformations or routing decisions occurred;
- where NiFi delivered the data;
- any troubleshooting or design decisions you made.

**Files:** [`nifi/`](nifi/)

---

## Apache Hive

<p align="center">
  <img src="hive/screenshots/hive-query-results.png" alt="Hive query results" width="900">
</p>

Hive demonstrates the ability to work with distributed data through a familiar **SQL interface**.

Your repository should preserve:

- table-creation scripts;
- load or external-table definitions, when applicable;
- representative analytical queries;
- screenshots of successful query output.

**Files:** [`hive/`](hive/)

---

## Apache Spark

<p align="center">
  <img src="spark/screenshots/spark-job-results.png" alt="Spark job results" width="900">
</p>

Spark demonstrates **distributed processing and transformation**.

Describe:

- what data Spark reads;
- what transformations or analysis it performs;
- what results are produced;
- why Spark was useful for that part of the pipeline.

**Files:** [`spark/`](spark/)

---

## Apache HBase

<p align="center">
  <img src="hbase/screenshots/hbase-scan-results.png" alt="HBase scan results" width="900">
</p>

HBase demonstrates a **NoSQL access pattern** alongside the SQL-oriented Hive portion of the project.

Preserve:

- table-creation commands;
- representative `put`, `get`, or `scan` commands;
- screenshots showing successful retrieval;
- a short explanation of how HBase differs from the Hive use case in your project.

**Files:** [`hbase/`](hbase/)

---

## Evidence that the system worked

A strong portfolio repository does not just contain code. It also shows **execution evidence**.

Before your Google Cloud credits expire or you delete the environment, capture:

| Component | Evidence to preserve |
|---|---|
| NiFi | Final flow / process-group screenshot |
| Hive | Representative SQL output |
| Spark | Job or processed-data output |
| HBase | `scan` or `get` output |
| Architecture | Final architecture diagram |
| Code | All final scripts and configuration that are safe to publish |

The placeholder images in this starter repository are intentionally obvious. **Replace them with your own screenshots before publishing.**

---

## Technology decisions

Complete this table for your implementation.

| Technology | Role in the project | Why it was appropriate |
|---|---|---|
| Apache NiFi | Data ingestion / orchestration | _Explain your reason_ |
| HDFS | Distributed storage | _Explain your reason_ |
| Apache Hive | SQL access | _Explain your reason_ |
| Apache Spark | Distributed processing | _Explain your reason_ |
| Apache HBase | NoSQL access | _Explain your reason_ |
| Google Cloud | Temporary infrastructure | _Explain your reason_ |

A future employer should be able to see that you understand **why** a technology was used, not only that you were able to run it.

---

## What I learned

Replace this section with 3–5 specific lessons from your project.

Examples:

- Designing a multi-stage data pipeline
- Troubleshooting communication between distributed services
- Working with HDFS-backed data
- Comparing SQL and NoSQL access patterns
- Building Spark transformations
- Designing and debugging NiFi flows
- Operating a multi-service environment in the cloud

---

## Cloud environment lifecycle

The original project environment was deployed using **Google Cloud educational credits**. Because those resources are temporary, the live cloud environment may later be decommissioned.

That does not reduce the value of the portfolio.

This repository is intended to provide a permanent technical record of the project through:

- source code;
- SQL;
- NiFi flow definitions;
- commands and configuration;
- diagrams;
- screenshots;
- execution evidence;
- implementation notes.

---

## Security and publishing notes

Before making this repository public:

- remove usernames and passwords;
- remove API keys and tokens;
- remove private keys and certificates;
- remove public/private IP addresses if they identify your environment;
- do not publish sensitive or restricted datasets;
- do not publish instructor solution material;
- verify screenshots do not expose credentials or personal information.

See [`STUDENT-CHECKLIST.md`](STUDENT-CHECKLIST.md) before publishing.

---

## How to talk about this project in an interview

A future employer may ask:

- What did you build?
- How did data move from source to destination?
- Why did you use NiFi?
- What was stored in HDFS?
- Why use Hive rather than only Spark?
- Why use HBase in addition to Hive?
- What did your Spark code actually do?
- What broke while you were building the system?
- How did you troubleshoot it?
- What would you change for a production deployment?

Use [`docs/interview-talking-points.md`](docs/interview-talking-points.md) to prepare concise answers.

---

## Portfolio objective

The final repository should let a reviewer understand four things quickly:

> **What you built. How it works. Why you designed it that way. Evidence that it worked.**

That is the goal of this portfolio.
