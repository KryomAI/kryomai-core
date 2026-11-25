# KryomAI Core Infrastructure Strategy

What runs where, now and later. No infrastructure beyond the
current workstation exists or is committed.

## Current envelope (R0–R2)

- Intel i5 laptop, 16 GB RAM, 512 GB SSD, Windows 11.
- Python-first, CPU-only research. R0–R2 budgets must fit
  inside this envelope.
- This machine is a legitimate R0–R2 workstation and nothing
  more. Frontier-scale foundation-model pretraining is not
  feasible on it and is never scheduled on it.

## R3: first GPU access

- Trigger: a proposal's declared budget exceeds the R2 CPU
  envelope and its R2 exit criteria are met.
- Access shape (rental vs owned) is decided per proposal with
  cost review. No standing commitment, no vendor named here.
- GPU work inherits all R2 reproducibility rules plus
  accelerator identity logging.

## R4: serving footprint

- Trigger: a component meets R4 stable-interface exit criteria.
- Footprint starts minimal: one versioned endpoint family with
  rollback, monitoring, and declared budgets.
- Growth follows measured product demand, not forecasts.

## R5: distributed scale

- Trigger: a scale-up program with its own infrastructure and
  budget approval, logged as a decision.
- Distributed training, large data pipelines, and multi-node
  serving live here or not at all.
- No R5 planning begins before R4 exit.

## Principles

- Smallest sufficient footprint at every stage.
- Measured triggers graduate work; forecasts do not.
- Cost and energy budgets are declared alongside compute
  budgets from R3 on.
- No vendor, platform, or cloud commitments in this document.
