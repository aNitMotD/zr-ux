# ZR-UX Removal Decision

## Status
Archived. No active development.

## Summary
ZR-UX was removed after design validation.

The goal of ZR-UX was to make ZR outputs more readable or user-friendly
through a UX or rendering layer.

## Reason for Removal
Experiments showed that any UX layer placed after ZR output
inevitably introduces semantic interpretation, even when strictly constrained.

This includes:
- restatement or paraphrasing
- perspective framing ("from a ZR-UX point of view")
- implicit responsibility attribution
- closure, guidance, or next-step signaling

These effects directly conflict with ZR’s core properties:
- non-judgment
- non-attribution
- responsibility boundary preservation
- boundary-based stopping

The issue was not insufficient constraints or wording,
but the existence of a post-analysis UX layer itself.

## Conclusion
ZR-UX was removed entirely.

Zero Reflect (ZR) is maintained as a standalone system.
ZR outputs are produced as-is, without any UX, rendering,
formatting, or post-processing layers.

This repository is intentionally preserved as a record
of that design decision.
