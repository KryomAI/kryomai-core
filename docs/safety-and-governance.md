# KryomAI Core Safety and Governance

Research governance for KryomAI Core: what is allowed, what needs
review, and what blocks work. Binding alongside
[research-principles.md](research-principles.md).

## Scope

This document governs research conduct, data handling, and release
gates. It does not assert legal ownership or corporate structure,
which remain undecided (see P1 in [decisions.md](decisions.md)).

## Data governance

- For stages R0–R2, use only public-domain and clearly open-licensed
  datasets. Record licenses, provenance, sources, and usage
  restrictions for every dataset.
- Every dataset needs a dataset card before use: source, version,
  access date, license, permitted uses, preprocessing, limitations,
  and biases.
- Raw data stays immutable. Processing is scripted and versioned.
- Incompatible or unverifiable licenses block the study. No
  exceptions without a logged decision.

## Dual-use and biosafety review

- Biotechnology, bioinformatics, and the Medicine and Drug Discovery
  subdomain require dual-use and biosafety review before work begins.
- Reviews are recorded with the proposal: risks considered, decision,
  and conditions.
- Work stays non-operational until its review passes.

## Biomedical boundaries

- All biomedical work is exploratory and non-clinical.
- No clinical advice, diagnosis, or treatment claims, in any output.
- Biomedical datasets need ethics review and explicitly licensed data.
- Findings are reported per task and per benchmark, never as medical
  guidance.

## Robotics and hardware containment

- Robotics work stays in simulation and offline datasets.
- No hardware control, laboratory automation, or fielded systems.
- Relaxation requires new review and a logged decision.

## Model-release gates

- No model, checkpoint, or weight release without a logged release
  decision covering evaluation evidence, safety review, and license.
- Model-weight licensing requires a separate future decision and
  explicit approval before any release (D6).
- Until then, no weights leave the research environment under any
  terms.

## API and serving gates

- Nothing is served and no API is offered before the stable-interface
  exit criteria in [development-roadmap.md](development-roadmap.md)
  are met.
- Served components need documentation, versioning, tests, and
  changelog entries first.

## Incidents and retractions

- Errors in published results are corrected publicly and promptly.
- Retracted claims stay visible as retracted, with reasons. History
  is never silently rewritten.
- Safety incidents pause the affected line of work until review
  closes with logged conditions.

## Review cadence

- This document is reviewed at every stage gate.
- Changes take effect only when approved and logged in
  [decisions.md](decisions.md).
