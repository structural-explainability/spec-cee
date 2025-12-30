# Contextual Evidence & Explanations Specification (CEE)

Status: Normative

This document defines the normative requirements for conformance with
Contextual Evidence & Explanations (CEE).

CEE is a downstream specification that operates over the
Structural Explainability (SE) substrate, including Accountable Entities (AE)
and Evolution Protocol (EP).

It introduces no new structural facts.
It attaches interpretive content to references drawn from the substrate.

## How to Read This Spec

Keywords MUST, MUST NOT, SHOULD, and MAY
are to be interpreted as described in RFC 2119.

Use of terms such as "canonical" denotes structural role only and
does not imply epistemic, causal, or normative preference.

This specification does not prescribe editorial structure,
terminology preference, or documentation layout beyond identifier semantics.

## Representation vs Constraint Classes

Some requirements describe what the substrate MAY represent,
while others constrain how such representations MUST NOT be interpreted.

Overlap between these classes is intentional:
representation permissions do not imply explanatory commitment.

## Identifier Semantics and Stability

Each requirement in this document is identified by a stable identifier
of the form `CEE.*`.

Identifiers are the sole normative reference for conformance.
Textual wording MAY be clarified over time without changing meaning;
any change that alters the requirement MUST result in a new identifier.

Renaming, reordering, or relocating identifiers constitutes a semantic
change and is therefore intentionally diff-visible.

Repository paths, filenames, and section ordering are non-normative and
do not affect identifier meaning.

---

## CEE.CONFORMANCE.SE.REQUIRED

Any system claiming conformance with Contextual Evidence & Explanations MUST
also conform to the Structural Explainability Specification.

CEE MUST NOT weaken or override SE neutrality constraints.

## CEE.CONFORMANCE.AE.EP.REQUIRED

CEE MUST reference entities, events, and histories defined by AE and EP.
CEE MUST NOT redefine identity, structure, or graph evolution.

CEE operates only over stable substrate identifiers.

## CEE.DEFINITION.CORE

Contextual Evidence & Explanations define a framework for attaching
interpretive content to structural histories recorded on the
Structural Explainability substrate.

CEE specifies:

- contextual scoping of interpretation
- evidentiary grouping and reference
- explanation records
- attestation of responsibility
- provenance of explanatory content

CEE does not specify truth, correctness, or enforcement.

## CEE.CONTEXT.TAG

A Context Tag identifies an interpretive context under which an explanation
is offered.

Context Tags:

- scope explanatory content
- identify frameworks, assumptions, or viewpoints
- are external to the substrate

Context Tags MUST NOT modify or reinterpret substrate records.
Context Tags MAY overlap, conflict, or evolve over time.

## CEE.EXPLANATION.RECORD

An Explanation Record associates interpretive content with references to
substrate entities, events, or graph histories.

Explanation Records:

- reference substrate identifiers
- do not assert structural change
- do not modify substrate state

Multiple Explanation Records MAY refer to the same substrate history.

## CEE.ATTESTATION

An Attestation records that an accountable actor asserts responsibility for
an explanation under a specified context.

Attestations:

- reference Explanation Records and Context Tags
- identify the asserting actor and scope of claim
- do not certify correctness or authority

Attestations MUST NOT alter or validate substrate records.

## CEE.PROVENANCE

Provenance records describe how an explanation, context assignment, or
attestation was produced.

Provenance MAY include:

- source materials
- methods or processes used
- tools or models involved
- derivation history of explanatory content

Provenance applies to CEE-level artifacts only.
Provenance MUST NOT be used to reinterpret or revise substrate history.

## CEE.MULTIPLICITY

CEE MUST support multiple explanations, attestations, and provenance chains
over the same substrate history.

CEE MUST NOT require reconciliation, prioritization, or resolution of
conflicting interpretations.

Disagreement is representable, not eliminable.

## CEE.SCOPE.EXCLUSIONS

This does not define:

- substrate identity rules
- graph validity or evolution rules
- causal or predictive models
- epistemic validation or truth criteria
- normative judgment or enforcement

These concerns are explicitly out of scope.
