# KryomAI Core Decision Log

Append-only record of binding project decisions. Entries are never deleted.
A superseded decision keeps its entry and gains a pointer to its replacement.

Each entry carries an ID, date, status, rationale, and implications.
Statuses: Approved, Pending, Deferred, Superseded.
Decider for all entries below: project owner, approved 2026-11-25,
unless stated otherwise.

## Research scope ratified by D3–D5

Twelve KryomAI Core research domains:

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
    (includes Medicine and Drug Discovery as a research subdomain;
    future independent specialization remains possible)
11. Multimodal scientific intelligence
12. Engineering and new technology development

Cross-cutting capability (not a standalone domain): Agentic Intelligence.

## Active decisions

### D1 — Project identity: KryomAI Core (Approved, 2026-11-25)

Decision: KryomAI Core is the sole official project identity.

Rationale: the GitHub repository was already transferred to the KryomAI
organization and renamed to `kryomai-core`. Keeping prior branding
alongside it caused the identity conflicts found in the
repository audit (brand-vs-hosting mismatch, inverted independence
statements). Dual branding is rejected.

Implications: all Wave 1–3 documentation is written under KryomAI Core.
Retired identities appear nowhere in current files; they survive
only in preserved Git commit history.

Constraint: the LICENSE copyright holder is NOT changed in this phase.
Changing it requires explicit ownership confirmation (see P1).

### D2 — Local folder and Git remote update deferred (Approved, 2026-11-25)

Decision: the local folder rename and the Git remote URL update happen
only after the v0.1.0 documentation is approved.

Rationale: keeps the documentation review diff clean and avoids mixing
identity migration with content review.

Implications: until then, the stale local folder name and old remote URL
are known and accepted. No Git history operations occur without explicit
owner approval.

### D3 — Medicine and Drug Discovery placement (Approved, 2026-11-25)

Decision: Medicine and Drug Discovery is a research subdomain of
Biotechnology and bioinformatics. Future independent specialization
remains possible through a later logged decision.

Rationale: preserves the prior biomedical research intent without
expanding the domain count. Keeps all biomedical work under one
safety-and-governance umbrella for now.

Implications: Wave 1 vision and roadmap documents list it strictly as a
subdomain. Non-clinical boundaries still apply.

### D4 — Agentic Intelligence as cross-cutting capability (Approved, 2026-11-25)

Decision: Agentic Intelligence is treated as a cross-cutting capability,
not a standalone research domain.

Rationale: tool use, multi-step reasoning, and sandbox containment apply
across domains rather than belonging to one.

Implications: documented wherever capabilities cut across domains
(model strategy, evaluation, safety); not given its own domain chapter.

### D5 — New-domain scope confirmed (Approved, 2026-11-25)

Decision: Software Engineering/Coding, Semiconductors, and General
Engineering are in KryomAI Core's research scope.

Rationale: these are intelligence-research directions (reasoning about
code, chips, and engineered systems), not product engineering, and
belong in Core.

Implications: Wave 1 vision and roadmap documents define all three.
Product-specific engineering stays in product repositories per D7.

### D6 — Model-weight licensing deferred (Approved, 2026-11-25)

Decision: model-weight licensing requires a separate future decision
and explicit approval before any weights release.

Rationale: code licensing (MIT) and weight licensing are distinct
questions with distinct consequences. No weights exist, so no premature
commitment is made.

Implications: no model weights are released under any terms until the
future decision is logged here. Code remains MIT unless changed by a
later decision.

### D7 — Repository topology (Approved, 2026-11-25)

Decision: KryomAI Core and individual products live in independent
repositories and integrate only through stable, versioned APIs.

Rationale: preserves Core's leanness, keeps product engineering
independent, and prevents hidden coupling through shared internals.

Implications: Wave 1 product-integration documentation encodes this as
a binding rule. No product code enters this repository.

### D8 — ML framework selection deferred (Approved, 2026-11-25)

Decision: ML framework selection is deferred to the v0.2.0 technical
strategy phase.

Rationale: v0.1.0 is documentation-only on a CPU laptop. Naming a
framework now would be premature commitment without evidence.

Implications: no framework name appears in v0.1.0 documentation.
Training strategy work in v0.2.0 produces the selection.

### D9 — R0–R2 data posture (Approved, 2026-11-25)

Decision: for stages R0–R2, use only public-domain and clearly
open-licensed datasets. Record licenses, provenance, sources, and
usage restrictions for every dataset.

Rationale: eliminates licensing risk during the CPU research phases
and makes every early result safely publishable.

Implications: Wave 1 safety and roadmap documents encode this rule.
Any relaxation requires a later logged decision. Incompatible or
unverifiable licenses block the study.

### D10 — History preservation and CI deferral (Approved, 2026-11-25)

Decision: preserve existing Git history. Defer implementation CI until
code exists; documentation validation may be introduced later. The
empty `.github/` directory is kept as is during this phase.

Rationale: history rewrites on a public repository cost more than they
gain. CI without code has nothing to validate. The `.github/`
directory is inert (Git does not track empty directories) and its
removal is explicitly out of scope for this phase.

Implications: no history-changing Git operations. No CI pipelines in
v0.1.0. `.github/` remains untouched.

### D11 — Python naming: distribution `kryomai`, import `kryomai` (Approved, 2026-11-25)

Decision: the Python distribution name is `kryomai` and the Python
import name is `kryomai`. Installation uses `pip install kryomai`;
code uses `import kryomai`. The source package directory is
`src/kryomai/`. The GitHub repository name remains `kryomai-core`.

Rationale: a single short name for distribution and import keeps
packaging, documentation, and user instructions consistent.
Distribution name and repository name do not need to match.

Implications: README and repository structure document
`src/kryomai/`; packaging configuration resolves `kryomai` under
`src/`. This decision does not authorize publishing to PyPI; a
release needs its own logged decision.

## Documentation-phase constraints (Approved, 2026-11-25)

Binding for Waves 0–3:

- Do not change the LICENSE copyright holder (see P1).
- Do not rename the Python package, modify `pyproject.toml`, change
  `src/`, or implement code.
- Complete only v0.1.0 documentation (Waves 0–3), one wave at a time,
  with owner approval after each wave.
- Do not run Git commit, push, reset, or other history-changing
  operations without explicit owner approval.
- Do not begin model implementation, dataset creation, training, or
  API development.

## Pending items

### P1 — LICENSE holder ownership confirmation (Pending)

Question: who is the legal copyright holder to name in LICENSE
(KryomAI entity, individual, or contributors collective)?

Blocks: LICENSE holder update and any ownership wording in new docs.
Until resolved, new documentation avoids asserting ownership and the
existing LICENSE text stays byte-identical.
