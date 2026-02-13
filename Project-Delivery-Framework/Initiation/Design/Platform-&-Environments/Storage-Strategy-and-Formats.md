# Storage Strategy & Formats

## Purpose

Define storage layout, table/file formats, and optimization policies across layers.

## Outcomes

A physical layout that balances performance, cost, and maintainability.

## Decisions to Make

- Lakehouse, warehouse, or hybrid
- File/table formats (Delta/Parquet/CSV)
- Partitioning, clustering, compaction
- Hot/warm/cold tiers and encryption

## Standards & Patterns

- Medallion layer conventions (raw/curated/serving)
- Partition by date/natural keys where beneficial
- Optimize/compact schedules and vacuum policies

## Deliverables & Artifacts

- Physical storage layout
- Format & partition standards
- Retention settings per layer

## Checklist

- [ ] Layer structure defined
- [ ] Formats & partitions agreed
- [ ] Optimize/vacuum policies set
- [ ] Encryption & access validated

