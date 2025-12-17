# 02 — Dependency and Coupling Map

## Lunar Dust Mitigator (LDM) — Phase 3 (Theory-Only)

> **Phase:** 3 (Theory)
>
> **Scope Rule:** This document maps logical dependencies and couplings between subsystems and assumptions. It does not define designs, interfaces, or execution plans.

---

## Purpose of This Document

This file answers:

> **What depends on what, and where hidden couplings could quietly break the system during execution?**

Dependencies are treated as risk multipliers. Couplings are treated as failure accelerants.

---

## Reference Baseline

All dependencies and couplings identified here:

* are consistent with Phase 2 conclusions
* reference unknowns defined in `01_Unknowns_Registry.md`
* introduce no new assumptions

---

## Dependency Types

* **Hard Dependency:** If X fails, Y cannot function at all
* **Soft Dependency:** If X degrades, Y degrades but remains partially useful
* **Assumed Independence:** No meaningful interaction exists

---

## Core Dependency Map

### D1 — Geometry → Throughput

* **Type:** Hard Dependency
* **Description:**
  Effective dust interception depends directly on exposed geometry and orientation.
* **Failure Effect:**
  Loss or distortion of geometry immediately reduces throughput.

---

### D2 — Geometry → Thermal Behavior

* **Type:** Hard Dependency
* **Description:**
  Radiative heat rejection depends on geometric openness and sky view.
* **Failure Effect:**
  Poor geometry can induce thermal runaway (Phase 2 kill condition).

---

### D3 — Accumulation → Geometry

* **Type:** Soft Dependency
* **Description:**
  Dust buildup alters effective geometry over time.
* **Failure Effect:**
  Gradual throughput degradation; rarely catastrophic.

---

### D4 — Power Availability → Active Elements

* **Type:** Hard Dependency (localized)
* **Description:**
  Any active behavior depends on intermittent power availability.
* **Failure Effect:**
  Active features cease; passive system remains.

---

### D5 — Thermal Cycling → Structural Integrity

* **Type:** Soft Dependency
* **Description:**
  Repeated thermal swings stress structure and joints.
* **Failure Effect:**
  Gradual mechanical degradation.

---

## Cross-Domain Couplings

### C1 — Accumulation ↔ Thermal

* **Coupling Type:** Soft
* **Description:**
  Dust accumulation alters radiative properties, affecting thermal behavior.
* **Risk Note:**
  Nonlinear; listed as U-04 in unknowns registry.

---

### C2 — Geometry ↔ Adjacent Systems

* **Coupling Type:** Soft
* **Description:**
  Redirected dust may increase exposure elsewhere.
* **Risk Note:**
  Integration-dependent; listed as U-06.

---

### C3 — Partial Burial ↔ Orientation

* **Coupling Type:** Hard
* **Description:**
  Burial alters effective orientation and interception logic.
* **Risk Note:**
  Binary survivability; listed as U-05.

---

## Forbidden Couplings

The following couplings are explicitly disallowed:

* geometry → required external power
* thermal control → adjacent hardware
* throughput → continuous coordination
* survivability → human intervention

Any appearance of these couplings invalidates Phase 3 discipline.

---

## Dependency Collapse Scenarios

Examples of cascading failures:

* Geometry distortion → thermal imbalance → structural failure
* Accumulation saturation → geometry loss → throughput collapse

These cascades are slow and observable, enabling early termination.

---

## Phase 3 Conclusion (Dependencies)

The Lunar Dust Mitigator exhibits:

* few hard dependencies
* many soft, degradable interactions
* limited but identifiable couplings

This structure favors failure tolerance and early risk detection.

---

## Plain-English Summary

This document maps how different parts of the Lunar Dust Mitigator depend on one another and where interactions could cause problems during execution. Most dependencies are soft and degrade performance gradually rather than catastrophically. Only a small number of hard couplings pose existential risk, and these are explicitly identified.
