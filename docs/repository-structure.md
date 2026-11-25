# KryomAI Core Repository Structure

Annotated map of this repository. This file is the single authority
for the layout: if the README tree and this file disagree, this file
wins and the README must be fixed.

## Current layout

```text
kryomai-core/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── pyproject.toml
├── .gitignore
├── docs/
│   ├── vision.md
│   ├── mission-and-objectives.md
│   ├── glossary.md
│   ├── architecture.md
│   ├── research-principles.md
│   ├── safety-and-governance.md
│   ├── research-roadmap.md
│   ├── development-roadmap.md
│   ├── product-integration.md
│   ├── model-strategy.md
│   ├── model-architecture.md
│   ├── data-strategy.md
│   ├── training-strategy.md
│   ├── evaluation-and-benchmarking.md
│   ├── inference-and-serving.md
│   ├── api-and-sdk-strategy.md
│   ├── infrastructure-strategy.md
│   ├── repository-structure.md
│   └── decisions.md
├── research/
│   └── README.md
└── src/
    └── kryomai/
        └── __init__.py
```

Notes:

- The tree root is shown as `kryomai-core`, matching GitHub. The
  local folder rename is deferred until after documentation approval
  (D2).
- `src/kryomai/` is the Python package directory (`import kryomai`).
  Distribution name `kryomai` and repository name `kryomai-core`
  intentionally differ (see D11 in [decisions.md](decisions.md)).
- `pyproject.toml`, `src/`, and `LICENSE` are frozen during the
  documentation phase.

## Directory purposes

- `/` — project entry points (README, CHANGELOG, LICENSE) and
  Python project configuration.
- `docs/` — durable decisions, plans, and strategies. Every file
  here constrains future work.
- `research/` — proposals and experiment records. No implementation
  code at this stage.
- `src/` — future Python packages. Today it holds only the minimal
  package initializer.

## Naming conventions

- Documents use lowercase hyphenated names (`data-strategy.md`).
- One topic per file. Cross-references use relative links.
- Code follows the src layout declared in `pyproject.toml`.

## Where new things go

- A durable decision or plan → `docs/`, and link it from the README
  map and this file.
- A study proposal or record → `research/`, per
  [research/README.md](../research/README.md).
- Dataset documentation → alongside the study in `research/`.
  Raw or generated data files are never committed.
- Python code → `src/`, only when a proposal is approved.
- Tests → `tests/`, only alongside the code they cover.
- Nothing speculative: no placeholder modules, no empty scaffolds.

## Strategy documents (v0.2.0)

Eight strategy documents extend `docs/`: `model-strategy.md`,
`model-architecture.md`, `data-strategy.md`, `training-strategy.md`,
`evaluation-and-benchmarking.md`, `inference-and-serving.md`,
`api-and-sdk-strategy.md`, `infrastructure-strategy.md`.
