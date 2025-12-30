# Conformance Checklist

This document defines the criteria for determining whether an artifact
conforms to the Contextual Evidence & Explanations specification.

Identifiers referenced in this document are the sole normative reference.
Ordering and formatting are non-normative.

An artifact may be a specification, schema, implementation, repository,
or other deliverable claiming conformance.

## Conformance Overview

An artifact CONFORMS if and only if:

- all mandatory requirements are satisfied
- no prohibited assertions are present
- conformance with Structural Explainability (SE),
  Accountable Entities (AE), and Evolution Protocol (EP) is preserved

CEE conformance is additive and overlay-only.
CEE MUST NOT modify or reinterpret substrate records.

Failure of any single check constitutes non-conformance.

CEE.ATTESTATION

- [ ] Attestations reference explanation records and context tags.
- [ ] Attestations identify asserting actors and scope of claim.
- [ ] Attestations do not certify correctness or authority.
- Fail if: attestations are treated as validation, certification, or enforcement.

CEE.CONFORMANCE.AE.EP.REQUIRED

- [ ] All references to entities, events, or histories resolve to AE and EP identifiers.
- [ ] No AE identity regime or EP graph rule is redefined or overridden.
- Fail if: identity, structure, or graph evolution is altered by CEE artifacts.

CEE.CONFORMANCE.SE.REQUIRED

- [ ] The artifact explicitly claims conformance with Structural Explainability.
- [ ] No CEE construct weakens or bypasses SE neutrality constraints.
- Fail if: epistemic, causal, or normative commitments are embedded as substrate facts.

CEE.CONTEXT.TAG

- [ ] Context tags are external to substrate records.
- [ ] Context tags scope interpretation only.
- [ ] Context tags may coexist, overlap, or conflict.
- Fail if: context tags modify or reinterpret substrate structure.

CEE.DEFINITION.CORE

- [ ] The artifact treats CEE as an interpretive overlay.
- [ ] Interpretive content is attached only via references to substrate artifacts.
- Fail if: CEE is treated as a structural, operational, or authoritative layer.

CEE.EXPLANATION.RECORD

- [ ] Explanation records reference substrate identifiers.
- [ ] Explanation records do not assert structural change.
- [ ] Multiple explanation records may reference the same substrate history.
- Fail if: explanations alter, replace, or overwrite substrate records.

CEE.MULTIPLICITY

- [ ] Multiple explanations, attestations, and provenance chains are supported.
- [ ] Conflicting interpretations may coexist without forced resolution.
- Fail if: reconciliation, prioritization, or resolution is required for conformance.

CEE.PROVENANCE

- [ ] Provenance records describe derivation of CEE-level artifacts only.
- [ ] Provenance does not revise or reinterpret substrate history.
- Fail if: provenance is applied to substrate events, identities, or graph evolution.

CEE.SCOPE.EXCLUSIONS

Verify that the artifact does not define:

- [ ] substrate identity rules
- [ ] graph validity or evolution rules
- [ ] causal or predictive models
- [ ] epistemic validation or truth criteria
- [ ] normative judgment or enforcement

Presence of any of the above constitutes non-conformance.

## Final Determination

An artifact CONFORMS if:

- all checks above pass, and
- no prohibited assertions are present.

Otherwise, the artifact is NON-CONFORMANT.

## Conformance Declaration

Artifacts claiming conformance SHOULD include a declaration of the form:

```text
Conforms to: CEE Specification vx.y
Conforms to: EP Specification vx.y
Conforms to: AE Specification vx.y
Conforms to: SE Specification vx.y
```
