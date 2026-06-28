# cdc-operations

Operational contracts for the Ruby CDC Ecosystem.

`cdc-operations` defines platform-neutral operational concepts for CDC workloads:

- health
- readiness
- draining
- graceful shutdown
- leadership
- scaling pressure
- topology
- metrics contracts

It does not parse WAL, define ChangeEvent semantics, execute processors, or provide Kubernetes manifests.

Those concerns belong to:

- `cdc-core` — CDC semantic contracts
- `cdc-parallel` / `cdc-concurrent` — execution runtimes
- `cdc-kubernetes` — Kubernetes implementation
- `cdc-orchestrator-pro` — orchestration and coordination

The goal is to prevent `cdc-core` from becoming a catch-all shared dictionary.
