# RetailFlow Data Engineering Submission

## Source

Official repository: https://github.com/Certisured/retailflow-data-engineering-databricks

Starting point: My own fork of the official repository, cloned from the `main` branch.

## What I built

Completed the RetailFlow Databricks data engineering exercises using PySpark and Delta tables.

The work includes:
- Reading and validating the supplied sales data.
- Cleaning records and separating rejected and duplicate rows.
- Enriching sales with store, product and customer information.
- Creating Bronze and Silver Delta tables.
- Processing incremental sales and handling replay.
- Building final reporting metrics and verification checks.

## Data quality examples

- Repaired the missing unit price for source row `D-004` using product `P004`.
- Rejected source row `D-063` because its quantity was invalid.

## Incremental processing examples

- Corrected sale `S0003` to quantity 4, record version 2.
- Retained late-arriving sale `S0080` with its original business date of 2 January 2026.

## Evidence

Evidence file: `retailflow_final_evidence.png`

The evidence contains the actual final verification output and replay results from Databricks.