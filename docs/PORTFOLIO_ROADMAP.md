# Portfolio delivery roadmap — December 2026

Target: four runnable, resume-demonstrable core projects by **17 November 2026**,
then feature delivery and hardening through **31 December 2026** for v1 releases.
This is a delivery plan, not a claim that future features already exist.

| Project | Current evidence | v1 scope | Detailed plan |
| --- | --- | --- | --- |
| SlotSync | Requester/approver/admin React workflows, versioned duration/approval policy, atomic CSV import/replay and audit; five-case UAT and real app-restart role-state/replay proof | Rich policy/opening hours, CSV mapping/updates, broader UAT and final release acceptance | [Plan](https://github.com/apoorvkumarvcd23-coder/slotsync/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| FieldDesk | Versioned indexing, granted local-model RAG, operator ingest/jobs, opt-in review and human-approved tickets; actual browser/model full app-process restart proof and original offline baseline | Held-out evaluation, broader retention/quotas, recovery and final release hardening | [Plan](https://github.com/apoorvkumarvcd23-coder/fielddesk/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| MarketPulse | One-day typed Parquet/DuckDB/SQL/Streamlit, clean CLI/browser replay and byte-preserving rejection; native public 4,320-key run plus separate Linux offline proof | One-month budgets, broad quarantine/recovery, dbt and final release gates | [Plan](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/blob/main/docs/IMPLEMENTATION_PLAN.md) |
| Data Placement | Safe configuration/events, bounded Redis and actual Kafka/local Spark MLlib/HDFS replay; strict outage denials, verified-mirror offline writes/recovery and browser states | Fair replay benchmarks, model persistence, broader checkpoint/recovery and final acceptance | [Plan](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/blob/main/docs/IMPLEMENTATION_PLAN.md) |

## Immediate core sprint

Ten build days run 7–16 November, with 17 November reserved for acceptance and
repairs. Core work began with SlotSync on 7 November. Verified slices are shown
above; remaining workflows still need their scheduled implementation/acceptance.

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
SlotSync's five-case booking/configuration/import UAT and FieldDesk's full
app-process stop/start with fresh cited inference are verified on 16 November.
Final four-project clean-clone/claim audit remains 17 November before core tags.

Daily work produces meaningful verified changes, with no empty, padded or
backdated commits. Missed tasks carry forward according to dependencies.
