# ZR-UX Operator Judgment Spec

This document defines judgment considerations for operators.
It does not prescribe system behavior.
It does not override or modify the ZR-UX Operation Spec.

This spec exists to guide human or supervisory judgment
in cases where strict application of the Operation Spec
produces degraded UX outcomes.

All final responsibility remains with the operator.

---

---

## Reference Relationship to Other Specifications

This document is subordinate to the ZR-UX Operation Spec.

- In case of conflict, the ZR-UX Operation Spec always takes precedence.
- This document must never be used to override explicit boundaries,
  forbidden domains, or responsibility constraints defined elsewhere.
- This document does not introduce new capabilities,
  permissions, or behaviors.

The sole purpose of this spec is to support operator judgment
in cases where the Operation Spec permits multiple valid responses
and UX degradation has been observed in practice.

This document must be read as a companion reference,
not as an extension or modification of the Operation Spec.

---

## 1. Scope and Intent

This spec applies only to judgment moments
where the ZR-UX Operation Spec allows multiple valid responses.

It must not be used to bypass explicit boundaries,
forbidden domains, or responsibility constraints
defined in the Operation Spec.

---

## 2. Judgment Activation Conditions

Operator judgment may be consulted when:

- The input does not explicitly request advice, evaluation, or judgment
- The input is ambiguous in intent or framing
- The system response would otherwise default to a boundary
- The boundary is not triggered by a forbidden domain

---

## 3. Reaction Level Misclassification Risk

Certain prompt shapes may appear analytical
while originating from low reaction contexts.

Examples include:
- “Can you break this down?”
- “How should I organize this?”
- “Can you help me structure this?”

These prompts may indicate confusion
or lack of an initial framing coordinate,
not readiness for structural decomposition.

---

## 4. Artifact Presence Consideration

The presence of an input artifact
indicates the existence of an object,
not the user's readiness to reason about it structurally.

Artifact presence alone must not be treated
as escalation of reaction level.

---

## 5. Boundary vs Framing Decision

Before emitting a boundary in ambiguous cases,
operators should consider whether a minimal framing response
could allow the user to clarify intent.

A framing response:

- Does not perform analysis
- Does not provide recommendations
- Does not assume responsibility
- Returns agency immediately to the user

---

## 6. Minimal Framing Examples (Non-prescriptive)

Examples of framing scaffolds include:

- Asking which aspect feels unclear
- Asking what the user is trying to understand
- Asking whether the goal is clarification or grouping

These examples are illustrative only
and must not be treated as templates.

---

## 7. Boundary Stability Consideration

Repeated prompts with unchanged input
do not necessarily indicate increased readiness
or implicit permission to proceed.

Repetition alone should not be used
to relax responsibility boundaries.

---

## 8. Invalid Use of This Spec

This spec must not be used to:

- Override explicit forbidden boundaries
- Justify advice or decision-making
- Convert judgment considerations into automated rules
- Backfill post-hoc rationales for boundary violations

---

## 9. Evaluation Criterion

If applying this judgment spec
does not materially reduce premature boundary emission
for low reaction contexts,
the UX layer should be considered ineffective.

---

## Closing Statement

This document exists to support judgment,
not to replace it.

If judgment cannot be exercised reliably,
the UX layer should be removed.

---

This spec is informed by repeated UX degradation
observed during test operation.

Concrete observations are recorded separately
and are not normative.
