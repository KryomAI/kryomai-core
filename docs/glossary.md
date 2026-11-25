# KryomAI Core Glossary

Canonical vocabulary for KryomAI Core documentation. If two documents
disagree on a term, this file wins. Terms are grouped by scope:
project identities, products, then technical terms.

See [decisions.md](decisions.md) for the binding decisions behind
these definitions.

## Project identities

### KryomAI

The overall AI research and foundation-model initiative. KryomAI is
the initiative; KryomAI Core is the project that carries it out.

### KryomAI Core

This project and repository. KryomAI Core exists to research,
design, train, evaluate, and improve proprietary AI models for
scientific and engineering intelligence, and to expose proven
capabilities through stable, versioned APIs and SDKs. None exist
yet; see [vision.md](vision.md). Core owns no product engineering.

### KryomLabs

A separate private research company and platform project. KryomLabs
Platform provides a multidisciplinary environment for research,
experiments, simulations, engineering, and scientific discovery.
KryomLabs is not KryomAI: it is intended to consume KryomAI Core
models through stable, versioned APIs once they exist. No shared
code, models, or internals.

### KryomAI Intelligence OS

A planned product that may consume KryomAI Core models through
stable, versioned APIs. It owns its engineering and repository
independently. No implementation from any prior effort exists in
this repository.

## Products

Each product below is an independent domain effort with its own
engineering and repository. Each may consume KryomAI Core models
through stable, versioned APIs. None is part of Core.

- **KryomCode.** Software engineering assistance product.
- **Kryom Quantum.** Quantum computing product effort.
- **Kryom Robotics.** Robotics and embodied systems product effort.
- **Kryom Cloud.** Cloud platform product effort.
- **Kryom Aerospace.** Aerospace product effort.
- **Kryom Semiconductor.** Semiconductor product effort.
- **Kryom BioTech.** Biotechnology product effort.
- **Kryom Nanotechnology.** Nanotechnology product effort.

## Technical terms

- **Foundation model.** A large model trained on broad data and
  adapted per task or domain. A research goal here, not an existing
  asset.
- **Specialized research model.** A model family member focused on
  one KryomAI Core domain or subdomain.
- **Model family.** Related models sharing architecture lineage,
  training method, and evaluation standards.
- **Domain.** One of the twelve KryomAI Core research domains.
- **Subdomain.** A scoped research area inside a domain, such as
  Medicine and Drug Discovery inside Biotechnology and
  bioinformatics.
- **Cross-cutting capability.** A capability that spans domains,
  such as Agentic Intelligence. Documented where it applies, not
  as a standalone domain.
- **Pretraining.** Initial large-scale training of a model. Future
  work; no pretraining runs exist.
- **Fine-tuning.** Adapting a trained model to narrower tasks or
  domains. Future work; no fine-tuning runs exist.
- **Post-training.** Alignment, calibration, and hardening after
  main training. Future work; none performed.
- **Evaluation harness.** The CPU-runnable tooling that scores
  models on fixed benchmarks. Planned; not yet built.
- **Benchmark.** A fixed task set with fixed metrics used for
  comparison. No KryomAI benchmarks exist yet.
- **Baseline.** The simplest reasonable reference result a new
  method must beat, recorded before comparison runs.
- **Dataset card.** The provenance record for one dataset: source,
  version, access date, license, permitted uses, preprocessing,
  limitations, and biases.
- **Proposal.** The short document that starts a research study:
  roadmap question, datasets, baselines, metrics, budget, risks,
  exit criteria.
- **Experiment record.** The complete account of one run: config,
  dataset versions, seeds, environment, metric outputs, and the
  separation of results from open questions.
- **Stage gate.** A review point a research stage exits only by
  meeting its criteria. Evidence, not dates, opens gates.
- **Stable API.** A versioned interface with documentation, tests,
  and changelog entries. Only proven components earn one.
- **SDK.** Client libraries over the stable APIs. Python-first
  when built. None exists.
- **Reproducibility.** The property that an independent rerun with
  the recorded code, data, seed, and environment matches the
  report.
- **Provenance.** The documented origin and license chain of data,
  models, and results.
- **Distribution name.** The installation name: `kryomai`
  (`pip install kryomai`). It need not match the repository name
  (`kryomai-core`). Not yet published.
- **Import name.** The Python import name: `kryomai`
  (`import kryomai`). It matches the `src/kryomai/` directory.
