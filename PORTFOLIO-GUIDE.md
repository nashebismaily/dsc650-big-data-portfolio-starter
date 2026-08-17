# How to Turn the DSC 650 Final Project into a Portfolio Project

## The idea

Your Google Cloud environment is temporary. Your technical work does not have to be.

The purpose of this repository is to preserve the **design, implementation, code, and evidence** from your DSC 650 final project in a form that remains useful after the cloud environment is deleted.

## What employers should see

A strong portfolio should answer these questions quickly:

1. What problem were you solving?
2. What technologies did you use?
3. How did data move through the system?
4. What did you personally build?
5. What code or configuration did you write?
6. What evidence shows that the system worked?
7. What technical decisions did you make?
8. What did you learn?

## What not to do

Avoid a public repository that looks like this:

```text
week-1/
week-2/
week-3/
assignment-4/
final-assignment/
```

That organization may make sense during a course, but it makes the work feel like homework.

Instead, organize the portfolio like an engineering project:

```text
architecture/
nifi/
hive/
spark/
hbase/
docs/
```

## Screenshots are evidence, not decoration

Use screenshots to prove meaningful execution:

- show the completed NiFi flow;
- show successful Hive output;
- show Spark results;
- show an HBase scan or get.

Do not fill the repository with dozens of nearly identical screenshots.

## Use your own language

This starter gives you a structure, but your final README should describe **your actual implementation**. Replace generic text with precise details from your project.

## Keep it safe

A public GitHub repository is not the place for credentials, private keys, sensitive data, or restricted course materials.

Run through `STUDENT-CHECKLIST.md` before publishing.
