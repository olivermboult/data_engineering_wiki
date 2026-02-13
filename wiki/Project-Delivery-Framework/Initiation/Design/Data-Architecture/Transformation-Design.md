# Transformation Design

## Purpose

Define how data moves and is refined across layers with reliable, testable transformations.

## Outcomes

Parameterized, reusable pipelines and notebooks with clear business rule placement.

## Decisions to Make

- Tooling (SQL vs. notebooks)
- Layer policies (raw → curated → serving)
- Backfills, late-arriving data, and idempotency
- Error handling and quarantine patterns

## Standards & Patterns

- Reusable transformation components/libraries
- Declarative mappings where possible
- Consistent folder and naming conventions

## Deliverables & Artifacts

- Transformation specs & mappings
- Reusable library/modules
- Error handling runbooks

## Checklist

- [ ] Reusable patterns implemented
- [ ] Parameterization in place
- [ ] Backfill/late data covered
- [ ] Error/quarantine tested

