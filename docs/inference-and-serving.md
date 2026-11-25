# KryomAI Core Inference and Serving

How models will be served once something exists to serve.
Nothing is served today.

## Serving stages

- **Local.** Researcher-side inference for evaluation and
  ablations. Arrives with R2 tooling needs, not before.
- **Shared.** Team-accessible endpoints for pilots. Requires
  R3 exit for the served component.
- **Product.** Serving behind versioned APIs for KryomLabs and
  products. Requires R4 exit: docs, tests, versioning,
  changelog entries.

## Budgets and conduct

- Latency, throughput, and cost budgets are declared per
  served component before it goes live.
- Batch and interactive paths are budgeted separately.
- Served outputs carry model version identity for
  traceability.

## Versioning and rollback

- Served models are versioned artifacts. Rollback to the
  previous version is always available.
- Breaking behavior changes follow the API deprecation
  policy in [api-and-sdk-strategy.md](api-and-sdk-strategy.md).

## Explicit non-goals

- No serving before stage gates, at any stage.
- No production serving from research checkpoints.
- No vendor or platform commitments in this document.
