# KryomAI Core Vision

**Advancing Intelligence Through Research.**

KryomAI Core is the research and development project behind KryomAI:
an independent initiative to research, design, train, evaluate, and
improve proprietary AI models for scientific and engineering
intelligence.

This document defines direction. It claims no results.

## Current status

- Stage: documentation foundation (R0, v0.1.0).
- Implemented models: none.
- Training runs performed: none.
- Published benchmarks or findings: none.
- APIs or SDKs: none.

Every future claim must cite code, data, and evaluation.
See [research-principles.md](research-principles.md).

## Mission

Build reliable methods for understanding and assisting scientific
and engineering work. Favor clarity over scale. Favor measurement
over assertion.

## Long-term goal

Develop proprietary model families specialized per research domain:
scientific reasoning, mathematics, software engineering, physics,
quantum computing, robotics, aerospace, semiconductors,
nanotechnology, biotechnology, multimodal science, and engineering.

KryomAI Core is not a general-purpose chatbot and not an API wrapper
around existing providers. Open models are studied, evaluated, and
used responsibly as references and baselines on the way; they are
not the destination.

None of this exists yet. The goal is stated so progress can be
measured against it, not to imply present capability.

## Research domains

Twelve long-term directions. Each begins with literature review and
small reproducible baselines before any larger effort.

### 1. Scientific research and reasoning

Study how models read literature, form hypotheses, check claims, and
report uncertainty. Early work uses small verifiable tasks with
formal checks, not fluency alone.

### 2. Mathematical and computational intelligence

Study structured reasoning on verifiable problems.
Success requires formal checks, not fluency alone.

### 3. Software engineering and coding

Study code understanding, generation, review, and repair on small
verifiable tasks. Correctness is checked by execution and tests, not
by inspection alone. Product engineering belongs to KryomCode; Core
researches the underlying intelligence.

### 4. Physics and scientific discovery

Explore ML assistance for modelling and analysis tasks.
Physical consistency and uncertainty matter more than fit.

### 5. Quantum computing and Quantum AI

Track quantum ML methods through simulation and literature.
No claim of quantum advantage is made or assumed.

### 6. Robotics and embodied intelligence

Begin with simulation and offline control datasets.
No hardware program is defined at this stage.

### 7. Aerospace research and engineering

Study planning, perception, and autonomy for constrained systems.
Early work is literature and public-dataset based. Product
engineering belongs to its own effort; Core researches the
underlying intelligence.

### 8. Semiconductor and chip design research

Study reasoning about circuits, layouts, and design constraints on
small verifiable tasks. Early work is literature and open-data
based. Fabrication and product engineering are out of scope.

### 9. Nanotechnology and materials science

Study property prediction on open materials datasets.
Experimental validation is out of scope until methods mature.

### 10. Biotechnology and bioinformatics

Focus on public sequence and structure datasets with clear licenses.
Strict safety and dual-use review applies. Includes the Medicine and
Drug Discovery subdomain: exploratory and non-clinical only, with
ethics review and licensed data. No diagnosis or treatment claims.

### 11. Multimodal scientific intelligence

Study joint text, image, and structured-data methods on small
benchmarks. Provenance and licensing of media datasets are mandatory.

### 12. Engineering and new technology development

Study how models assist design, analysis, and trade-off reasoning
across engineering disciplines. Early work is literature and
small-benchmark based.

## Cross-cutting capabilities

Agentic Intelligence — tool use, multi-step reasoning, and sandboxed
autonomy — spans all domains. It is studied in sandboxed tasks with
evaluation and containment, and documented where it applies rather
than as a standalone domain. See [glossary.md](glossary.md).

## Boundaries

- No AGI/ASI claims. Progress is reported per task and per benchmark.
- Sensitive domains stay non-operational until safety review passes.
- KryomAI Core will provide the intelligence layer; KryomLabs
  Platform and other products may consume it through stable,
  versioned APIs. KryomLabs and KryomAI Core are separate projects.
- No training runs, model releases, or serving exist at this stage.

## Reading order

1. [glossary.md](glossary.md)
2. [mission-and-objectives.md](mission-and-objectives.md)
3. [research-principles.md](research-principles.md)
4. [safety-and-governance.md](safety-and-governance.md)
5. [architecture.md](architecture.md)
6. [research-roadmap.md](research-roadmap.md)
7. [development-roadmap.md](development-roadmap.md)
