# ANUSANDHAN Development Roadmap

Engineering serves research. No code is written ahead of a documented need.
CPU-first operation is a hard constraint for early stages.

## Stage 0 — Documentation (current)

- Establish vision, principles, architecture, and roadmaps.
- Define research organization in `research/README.md`.
- Accept this foundation after review.
- No source code. No dependencies.

## Stage 1 — Reproducibility skeleton

- Add environment specification with locked versions.
- Add seed, config, and logging conventions.
- Add dataset-card and experiment-report templates.
- Add lint and unit-test setup for future utilities.
- Definition of done: a trivial CPU run is fully reproducible.

## Stage 2 — Evaluation tooling

- Add metric definitions with fixed versions.
- Add baseline runners on small public datasets.
- Add report format separating results from goals.
- Definition of done: baselines reproduce within stated tolerance.

## Stage 3 — Domain pilots (engineering support)

- Add only modules required by an approved proposal.
- One module per responsibility. No speculative folders.
- CPU time and memory budgets enforced and logged.
- Definition of done: independent rerun matches the report.

## Stage 4 — Stable interfaces

- Promote only proven components to versioned APIs.
- Each API needs docs, tests, versioning, and changelog entries.
- External integration, including any future KryomCode or KryomAI use,
  goes through these stable APIs only.

## Testing and quality rules

- Unit tests for utilities. Regression tests for reported numbers.
- Evaluation code is tested separately from methods under study.
- Every dataset addition records source, version, and license.
- Incompatible or unclear licenses block the addition.

## Explicit non-goals

- No GPU-required pipelines in Stages 0–2.
- No empty `src/` scaffolds or placeholder packages.
- No model releases before Stage 3 exit criteria are met.
