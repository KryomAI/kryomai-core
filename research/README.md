# KryomAI Core Research

This folder organizes research activity. It holds proposals and records.
It holds no implementation code at this stage.

Current status: no active studies. No results to report.

## How research starts

1. Write a short proposal referencing the roadmap question it addresses.
2. Name datasets, licenses, baselines, metrics, and compute budget.
3. Define exit criteria and what counts as a negative result.
4. Gain review against [research-principles.md](../docs/research-principles.md)
   and [safety-and-governance.md](../docs/safety-and-governance.md).
5. Only then create the minimal folder the proposal needs.

No speculative domain folders. No placeholder modules.

## Proposal template (future)

- Title and roadmap domain (or subdomain).
- Research question and hypothesis.
- Datasets with source, version, and license.
- Baselines and pre-registered metrics.
- Compute budget, seeds, and environment.
- Risks, ethics, and safety notes.
- Exit criteria.

## Experiment record template (future)

- Proposal link and config version.
- Dataset versions and processing scripts.
- Seeds, environment lock, and run logs.
- Metric outputs with variance and tolerance.
- Separation of demonstrated results from open questions.

## Dataset cards (future)

Each dataset used must record:

- Source, version, and access date.
- License and permitted uses.
- Preprocessing steps and script versions.
- Known limitations and biases.

For R0–R2, only public-domain and clearly open-licensed datasets
are used. Incompatible or unverifiable licenses block the study.

## Boundaries

- CPU-first for R0–R2. GPU-dependent proposals are out of scope
  until the R3 gate opens.
- Biomedical work is non-clinical and needs ethics review.
- Robotics work stays simulated and offline.
- Results here never become products directly; promotion follows
  the R4 stable-interface criteria.
