# Data Modeling & Standards

## Purpose

Create consistent, performant models fit for analytics and downstream consumption.

## Outcomes

Clear modeling conventions and entity/table specifications with keys and SCD strategy.

## Decisions to Make

- Modeling paradigm (star, 3NF, wide tables) per use case
- Keys (natural vs. surrogate), constraints, relationships
- SCD types and history retention
- Data types, null handling, time zones

## Standards & Patterns

- Star schemas for BI; normalized where needed
- Consistent surrogate key patterns
- Conform shared dimensions where beneficial

## Deliverables & Artifacts

- Logical & physical models
- Modeling conventions
- Entity/table specs and lineage

## Checklist

- [ ] Model paradigm selected per area
- [ ] Key & SCD strategy defined
- [ ] Data types & null rules set
- [ ] Performance validated

