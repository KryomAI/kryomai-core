# ANUSANDHAN Research Roadmap

Research proceeds in stages. A stage advances only when its exit criteria are met.
No dates are promised. Evidence gates progress.

## Stages

- **Stage 0 — Foundation (current).** Documentation, principles, and roadmaps.
  Exit: this set of docs is reviewed and accepted.
- **Stage 1 — Baselines.** Literature surveys and CPU-scale reproductions.
  Exit: dataset cards, baseline scores, and seed-stable runs.
- **Stage 2 — Controlled studies.** Small ablations with pre-registered metrics.
  Exit: reports separating demonstrated results from open questions.
- **Stage 3 — Domain pilots.** Narrow tasks in selected domains.
  Exit: independent reproduction of key runs.
- **Stage 4 — Integration.** Stable APIs for proven components only.
  Exit: versioned interface, tests, and changelog.

## Research questions by domain

1. **Foundation Models and LLMs.**
   Q: How do open models fail on verifiable tasks?
   M1: evaluation harness on CPU. M2: failure taxonomy. M3: narrow pilot.
2. **Neural Networks and Transformer Architectures.**
   Q: Which components matter on small controlled tasks?
   M1: minimal CPU baseline. M2: ablations. M3: interpretability notes.
3. **Mathematical and Scientific Intelligence.**
   Q: When does structured checking beat free-form generation?
   M1: verifiable problem set. M2: checker comparison. M3: error analysis.
4. **Physics and Scientific Discovery.**
   Q: Can small models respect physical constraints?
   M1: constrained regression baseline. M2: consistency metrics. M3: pilot study.
5. **Quantum AI and Quantum Computing.**
   Q: What transfers from classical simulation to real constraints?
   M1: literature map. M2: simulator baselines. M3: scope decision.
6. **Robotics and Embodied AI.**
   Q: What can offline and simulated control teach before hardware?
   M1: simulator survey. M2: offline baseline. M3: sim-only policy report.
7. **Biotechnology and Bioinformatics.**
   Q: What is learnable from licensed public sequence data?
   M1: dataset cards. M2: baseline classifier. M3: safety-reviewed pilot.
8. **Medicine and Drug Discovery Research.**
   Q: Which non-clinical prediction tasks are reproducible on CPU?
   M1: licensed dataset review. M2: baseline with calibration. M3: ethics-gated pilot.
   Non-clinical only. No diagnostic or therapeutic claims.
9. **Nanotechnology and Materials Science.**
   Q: How far do open property datasets support prediction?
   M1: open-data inventory. M2: baseline regressor. M3: uncertainty study.
10. **Space and Aerospace Research.**
    Q: Which autonomy sub-tasks suit constrained onboard compute?
    M1: task survey. M2: planning baseline. M3: resource-profiled pilot.
11. **Multimodal AI.**
    Q: When does a second modality help on small benchmarks?
    M1: licensed mini-benchmark. M2: unimodal baselines. M3: fusion ablation.
12. **Agentic Intelligence and Autonomous Research Systems.**
    Q: How do multi-step agents behave under sandbox limits?
    M1: sandboxed task set. M2: tool-use baseline. M3: containment report.

## Cross-cutting milestones

- Dataset provenance and licensing documented for every study.
- Seeds, environments, and configs locked for every run.
- Evaluation defined before experiments begin.
- Negative results published alongside positive ones.
- No domain moves to Stage 3 without a Stage 1 reproduction.
