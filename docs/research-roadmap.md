# KryomAI Core Research Roadmap

Research proceeds in stages. A stage is entered only when the
previous stage's exit criteria are met. No dates are promised.
Evidence gates progress.

Terms: see [glossary.md](glossary.md). Binding rules: see
[research-principles.md](research-principles.md) and
[safety-and-governance.md](safety-and-governance.md).

## Stages

### R0 — Foundation (current)

Entry: project chartered with approved decisions (D1–D10 logged).
Exit: v0.1.0 and v0.2.0 documentation reviewed and accepted; zero
unresolved items; this roadmap names all twelve domains identically
to [vision.md](vision.md).

### R1 — Baselines

Entry: R0 exit.
Exit: for each studied task, a dataset card, baseline scores, and
seed-stable CPU runs exist; environments and configs are locked.
Measure: rerun variance within stated tolerance on three seeds.

### R2 — Controlled studies

Entry: R1 exit for the tasks under study.
Exit: reports with preregistered metrics separate demonstrated
results from open questions; negative results published alongside
positive ones.
Measure: every claim traces to code version, dataset version,
seed, and evaluation record.

### R3 — Domain pilots

Entry: R2 exit for the pilot tasks, GPU access approved, and ML
framework selected through the v0.2.0 strategy process.
Exit: independent reproduction of key runs by a second
environment.
Measure: reproduced metrics match the report within stated
tolerance.

### R4 — Stable interfaces

Entry: R3 exit for the promoted components.
Exit: versioned API and SDK surface with documentation, tests,
and changelog entries; KryomLabs integration contract reviewed.
Measure: interface tests pass; deprecation policy published.

### R5 — Scale-up program

Entry: R4 exit plus a dedicated infrastructure and budget
approval with its own logged decision.
Exit: defined per program in the approving decision. Frontier
training lives here or not at all.

## Research questions by domain

1. **Scientific research and reasoning.**
   Q: How do models assist literature review, hypothesis checks,
   and uncertainty reporting on verifiable tasks?
   M1: verifiable task set. M2: checker comparison. M3: pilot study.
2. **Mathematical and computational intelligence.**
   Q: When does structured checking beat free-form generation?
   M1: verifiable problem set. M2: checker comparison. M3: error analysis.
3. **Software engineering and coding.**
   Q: How far do execution-checked tasks support code understanding
   and repair studies on CPU?
   M1: execution-checked task set. M2: baseline comparison. M3: pilot study.
4. **Physics and scientific discovery.**
   Q: Can small models respect physical constraints?
   M1: constrained regression baseline. M2: consistency metrics. M3: pilot study.
5. **Quantum computing and Quantum AI.**
   Q: What transfers from classical simulation to real constraints?
   M1: literature map. M2: simulator baselines. M3: scope decision.
6. **Robotics and embodied intelligence.**
   Q: What can offline and simulated control teach before hardware?
   M1: simulator survey. M2: offline baseline. M3: sim-only policy report.
7. **Aerospace research and engineering.**
   Q: Which autonomy sub-tasks suit constrained onboard compute?
   M1: task survey. M2: planning baseline. M3: resource-profiled pilot.
8. **Semiconductor and chip design research.**
   Q: What design-reasoning tasks are checkable without fabrication?
   M1: literature and open-data survey. M2: verifiable task baseline.
   M3: scope decision.
9. **Nanotechnology and materials science.**
   Q: How far do open property datasets support prediction?
   M1: open-data inventory. M2: baseline regressor. M3: uncertainty study.
10. **Biotechnology and bioinformatics.**
    Q: What is learnable from licensed public sequence data?
    M1: dataset cards. M2: baseline classifier. M3: safety-reviewed pilot.
    Includes the Medicine and Drug Discovery subdomain: non-clinical
    prediction tasks with ethics review and licensed data only.
11. **Multimodal scientific intelligence.**
    Q: When does a second modality help on small benchmarks?
    M1: licensed mini-benchmark. M2: unimodal baselines. M3: fusion ablation.
12. **Engineering and new technology development.**
    Q: Which design-reasoning tasks admit verifiable evaluation?
    M1: task survey. M2: baseline comparison. M3: pilot study.

Agentic Intelligence is a cross-cutting capability studied within
these domains under sandbox limits, not a thirteenth domain.

## Cross-cutting milestones

- Dataset provenance and licensing documented for every study.
- Seeds, environments, and configs locked for every run.
- Evaluation defined before experiments begin.
- Negative results published alongside positive ones.
- No domain moves to R3 without an R1 reproduction.
- No framework commitment before the v0.2.0 strategy process (D8).
