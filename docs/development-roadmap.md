# KryomAI Core Development Roadmap

Engineering serves research. No code is written ahead of a documented
need. CPU-first operation is a hard constraint for R0–R2.

Research stages and their gates live in
[research-roadmap.md](research-roadmap.md). This document defines the
engineering work each stage requires.

## R0 — Documentation (current)

Entry: project chartered.
Scope: establish vision, principles, architecture, roadmaps,
strategies, and research organization.
Exit: v0.1.0 and v0.2.0 documentation reviewed and accepted.
No source code beyond the minimal package initializer. No dependencies.

## R1 — Reproducibility skeleton

Entry: R0 exit.
Scope: environment specification with locked versions; seed, config,
and logging conventions; dataset-card and experiment-report
templates; lint and unit-test setup for future utilities.
Exit: a trivial CPU run is fully reproducible by a second machine.
Measure: identical outputs from a clean environment rebuild.

## R2 — Evaluation tooling

Entry: R1 exit.
Scope: metric definitions with fixed versions; baseline runners on
small public datasets; report format separating results from goals.
Exit: baselines reproduce within stated tolerance.
Measure: three-seed reruns inside tolerance, recorded variance.

## R3 — Domain pilots (engineering support)

Entry: R2 exit, GPU access approved, framework selected.
Scope: only modules required by an approved proposal; one module per
responsibility; compute time and memory budgets enforced and logged.
Exit: independent rerun matches the report.
Measure: reproduced metrics within stated tolerance.

## R4 — Stable interfaces

Entry: R3 exit for promoted components.
Scope: versioned APIs and Python-first SDK for proven components
only; docs, tests, versioning, changelog entries; KryomLabs
integration contract.
Exit: interface test suite passes; deprecation policy published.
Measure: zero breaking changes outside the policy window.

## R5 — Scale-up support

Entry: R4 exit plus dedicated infrastructure and budget approval.
Scope: defined per program in the approving decision. Distributed
training support lives here or not at all.
Exit: defined per program.

## Testing and quality rules

- Unit tests for utilities. Regression tests for reported numbers.
- Evaluation code is tested separately from methods under study.
- Every dataset addition records source, version, and license.
- Incompatible or unclear licenses block the addition.

## Explicit non-goals

- No GPU-required pipelines in R0–R2.
- No empty `src/` scaffolds or placeholder packages.
- No framework or vendor commitments before evidence (D8).
- No model releases before R3 exit criteria are met.
- No serving before R4 exit criteria are met.
