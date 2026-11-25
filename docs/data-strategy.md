# KryomAI Core Data Strategy

Dataset licensing, provenance, quality, and governance. Binding
alongside [safety-and-governance.md](safety-and-governance.md).

## Sourcing policy

- For R0–R2, use only public-domain and clearly open-licensed
  datasets. Record licenses, provenance, sources, and usage
  restrictions for every dataset.
- Prefer small, well-documented datasets over large, opaque ones.
- Every dataset needs a dataset card before use.

## Dataset-card schema

Source, version, access date, license, permitted uses,
preprocessing steps with script versions, known limitations and
biases. Cards live with the study in `research/`.

## Provenance and quality

- Raw data stays immutable. Processing is scripted and versioned.
- Quality dimensions recorded per dataset: coverage, noise,
  label reliability, duplication, leakage risks.
- Leakage checks between training and evaluation splits are
  mandatory where splits exist.

## Forbidden data

- Data with incompatible or unverifiable licenses.
- Personal, biometric, or clinical data without explicit review
  and documented legal basis. R0–R2 default: do not use.
- Scraped data with unclear terms of use.

## Per-domain notes

- Scientific research and reasoning: verifiable task sets with
  formal checks; no fluency-only benchmarks.
- Mathematical and computational intelligence: problems with
  machine-checkable answers.
- Software engineering and coding: execution-checked tasks with
  permissive licenses.
- Physics and scientific discovery: constrained regression and
  modelling sets with uncertainty annotations where available.
- Quantum computing and Quantum AI: simulator outputs and
  literature-derived sets.
- Robotics and embodied intelligence: simulation and offline
  control datasets only.
- Aerospace research and engineering: planning and perception
  sets suited to constrained compute.
- Semiconductor and chip design research: open design and
  literature-derived reasoning sets.
- Nanotechnology and materials science: open property datasets.
- Biotechnology and bioinformatics: public sequence and structure
  sets with clear licenses, plus ethics-reviewed biomedical sets
  for the Medicine and Drug Discovery subdomain.
- Multimodal scientific intelligence: small licensed
  text-image-structured sets with full media provenance.
- Engineering and new technology development: literature and
  small-benchmark reasoning sets.

## Governance

- Dataset additions need proposal review. Incompatible licenses
  block the addition without exception.
- This strategy is reviewed at every stage gate.
