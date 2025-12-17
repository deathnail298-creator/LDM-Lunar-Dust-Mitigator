# 03 — Kill Criteria Definition

## Lunar Dust Mitigator (LDM) — Phase 3 (Theory-Only)

> **Phase:** 3 (Theory)
>
> **Scope Rule:** This document defines explicit conditions under which execution must be halted. Kill criteria are framed to minimize sunk-cost bias and prevent continuation of non-viable paths.

---

## Purpose of This Document

This file answers:

> **Under what conditions should execution be stopped immediately, even if effort or resources have already been invested?**

Kill criteria are not pessimistic; they are discipline.

---

## Reference Baseline

All kill criteria:

* are consistent with Phase 2 conclusions
* reference unknowns defined in `01_Unknowns_Registry.md`
* reference dependencies defined in `02_Dependency_and_Coupling_Map.md`
* introduce no new assumptions

---

## Kill-Criteria Philosophy

* Early termination is preferable to prolonged failure
* Binary decisions beat ambiguous continuation
* Emotional or reputational factors are irrelevant

If a criterion is met, execution stops.

---

## Category A — Physics Violations

Execution must terminate if any of the following are observed:

### K-A1 — Non-Local Dust Control Required

* Observation that mitigation must affect area-wide dust to be useful

### K-A2 — Continuous Active Power Required

* Observation that passive or intermittent operation is insufficient

### K-A3 — Electrostatic Control Required

* Observation that reliable function depends on active electrostatic manipulation

These indicate violation of Phase 2 physics bounds.

---

## Category B — Thermal Non-Viability

Execution must terminate if:

### K-B1 — Thermal Runaway Is Intrinsic

* Viable geometries cannot reject heat without active cooling

### K-B2 — Thermal Cycling Causes Rapid Structural Failure

* Degradation occurs on timescales too short for usefulness

These indicate thermal infeasibility.

---

## Category C — Mechanical or Dust Behavior Failures

Execution must terminate if:

### K-C1 — Accumulation Causes Immediate Loss of Function

* Dust buildup renders system ineffective before meaningful benefit

### K-C2 — Abrasion Destroys Geometry Rapidly

* Surfaces degrade faster than mitigation value accrues

These indicate unacceptable degradation rates.

---

## Category D — Integration Hazards

Execution must terminate if:

### K-D1 — Secondary Dust Hazards Are Created

* Redirected dust increases risk to critical hardware

### K-D2 — Structural or Thermal Coupling Is Required

* Safe operation depends on integration with other systems

These indicate unacceptable interface risk.

---

## Category E — Scalability Collapse

Execution must terminate if:

### K-E1 — Single-Unit Behavior Does Not Generalize

* Scaling introduces new failure modes not present in isolation

### K-E2 — Deployment Density Becomes Critical

* Precise placement or coordination is required for usefulness

These indicate scaling non-viability.

---

## Decision Enforcement

* Meeting any single kill criterion is sufficient to stop execution
* No compensating improvements override a kill condition
* Restart requires returning to Phase 2 or Phase 3 analysis

---

## Phase 3 Conclusion (Kill Criteria)

These kill criteria:

* protect against optimism drift
* preserve program credibility
* enable early, defensible termination

They are an explicit contract with reality.

---

## Plain-English Summary

This document defines clear conditions under which work on the Lunar Dust Mitigator must stop. If the system violates basic physics assumptions, proves thermally or mechanically non-viable, creates integration hazards, or fails to scale without tight coordination, execution should be terminated immediately. These criteria exist to prevent wasted effort and sunk-cost bias.
