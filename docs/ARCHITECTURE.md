# CDC Operations Architecture

Architecture style: arc42

## Purpose

Separate operational semantics from deployment implementations.

## Operational Domains

Health

Lifecycle

Leadership

Topology

Scaling

Metrics

Discovery

## Relationships

```
cdc-core
  ↓
cdc-operations
  ↓
platform adapters
```

## Responsibilities

cdc-operations defines operational contracts.

Platform adapters implement those contracts.
