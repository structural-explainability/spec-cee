# Contextual Evidence & Explanations Identifiers (CEE)

This document defines the stable requirement identifiers used by the
Contextual Evidence & Explanations (CEE) specification.

Identifiers are the sole normative reference mechanism.
Section ordering, formatting, and presentation are non-normative.

## Overview

Defines interpretive attachments
(context, evidence, explanations, attestations, provenance) operating
over Accountable Entities (AE) and Evolution Protocol (EP) artifacts,
without modifying substrate structure,
under the neutrality constraints of Structural Explainability (SE).

## Identifier Semantics and Ordering

Identifiers are the sole normative reference mechanism.
Section ordering, formatting, and presentation are non-normative.

Identifiers are listed in strict alphabetical order to remove
editorial discretion and ensure deterministic placement.

## Identifier Naming Rules

All identifiers follow this pattern:

CEE.<CATEGORY>.<SUBCATEGORY>.<QUALIFIER>

Identifiers are:

- semantic, not positional
- stable across versions
- reusable across prose, code, and formal proofs
- language-agnostic
- suitable for direct mapping to Lean theorem names

Identifiers MUST NOT be renamed or repurposed.
New identifiers MAY be added only in a new major version of CEE.

## Canonical Identifier List (Alphabetical, with Notes)

CEE.ATTESTATION

Defines records asserting responsibility for an explanation under a given context.

CEE.CONFORMANCE.AE.EP.REQUIRED

States that CEE operates over Accountable Entities and Evolution Protocol artifacts.

CEE.CONFORMANCE.SE.REQUIRED

States that CEE conforms to the Structural Explainability specification.

CEE.CONTEXT.TAG

Defines identifiers for interpretive contexts applied to explanations.

CEE.DEFINITION.CORE

Defines CEE as a framework for attaching interpretive content to substrate history.

CEE.EXPLANATION.RECORD

Defines records associating explanatory content with substrate references.

CEE.MULTIPLICITY

Requires support for multiple, potentially conflicting interpretations.

CEE.PROVENANCE

Defines records describing how explanatory content was produced.

CEE.SCOPE.EXCLUSIONS

Defines what CEE explicitly does not specify.

## Cross-Artifact Consistency Rule

Each identifier in this list MUST appear:

- exactly once in SPEC.md
- exactly once in CONFORMANCE.md
- exactly once as a field in the Lean ConformanceEvidence structure
- exactly once in the Lean requirements list

Alphabetical order SHOULD be preserved across all artifacts.
