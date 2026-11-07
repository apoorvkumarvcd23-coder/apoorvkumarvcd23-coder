# Portfolio delivery roadmap — December 2026

Target: four complete, demonstrable local v1 projects by **31 December 2026**.
This is a delivery plan, not a claim that future features already exist.

| Project | Current evidence | v1 scope | Detailed plan |
| --- | --- | --- | --- |
| SlotSync | Planning documents; no runnable code yet | Configurable booking, database overlap protection, approvals, CSV import and UAT | [Plan](https://github.com/apoorvkumarvcd23-coder/slotsync/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| FieldDesk | Working offline retrieval/approved tickets and a 16-question diagnostic | Document permissions, durable indexing, local embeddings/LLM, source checks and review queue | [Plan](https://github.com/apoorvkumarvcd23-coder/fielddesk/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| MarketPulse | Verified market-data sample ingestion, manifests and dlt/DuckDB | Multi-symbol bounded batch processing, quarantine, Parquet, analytics and dashboard | [Plan](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| Data Placement | Kafka/local Spark, EMA/MLlib, Redis/HDFS and dashboard | Safe configuration/events, strict backend policy, fair replay benchmark and recovery | [Plan](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/blob/main/docs/IMPLEMENTATION_PLAN.md) |

## Milestones

- **7–14 November:** establish source evidence, test/build foundations, booking
  schema and versioned knowledge records.
- **15–21 November:** transactional booking/idempotency, document permissions,
  indexing jobs, bounded ingestion plans and backend policy tests.
- **22–28 November:** configurable approval workflows, local model adapters,
  timestamp normalisation, quarantine and safe event processing.
- **29 November–5 December:** requester/operator interfaces, review queue,
  Parquet, cursor isolation and repeatable workloads.
- **6–12 December:** administration/import preview, expanded evaluation, actual
  local-model demonstration, tested analytics/dashboard and model persistence.
- **13–19 December:** atomic imports, worker recovery, executed UAT, telemetry,
  bounded backfill and fair placement benchmark.
- **20–26 December:** full acceptance scenarios, clean-clone deployment,
  controlled recovery, replay and graceful shutdown.
- **27–31 December:** release gates, runbooks, demonstrations and final audit.

## Release acceptance

Each release needs a reproducible setup, synthetic seed data, passing automated
checks, a real end-to-end demonstration, failure/recovery evidence, screenshots
and documented limitations. A version tag is earned by the checks, not the date.

FieldDesk retains a deterministic offline baseline and separately verifies real
local inference. MarketPulse's two-year cloud/live-streaming roadmap is a later
phase. Data Placement separates modelled WAN latency from measured local I/O.
SlotSync does not claim delivered Java functionality until the application runs.

Daily work produces meaningful verified changes, with no empty, padded or
backdated commits. Missed tasks carry forward according to dependencies.
