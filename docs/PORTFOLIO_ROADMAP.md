# Portfolio delivery roadmap — December 2026

Target: four runnable, resume-demonstrable core projects by **17 November 2026**,
then feature delivery and hardening through **31 December 2026** for v1 releases.
This is a delivery plan, not a claim that future features already exist.

| Project | Current evidence | v1 scope | Detailed plan |
| --- | --- | --- | --- |
| SlotSync | Planning documents; no runnable code yet | Configurable booking, database overlap protection, approvals, CSV import and UAT | [Plan](https://github.com/apoorvkumarvcd23-coder/slotsync/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| FieldDesk | Working offline retrieval/approved tickets and a 16-question diagnostic | Document permissions, durable indexing, local embeddings/LLM, source checks and review queue | [Plan](https://github.com/apoorvkumarvcd23-coder/fielddesk/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| MarketPulse | Verified market-data sample ingestion, manifests and dlt/DuckDB | Multi-symbol bounded batch processing, quarantine, Parquet, analytics and dashboard | [Plan](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| Data Placement | Kafka/local Spark, EMA/MLlib, Redis/HDFS and dashboard | Safe configuration/events, strict backend policy, fair replay benchmark and recovery | [Plan](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/blob/main/docs/IMPLEMENTATION_PLAN.md) |

## Immediate core sprint

Ten build days run 7–16 November, with 17 November reserved for acceptance and
repairs. Core work starts with SlotSync tonight rather than waiting for December.

- **SlotSync:** transactional booking and roles, basic configuration/approvals,
  resource CSV preview/apply, React workflows, audit and executed UAT.
- **FieldDesk:** versioned documents, durable indexing, real local-model RAG in
  pgvector, document permissions, validated citations and an operator review flow.
- **MarketPulse:** bounded multi-symbol ingestion, trusted Parquet/DuckDB loads,
  idempotency/recovery evidence, SQL summaries and a minimal dashboard.
- **Data Placement:** validated/safe inputs and configuration, strict backend
  policy, seeded workload, automated checks and a recorded integration demo.

Core milestones require code and actual demonstration evidence before they are
used as completed resume claims. A prototype or a planned feature alone does not
satisfy the expanded core scope.

## After the core: 18 November–31 December

Add richer configuration/import workflows, larger held-out RAG evaluations,
analytics engineering, broader recovery and permission tests, fair placement
benchmarks, observability and clean-clone release evidence. Full v1 release
gates run on 28–31 December. If a core gate is still incomplete, fixing it takes
priority over optional extensions.

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
