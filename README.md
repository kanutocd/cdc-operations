# cdc-operations

Operational contracts for the Ruby CDC Ecosystem.

## Purpose

`cdc-operations` defines platform-neutral operational concepts for long-running CDC workloads.

It establishes the vocabulary and contracts used by deployment platforms such as Kubernetes without depending on any particular infrastructure.

## Responsibilities

- Health model
- Lifecycle model
- Leadership model
- Topology model
- Scaling semantics
- Metrics contract
- Service discovery concepts
- Operational vocabulary

## Non-Goals

`cdc-operations` does not:

- define ChangeEvent semantics
- execute processors
- orchestrate workloads
- integrate with Kubernetes
- provide deployment manifests

Those concerns belong elsewhere.

## Relationship

```
Semantic contracts
    ↓
cdc-core
```

```
Operational contracts
     ↓
cdc-operations
```

```
Platform implementations
    ↓
cdc-k8s
cdc-systemd
cdc-ecs
cdc-lambda
```
