# StructureMedic

> Portable agent for identifying repositories with excessive root-level file accumulation.

## What it does

StructureMedic examines the project tree and flags cases where many files live directly in the repository root. It recommends grouping related concerns into directories when the layout becomes difficult to navigate.

### Diagnostic fingerprint

**File distribution → organization signal → evidence → restructuring plan**

## Why this agent is distinct

StructureMedic evaluates organization rather than code correctness. A project can compile perfectly and still become difficult to navigate as the root grows.

Its rule provides a simple, reproducible signal for that problem.

## Workflow

```text
Project tree
    ↓
Path distribution analysis
    ↓
Structure rule
    ↓
Evidence
    ↓
Organization recommendation
```

## Verification

The repository contains an OpenGAP passport, a structure-focused fixture, explainability contracts, four framework adapters, and automated adapter tests.

OpenGAP validation passed and all four generated framework exports have been exercised successfully.

## Design principle

**Structure is a usability layer.** StructureMedic bases its recommendation on measurable file placement rather than subjective claims about style.

## Medic family

StructureMedic is the project-organization specialist in the Medic family.