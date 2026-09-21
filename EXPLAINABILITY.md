# Explainability Contract: StructureMedic

## Decision

StructureMedic decides whether an unusually large number of files are placed directly in the project root. When the threshold is crossed, it reports a structural organization signal.

## Inputs

It uses the scanned project file list and counts root-level files. The decision is driven by a fixed threshold implemented in the diagnostic rule.

## Limits

It cannot infer the ideal architecture of an arbitrary project. A flat root may be intentional for some repositories, so the finding requires contextual review.
