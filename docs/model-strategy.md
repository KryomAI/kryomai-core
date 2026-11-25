# KryomAI Core Model Strategy

Strategy for proprietary model-family development. No models exist;
this document defines what will be built, in what order, and under
what gates — not how to build it today.

## Goal

Develop proprietary model families specialized per research domain,
backed by reproductions and independent reruns at every step.

## Family taxonomy

- **Domain specialists.** One family line per research domain,
  trained and evaluated against that domain's benchmarks.
- **Shared backbone (research question).** Whether domains share a
  common pretrained backbone is undecided. It becomes a proposal
  only with falsifiable criteria: shared training must beat
  per-domain training on at least two domains' preregistered
  metrics, at comparable compute, or the question stays open.
- **Subdomain variants.** Members such as a Medicine and Drug
  Discovery variant inherit their parent domain's gates plus
  subdomain safety review.

## Build versus adapt

- Open models are references and baselines first: study, evaluate,
  reproduce, then decide.
- Adaptation of an open model requires the same gates as building:
  preregistered metrics, baselines, variance, reproduction.
- Building from scratch starts tiny (R2 CPU budgets) and grows only
  through gates. No size is promised at any stage.

## Specialization order

- Domains specialize one at a time, led by R1/R2 evidence strength.
- No domain starts R3 pilots without R1 reproductions.
- The order is decided per stage gate and logged in
  [decisions.md](decisions.md).

## Release and versioning

- Model releases follow the gates in
  [safety-and-governance.md](safety-and-governance.md): evaluation
  evidence, safety review, and license decision first.
- Weights need a separate licensing decision before any release (D6).
- Released families carry semantic versions and changelog entries.

## What this strategy does not do

- Name architectures, sizes, or performance targets.
- Name frameworks or infrastructure vendors.
- Promise dates or release order beyond the gating rules above.
