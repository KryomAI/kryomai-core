# KryomAI Core API and SDK Strategy

Design principles for future interfaces. No API or SDK exists;
no endpoint is promised. Principles first, so the first
interface inherits them.

## Versioning and stability

- Semantic versioning for every interface. Breaking changes
  only in major versions with a published deprecation window.
- Experimental surfaces are labeled experimental and carry no
  stability promise.

## Endpoint families (planned)

- Inference: versioned model invocation with model identity
  in every response.
- Evaluation: harness runs and benchmark queries for
  reproducibility checks.
- Metadata: dataset cards, model records, and changelog feeds.
Families, not endpoints. Concrete routes arrive with R4
proposals.

## SDK principles

- Python-first, matching the research stack.
- Thin over the API: no hidden behavior beyond documented
  retries and error mapping.
- Versioned in lockstep with the API it targets.

## Access posture

- Authentication, rate limits, and audit logging are required
  before any shared or product endpoint goes live.
- Local research endpoints stay unauthenticated by design and
  never leave the workstation.

## KryomLabs consumption contract

- KryomLabs and products consume released versions only.
- Core publishes machine-readable interface definitions with
  every release.
- Support windows are declared per major version.
