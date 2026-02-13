# Real-Time & Event Processing (Optional)

## Purpose

Support low-latency analytics and alerting through streaming/event-driven patterns.

## Outcomes

Clearly defined hot/warm/cold paths with SLAs and reprocessing strategies.

## Decisions to Make

- Ingestion (events, CDC, stream processors)
- Materialized aggregations and joins
- Ordering, late data, watermarking
- Retention and reprocessing

## Standards & Patterns

- Separate hot path from serving models
- Idempotent stream processing
- Back-pressure and DLQ handling

## Deliverables & Artifacts

- Streaming topology
- SLAs & monitoring
- Replay/backfill procedures

## Checklist

- [ ] Hot path defined
- [ ] Aggregations validated
- [ ] Late data handled
- [ ] Replay tested

