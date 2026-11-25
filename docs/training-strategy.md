# KryomAI Core Training Strategy

How pretraining, fine-tuning, and post-training will work. No
training runs exist. Strategy first; the first run needs an
approved proposal under these rules.

## Staged training

- **R1–R2 (CPU only).** Tiny studies inside workstation budgets:
  locked configs, seeds, and environments. If a run does not fit
  the R2 budget, it waits for R3; budgets are ceilings, never
  targets.
- **R3 (GPU-gated).** Domain pilots after R2 exit, approved GPU
  access, and framework selection. One proposal per pilot.
- **R4–R5.** Interface-driven retraining and scale-up programs,
  each under its own approving decision with budget and gates.

## Reproducibility rules

- One run equals one config plus one seed plus one environment
  lock, all checked in before the run.
- Configs are declarative. Randomness is seeded and logged.
- Budgets (time, memory, and later accelerators) are declared in
  advance and logged after.

## Checkpoints and records

- Checkpoints are versioned artifacts with training lineage:
  config, data versions, seed, environment, and eval snapshot.
- No checkpoint leaves the research environment without passing
  the release gates in
  [safety-and-governance.md](safety-and-governance.md).

## Fine-tuning and post-training

- Same gates as pretraining: preregistered metrics, baselines,
  variance, reproduction.
- Post-training (alignment, calibration, hardening) is defined
  per proposal with its own acceptance criteria.

## CPU limits, stated plainly

- The current workstation (Intel i5, 16 GB RAM, 512 GB SSD) is
  an R0–R2 machine. Frontier-scale foundation-model pretraining
  is not feasible on it and is never scheduled on it.
- Graduation triggers to R3-class compute: dataset size, run
  time, or memory need exceeding the declared R2 budget.

## Deferrals

- Framework selection: v0.2.0 strategy process (D8).
- Infrastructure specifics: see
  [infrastructure-strategy.md](infrastructure-strategy.md).
