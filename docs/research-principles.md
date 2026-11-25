# KryomAI Core Research Principles

These principles are binding. A proposal that conflicts with them is rejected.

## 1. Honest reporting

- Demonstrated capabilities and future goals are stated separately.
- Every claim cites code version, dataset version, seed, and evaluation.
- Negative results and failures are recorded.
- No AGI/ASI claims. Report per-task, per-benchmark evidence only.
- No model, capability, or result is claimed before it is demonstrated
  and independently rerunnable.

## 2. Reproducibility

- CPU-first. Early work must run without specialized hardware.
- Lock environments, configs, and seeds.
- Raw data stays immutable. Processing is scripted and versioned.
- An independent rerun is the standard for acceptance.

## 3. Evaluation discipline

- Define metrics and baselines before running experiments.
- Compare against the simplest reasonable baseline first.
- State tolerance and variance. Single-seed wins are not findings.
- Keep evaluation code independent from the method under test.

## 4. Data provenance and licensing

- Every dataset needs source, version, access date, and license.
- For stages R0–R2, use only public-domain and clearly open-licensed
  datasets. Record licenses, provenance, sources, and usage
  restrictions for every dataset.
- Use only data with a compatible, documented license.
- Media and biomedical data need explicit provenance review.
- Remove or replace data whose license cannot be verified.

## 5. Safety and ethics

- Biotechnology and medical-subdomain work is non-operational until
  reviewed. See [safety-and-governance.md](safety-and-governance.md).
- No clinical advice, diagnosis, or treatment claims.
- Dual-use and biosafety risks are assessed before work begins.
- Robotics work stays in simulation and offline data at this stage.

## 6. Scope control

- Small, verifiable steps before broad programs.
- No speculative implementation folders or placeholder modules.
- Each new module needs an approved proposal and an exit criterion.
- Framework and architecture commitments wait for evidence (D8).

## 7. Ecosystem independence

- KryomAI Core stays an independent research project: KryomLabs and
  individual products integrate through stable, versioned APIs only.
- Shared work, if any, uses those APIs. No hidden coupling through
  internals or private dependencies.
- Terms are defined in [glossary.md](glossary.md).

## 8. Open science

- Prefer open datasets, open methods, and open reports.
- Document enough detail for external reproduction.
- Cite prior work accurately. State what is new and what is replicated.
