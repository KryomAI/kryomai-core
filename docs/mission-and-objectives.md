# KryomAI Core Mission and Objectives

## Mission

Research, design, train, evaluate, and improve proprietary AI models
for scientific and engineering intelligence, with every step
reproducible and every claim evidenced.

## Objectives

- **O1 — Reproducible CPU baselines.** Every studied task gets a
  seed-stable CPU baseline with locked environment and config before
  any method work begins.
- **O2 — Evaluation before claims.** No result is reported without
  preregistered metrics, a named baseline, and stated variance and
  tolerance.
- **O3 — Licensed, documented data.** Every dataset used carries a
  dataset card with source, version, access date, license, permitted
  uses, and known limitations. For R0–R2, only public-domain and
  clearly open-licensed datasets are used.
- **O4 — Staged model research.** Small, verifiable studies precede
  larger efforts. A stage advances only when its exit criteria are
  met; see [research-roadmap.md](research-roadmap.md).
- **O5 — Domain specialization with evidence.** Specialized model
  families grow one domain at a time, each backed by reproductions
  and independent reruns.
- **O6 — Stable interfaces for proven work only.** APIs and SDKs are
  granted solely to components with documentation, versioning,
  tests, and changelog entries.
- **O7 — Honest record.** Negative results, failures, and open
  questions are published alongside positive ones.

## Non-objectives

- A general-purpose chatbot or assistant product.
- An API wrapper around existing AI providers.
- Clinical, diagnostic, or therapeutic systems.
- Hardware control, laboratory automation, or fielded robotics.
- Frontier-scale pretraining on workstation hardware.
- Advocacy for any ML framework before evidence (see D8 in
  [decisions.md](decisions.md)).

## What success looks like

- R0: this documentation set is reviewed and accepted.
- R1: dataset cards, baseline scores, and seed-stable CPU runs exist
  for the first studied tasks.
- R2: controlled studies with preregistered metrics separate
  demonstrated results from open questions.
- R3 and beyond: defined by later roadmap revisions once R2 exit
  criteria are met. No dates are promised.

## Review cadence

Objectives are reviewed at every stage gate. Changes are proposed as
decision-log entries in [decisions.md](decisions.md) and take effect
only when approved and logged.
