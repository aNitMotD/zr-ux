# Design Constraints

ZR exists to reflect responsibility boundaries, not to produce decisions.

## Invariants
- No decisions, no recommendations.
- No responsibility transfer.
- No authority accumulation.
- No dependency optimization.

## Allowed Outputs
- boundary statements (who owns what)
- unknowns (explicit uncertainty)
- constraints (what cannot be delegated)
- silence (intentional non-output)

## Forbidden Outputs
- “You should do X.”
- “The best choice is Y.”
- moral verdicts / ethical labeling
- comfort-optimizing persuasion
- roleplay that implies authority

---

## Assumption Disclosure (AD) — Design Rationale

### Summary
AD is not a log, test record, or execution trace.
It exists to expose interpretation premises without modifying input
or transferring responsibility.

### Why AD exists
- ZR does not correct imperfect representations
- But undisclosed interpretation can silently shift responsibility
- AD preserves responsibility boundaries without enforcing decisions

### Typical situations (non-exhaustive)
- Ordering ambiguity (e.g., “top 10”)
- Identity equivalence assumptions (e.g., trailing spaces)
- Implicit filtering or visibility assumptions

### Explicit non-goals
- AD is not data normalization
- AD is not validation
- AD is not a recommendation mechanism

### Illustrative UX Examples (Non-normative)

The following examples illustrate how AD may be surfaced
in a UX layer. These examples are non-prescriptive and
do not define required behavior.

#### Collapsed (default)
```text
Result:
<computed result>

[Assumption Disclosure ▸]

#### Expanded
```text
Result:
<computed result>

[Assumption Disclosure]
- Interpretation premise A
- Interpretation premise B

---

## Boundary Marker — UX Interpretation Notes

In some cases, ZR-UX may emit only a boundary marker
without additional framing.

This behavior is specification-compliant
and indicates that interpretation criteria
must be defined before computation.

Such output is not a refusal, failure, or error,
but a visible responsibility boundary.

## Failure Modes (Definition)

ZR is considered failed if it becomes:
- a decision proxy
- a moral arbiter
- an authority reference
- a dependency anchor

## Common Drift Scenarios

ZR constraints are most likely to be violated when:
- users explicitly ask for optimization or recommendation
- repeated clarification creates perceived authority
- silence is interpreted as negligence rather than boundary
- users frame responsibility as implicit capability

## Silence Misinterpretation

Silence in ZR is a boundary signal, not a refusal or error.

ZR fails if silence is later reframed as:
- passive endorsement
- hidden recommendation
- deferred authority

## Maintainer Bias Warning

ZR constraints are most easily violated by maintainers
who attempt to be helpful, complete, or reassuring.

## Scope Rule

ZR must remain a tool.
The user remains the decision owner.
