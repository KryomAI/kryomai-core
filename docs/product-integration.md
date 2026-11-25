# KryomAI Core Product Integration

How KryomAI Core relates to KryomLabs and to individual products.
Rule first, details after: Core and products live in independent
repositories and integrate only through stable, versioned APIs (D7).

Terms: see [glossary.md](glossary.md).

## The three layers

```text
KryomAI Core (this repository)
  research, models, evaluation, stable APIs and SDKs
        |  stable, versioned APIs only
        v
KryomLabs Platform + independent products
  each owns its engineering and repository
```

Core never absorbs product engineering. Products never reach into
Core internals. The API contract is the only coupling, in both
directions.

## KryomLabs

KryomLabs is a separate private research company and platform
project. Its platform provides a multidisciplinary environment for
research, experiments, simulations, engineering, and scientific
discovery. It is intended to consume KryomAI Core models through
stable, versioned APIs once they exist. No shared code, models, or
internals. No joint releases: each side versions independently.

## Products

Each product below is an independent domain effort. Each may consume
KryomAI Core models and evaluation tooling through stable, versioned
APIs. None exists as a Core deliverable; none is part of this
repository.

- **KryomCode.** Software engineering assistance. Consumes code
  intelligence capabilities when Core publishes them.
- **KryomAI Intelligence OS.** Planned product surface for Core
  intelligence. Consumes served models through versioned APIs.
- **Kryom Quantum.** Quantum computing effort. Consumes quantum-AI
  research outputs within its own engineering.
- **Kryom Robotics.** Robotics and embodied systems. Consumes
  planning and perception research; hardware stays product-side.
- **Kryom Cloud.** Cloud platform. Hosts serving and API delivery
  defined by Core's interface contracts.
- **Kryom Aerospace.** Aerospace effort. Consumes autonomy and
  planning research within its own engineering.
- **Kryom Semiconductor.** Semiconductor effort. Consumes
  design-reasoning research within its own engineering.
- **Kryom BioTech.** Biotechnology effort. Consumes bioinformatics
  research under product-side safety review in addition to Core's.
- **Kryom Nanotechnology.** Nanotechnology effort. Consumes
  materials research within its own engineering.

## Future API and model-family strategy

When Core has proven components, it will expose them as versioned
model families behind a versioned API, with a Python-first SDK.
Design principles live in
[api-and-sdk-strategy.md](api-and-sdk-strategy.md); family planning
lives in [model-strategy.md](model-strategy.md). Neither the API nor
any model family exists today, and no dates are promised.

## Integration rules

- Products integrate with released, versioned Core interfaces only.
- Breaking changes follow the published deprecation policy.
- Product requirements never override Core's research principles or
  safety gates.
- What Core never absorbs: product UIs, product infrastructure,
  hardware drivers, clinical or fielded systems.
