# KryomAI Core Evaluation and Benchmarking

How scientific and engineering intelligence gets measured. No
harness, benchmark, or result exists yet.

## Harness design

- CPU-runnable first: every benchmark runs on the R0–R2
  workstation before any accelerated variant is considered.
- Fixed task sets, fixed metric versions, locked environments.
- One command reproduces one reported number from a clean
  checkout plus recorded data versions.

## Preregistration and baselines

- Metrics and baselines are declared before runs, not after.
- The simplest reasonable baseline runs first, including open
  models used as references where appropriate.
- Post-selected metrics are reported as exploratory, never as
  findings.

## Reporting standard

- Every number carries variance, tolerance, seed count, and
  environment identity.
- Single-seed wins are not findings.
- Negative results and failures publish alongside positive ones.

## Per-domain notes

Each domain evaluates on small, licensed, verifiable task sets
before any larger effort: formal checks for reasoning and
mathematics; execution checks for coding; consistency metrics
for physics; simulator tracks for quantum; sim-only policies
for robotics; resource-profiled planning for aerospace;
verifiable design tasks for semiconductors; open property sets
for materials; licensed sequence tasks (plus ethics-gated
non-clinical tasks for the medicine subdomain) for
biotechnology; licensed mini-benchmarks for multimodal work;
and small design-reasoning sets for engineering.

## Independence

- Evaluation code is written and tested separately from the
  methods under study.
- Benchmark additions need proposal review like datasets do.
