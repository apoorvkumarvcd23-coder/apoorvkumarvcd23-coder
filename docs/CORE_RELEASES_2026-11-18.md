# Four runnable portfolio cores — accepted 18 November 2026

All four repositories have an annotated **v0.1.0** core tag. Acceptance completed on **18 November IST**, carried forward from the 17 November target. The tags were created at actual current time after the exact tagged commit passed its complete clean-checkout Linux CI and integration artifact checks.

Native Windows clean-checkout observations are dated **17 November**. SlotSync’s admin loading-race repair and its renewed native browser/UAT run are dated **18 November**. Native PostgreSQL/SQLite proof and Linux PostgreSQL/pgvector/HDFS proof are identified separately in each repository; local Docker was unavailable during the native audit.

## Immutable releases and CI

| Core | Tag and commit | Passing CI |
| --- | --- | --- |
| SlotSync | [v0.1.0](https://github.com/apoorvkumarvcd23-coder/slotsync/tree/v0.1.0) · [82b2c56](https://github.com/apoorvkumarvcd23-coder/slotsync/commit/82b2c56a0064090829e479e71dfd1249e17f1723) | [complete run](https://github.com/apoorvkumarvcd23-coder/slotsync/actions/runs/44158745407) |
| FieldDesk | [v0.1.0](https://github.com/apoorvkumarvcd23-coder/fielddesk/tree/v0.1.0) · [ca4d02a](https://github.com/apoorvkumarvcd23-coder/fielddesk/commit/ca4d02af63c46eee86c9b2cf6e0204ee895acb2d) | [complete run](https://github.com/apoorvkumarvcd23-coder/fielddesk/actions/runs/44157066230) |
| MarketPulse Lakehouse | [v0.1.0](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/tree/v0.1.0) · [074a2e8](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/commit/074a2e860b6c5b82ebedfa423b19aba3f7f2c3e8) | [complete run](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/actions/runs/44157080628) |
| Latency-Aware Data Placement | [v0.1.0](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/tree/v0.1.0) · [a975df6](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/commit/a975df617d05f057a0aa1352b84f5cedfba29858) | [complete run](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/actions/runs/44157091174) |

Each tag’s remote object and peeled commit were verified with GitHub. [Machine-readable release and artifact ledger](core-releases-2026-11-18.json) records the full commits, annotated tag objects, CI jobs and downloaded artifact SHA-256 values. Artifact ZIPs were checked against GitHub’s digests before their structured evidence was inspected. GitHub Actions artifacts expire; the pinned repository runbooks, reports and screenshots remain in the tagged source.

## Demonstrated scope and limits

### SlotSync

39 PostgreSQL integration checks; 14 React tests and production build; readiness/outage recovery; five browser scenarios, five business UAT cases and exact role-state/actor-key replay after app restart.

Synthetic accounts and bounded UAT. Opening hours, richer policy rules, CSV update/mapping and broader load/security UAT remain December work.

[Contract, runnable demo and claim-to-code/test ledger](https://github.com/apoorvkumarvcd23-coder/slotsync/blob/v0.1.0/docs/CORE_ACCEPTANCE.md).

### FieldDesk

61 tests each on SQLite and pgvector; actual nomic 768-dimensional embeddings and Qwen3.5:9b generation; granted citations, unsupported/revoked/outage/1 ms handoffs; worker crash/replay and four fully exited app processes with preserved ticket/review/job state and fresh cited inference.

Synthetic workflow proof does not establish held-out answer accuracy. Original 16-case offline diagnostic is retained (9/10 answerable top-1, 4/6 unsupported handoff, 18/18 source quotations); it is separate from actual-model evidence. The 40-case evaluation, broader retention/quotas and production ticket-provider integration remain.

[Contract, runnable demo and claim-to-code/test ledger](https://github.com/apoorvkumarvcd23-coder/fielddesk/blob/v0.1.0/docs/CORE_ACCEPTANCE.md).

### MarketPulse Lakehouse

162 tests; real CLI/dlt/DuckDB/Parquet and Chromium workflow; ms/us fixtures each load/replay nine unique keys; bad checksum and invalid OHLC preserve all trusted bytes. Separate native 17 November public BTC/ETH/SOL run/replay each reconciles 4,320 keys.

One public UTC day and tiny Linux offline fixtures, without month-scale or throughput claims. Linux CI does not download public archives. Month budgets, dbt/marts and broader recovery remain.

[Contract, runnable demo and claim-to-code/test ledger](https://github.com/apoorvkumarvcd23-coder/marketpulse-lakehouse/blob/v0.1.0/docs/CORE_ACCEPTANCE.md).

### Latency-Aware Data Placement

63 Linux tests; actual Kafka/local Spark MLlib/Redis with real HDFS and simulated-cloud runs; each seeded trace reconciles 148 received = 144 accepted + 3 invalid + 1 duplicate. Actual NameNode/DataNode outage/recovery, five strict denials, verified mirrors and ten checked HDFS files.

Single-node integration lab with synthetic data. Tier/WAN latency is modelled and local I/O is measured separately. Tiny-fixture cycle rates and overlapping rolling windows are not fair held-out predictive or performance benchmarks. Model persistence, checkpointing and fair baselines remain.

[Contract, runnable demo and claim-to-code/test ledger](https://github.com/apoorvkumarvcd23-coder/Intelligent-Latency-Aware-Data-Placement-/blob/v0.1.0/docs/CORE_ACCEPTANCE.md).

## Acceptance repairs

The first SlotSync acceptance run [failed](https://github.com/apoorvkumarvcd23-coder/slotsync/actions/runs/44157053877): an initial policy fetch could overwrite the admin’s edit before saving. Controls now wait for policy readiness. A deterministic deferred-response regression fails before the repair and passes after it; browser checks also verify the actual saved policy response. Only the repaired commit was tagged.

MarketPulse’s fresh Windows checkout exposed CRLF/LF formatter disagreement. Its new .gitattributes gives fresh checkouts LF consistently; a separate fresh clone with core.autocrlf=true passes the normal lint/format commands without an override. Existing user edits were preserved.

## Next through 31 December

The cores are available for demos with the limits above. Richer SlotSync policy/opening-hours work is the earliest carried extension; held-out RAG evaluation, month-scale analytics, fair placement benchmarks and release hardening follow the [delivery roadmap](PORTFOLIO_ROADMAP.md). No v1.0.0 release, production deployment, benchmark win or future feature is implied by these core tags.
