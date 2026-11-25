# KryomAI Core Model Architecture Research

How architectures get researched. This is a methodology document.
It selects no architecture and promises none.

## Method

1. Survey the literature for the target capability.
2. Reproduce the simplest published baseline on CPU.
3. Ablate one component at a time with preregistered metrics.
4. Pilot narrowly; promote only through stage gates.

Each step needs an approved proposal per
[research/README.md](../research/README.md).

## Architecture records

- Every studied architecture gets a record: lineage, components,
  training recipe reference, evaluation results, known failures.
- Records live with experiment records, not as code comments.
- Rejected architectures stay recorded with rejection reasons.

## Component studies

- Study components in isolation on CPU-scale tasks before
  combining them.
- Interpretability notes accompany every component study.
- Combined systems inherit every component's known limitations.

## Scaling studies

- Scaling questions are answered with measured small-scale trends,
  never extrapolated claims.
- A scaling study states its compute budget in advance and stops
  at it.

## Selection and rejection criteria

- Select: preregistered metric wins over the simplest baseline,
  reproduced independently, within declared budgets.
- Reject: single-seed wins, post-selected metrics, unreproducible
  runs, budget overruns without a new proposal.

## Deferrals

- Framework choice: v0.2.0 strategy process (D8).
- Serving architecture: [inference-and-serving.md](inference-and-serving.md).
