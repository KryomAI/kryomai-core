# KryomAI Core

**Advancing Intelligence Through Research.**

KryomAI Core is the research and development project behind KryomAI:
an independent initiative to research, design, train, evaluate, and
improve proprietary AI models for scientific and engineering
intelligence.

> **Status:** R0 v0.1.0 — documentation foundation, pre-implementation.
> No models are implemented. No experimental results are claimed.
> See [CHANGELOG.md](CHANGELOG.md).

## Research vision

KryomAI Core investigates machine intelligence for science and
engineering through reproducible, staged research.
The long-term scope spans twelve domains:

1. Scientific research and reasoning
2. Mathematical and computational intelligence
3. Software engineering and coding
4. Physics and scientific discovery
5. Quantum computing and Quantum AI
6. Robotics and embodied intelligence
7. Aerospace research and engineering
8. Semiconductor and chip design research
9. Nanotechnology and materials science
10. Biotechnology and bioinformatics
11. Multimodal scientific intelligence
12. Engineering and new technology development

Medicine and Drug Discovery is a subdomain of Biotechnology and
bioinformatics. Agentic Intelligence is a cross-cutting capability.

These are research directions, not demonstrated capabilities.
Details are in [docs/vision.md](docs/vision.md)
and [docs/research-roadmap.md](docs/research-roadmap.md).

## Principles

- CPU-first development initially. No GPU dependency for early work.
- Reproducibility by default: seeds, environments, datasets, and evaluation.
- Honest reporting: demonstrated results are kept separate from future goals.
- Dataset provenance and licensing are documented before use.
- For R0–R2, only public-domain and clearly open-licensed datasets.
- No unsupported AGI/ASI claims.
- Safety and ethics review for sensitive domains.

Full principles: [docs/research-principles.md](docs/research-principles.md).
Governance: [docs/safety-and-governance.md](docs/safety-and-governance.md).

## Repository structure

```text
kryomai-core/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── pyproject.toml
├── .gitignore
├── docs/
│   ├── vision.md
│   ├── mission-and-objectives.md
│   ├── glossary.md
│   ├── architecture.md
│   ├── research-principles.md
│   ├── safety-and-governance.md
│   ├── research-roadmap.md
│   ├── development-roadmap.md
│   ├── product-integration.md
│   ├── model-strategy.md
│   ├── model-architecture.md
│   ├── data-strategy.md
│   ├── training-strategy.md
│   ├── evaluation-and-benchmarking.md
│   ├── inference-and-serving.md
│   ├── api-and-sdk-strategy.md
│   ├── infrastructure-strategy.md
│   ├── repository-structure.md
│   └── decisions.md
├── research/
│   └── README.md
└── src/
    └── kryomai/
        └── __init__.py
```

The tree root matches GitHub; the local folder rename is deferred
per [docs/decisions.md](docs/decisions.md) (D2). `src/kryomai/`
is the Python package directory. No source-code modules exist yet
beyond the minimal package initializer.

## Documentation map

- Vision: [docs/vision.md](docs/vision.md)
- Mission and objectives: [docs/mission-and-objectives.md](docs/mission-and-objectives.md)
- Glossary: [docs/glossary.md](docs/glossary.md)
- Architecture: [docs/architecture.md](docs/architecture.md)
- Research principles: [docs/research-principles.md](docs/research-principles.md)
- Safety and governance: [docs/safety-and-governance.md](docs/safety-and-governance.md)
- Research roadmap: [docs/research-roadmap.md](docs/research-roadmap.md)
- Development roadmap: [docs/development-roadmap.md](docs/development-roadmap.md)
- Product integration: [docs/product-integration.md](docs/product-integration.md)
- Repository structure: [docs/repository-structure.md](docs/repository-structure.md)
- Decision log: [docs/decisions.md](docs/decisions.md)
- Model strategy: [docs/model-strategy.md](docs/model-strategy.md)
- Model-architecture research: [docs/model-architecture.md](docs/model-architecture.md)
- Data strategy: [docs/data-strategy.md](docs/data-strategy.md)
- Training strategy: [docs/training-strategy.md](docs/training-strategy.md)
- Evaluation and benchmarking: [docs/evaluation-and-benchmarking.md](docs/evaluation-and-benchmarking.md)
- Inference and serving: [docs/inference-and-serving.md](docs/inference-and-serving.md)
- API and SDK strategy: [docs/api-and-sdk-strategy.md](docs/api-and-sdk-strategy.md)
- Infrastructure strategy: [docs/infrastructure-strategy.md](docs/infrastructure-strategy.md)
- Research organization: [research/README.md](research/README.md)

## Relationship with KryomLabs

KryomLabs is a separate multidisciplinary research platform.
KryomAI Core will provide its intelligence layer through stable,
versioned APIs. No shared code, models, or internal dependencies.
Details: [docs/product-integration.md](docs/product-integration.md).

## License

MIT License. See [LICENSE](LICENSE).
