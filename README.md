# Contextual Evidence & Explanations (CEE)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/spec-cee/actions/workflows/ci.yml/badge.svg)
[![Check Links](https://github.com/structural-explainability/spec-cee/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/spec-cee/actions/workflows/links.yml)

> Authoritative specification of Contextual Evidence & Explanations (CEE).

## Overview

The Contextual Evidence & Explanations (CEE) specification defines a structured
overlay for attaching interpretive content to neutral structural histories.

CEE records how entities, events, and graph evolutions may be interpreted,
explained, and justified under different contexts, by different actors, and
using different methods.

CEE introduces no new structural facts and asserts
no authority over truth, correctness, or enforcement.

## Purpose

The purpose of CEE is to enable
**accountable, plural explanation**
over shared structural history without embedding interpretation into the substrate itself.

CEE concerns interpretation, responsibility, and provenance only.
It does not define identity, structure, or change.

## Scope

This specification defines:

- contextual scoping of interpretation
- explanation records referencing structural history
- attestations of responsibility for interpretive claims
- provenance describing how explanatory content was produced

This specification does NOT define:

- entity identity rules
- structural relationships or graph evolution
- causal or predictive models
- epistemic validation or truth criteria
- normative judgment or enforcement

## Position in the Stack

CEE operates strictly above the Structural Explainability substrate.

- Structural Explainability (SE) defines admissible representational constraints.
- Accountable Entities (AE) define identity and persistence regimes.
- Evolution Protocol (EP) defines graph evolution over those identities.
- Contextual Evidence & Explanations (CEE) attach interpretation to those histories.

CEE never modifies the substrate.
All references are by stable identifier only.

## Relationship to Other Specifications

- CEE **conforms to** the Structural Explainability specification.
- CEE **operates over** Accountable Entities and Evolution Protocol histories.
- CEE provides interpretive overlays for downstream use.
- No upstream specification depends on CEE.

## Repository Contents

- [SPEC.md](./SPEC.md) - Normative specification
- [IDENTIFIERS.md](./IDENTIFIERS.md) - Stable requirement identifiers
- [CONFORMANCE.md](./CONFORMANCE.md) - Conformance checklist
- [ANNOTATIONS.md](./ANNOTATIONS.md) - Annotation standards
- [LICENSE](./LICENSE) - licensing terms
- [CITATION.cff](./CITATION.cff) - Citation metadata
- [CHANGELOG.md](./CHANGELOG.md) - Version history


## Clarifying Statement

Structural Explainability defines a neutral substrate for identity, structure,
and change.
That substrate records what exists and how it evolves over time
without asserting explanation, interpretation, or judgment.

Contextual Evidence & Explanations operate strictly above this substrate.
CEE does not alter entities, relationships, or graph histories.
Instead, it attaches interpretive content
to references drawn from the substrate.

Context tags, attestations, and provenance are CEE-level constructs.
They scope interpretation, record responsibility for claims,
and document how explanations were produced.
They do not modify, validate, or enforce the
underlying structural record.

This separation ensures that:

- structural history remains stable and neutral,
- multiple, conflicting explanations may coexist over the same history,
- responsibility and method are explicit without collapsing into truth or authority.

Explanation is enabled by the substrate but never embedded within it.
