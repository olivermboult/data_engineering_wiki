# Source Systems & Integration

## Purpose

Design robust, observable ingestion from all data sources with clear contracts and schedules.

## Outcomes

An ingestion inventory, mappings, and reliable pipelines with error handling and retries.

## Decisions to Make

- Batch vs. streaming vs. micro-batch
- Connectivity (gateways, private endpoints, shortcuts)
- Cadence, change data capture (CDC) vs. full loads
- Idempotency and schema drift handling

## Standards & Patterns

- Source-to-landing (raw) mapping per feed
- Standard landing formats (Delta/Parquet)
- Parameterized pipelines and consistent naming

## Deliverables & Artifacts

- Source inventory
- Source-to-raw mappings
- Ingestion runbooks and schedules
- Error handling patterns

## Checklist

- [ ] All sources catalogued
- [ ] Connectivity methods confirmed
- [ ] Mappings approved
- [ ] Error handling tested

