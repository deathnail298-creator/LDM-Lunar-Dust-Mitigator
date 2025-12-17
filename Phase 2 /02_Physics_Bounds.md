# 02 — Physics Bounds

## Lunar Dust Mitigator (LDM) — Phase 2 (Theory-Only)

> **Phase:** 2 (Theory)
>
> **Scope Rule:** This document defines first-order physical limits that bound what the Lunar Dust Mitigator can and cannot do. These are *non-negotiable* constraints derived from basic physics, not performance targets.

---

## Purpose of This Document

This file answers a single question:

> **What does physics absolutely forbid, regardless of clever design?**

Anything that violates the bounds in this document is not a design problem — it is a physical impossibility and must be discarded.

---

## Reference Assumptions

All reasoning in this document relies only on assumptions defined in:

* `01_System_Assumptions.md`

No new assumptions are introduced here.

---

## Bound 1 — Vacuum Dominance

### Statement

In a lunar vacuum environment:

* There is **no convective transport** of dust
* All dust motion is governed by **ballistics, contact mechanics, or electrostatics**

### Implication

* No airflow-based mitigation logic is available
* Any concept that relies on “redirecting flow” is invalid

**Forbidden:** treating dust like an aerosol

---

## Bound 2 — Momentum Conservation

### Statement

Dust particles possess momentum imparted by:

* rocket exhaust plumes
* wheel-regolith interaction
* human motion

Momentum cannot be destroyed — only redirected or dissipated via contact.

### Implication

* Dust interception requires a surface or field that absorbs or redirects momentum
* “Passive disappearance” of dust is impossible

**Forbidden:** assuming dust can simply be neutralized mid-flight

---

## Bound 3 — Abrasion Is Guaranteed

### Statement

Angular lunar dust interacting with any solid surface will:

* abrade exposed materials
* roughen surfaces over time

This is a certainty, not a failure mode.

### Implication

* Long-term survivability requires tolerance, not prevention
* Polished or precision surfaces are non-viable

**Forbidden:** designs requiring pristine surfaces

---

## Bound 4 — Electrostatics Are Unreliable

### Statement

Electrostatic forces:

* exist in the lunar environment
* vary unpredictably with illumination, charge history, and geometry

### Implication

* Electrostatics may worsen dust adhesion
* They cannot be relied upon for deterministic control

**Forbidden:** electrostatic dust repulsion as a primary mechanism

---

## Bound 5 — Line-of-Sight Dominance

### Statement

In vacuum, dust trajectories are primarily ballistic.

### Implication

* Interception probability depends strongly on geometry and orientation
* Shielding is directional, not omnidirectional

**Forbidden:** assuming area-wide mitigation without physical presence

---

## Bound 6 — Energy Cannot Be Free

### Statement

Any active mitigation requires energy input.

Energy must come from:

* stored power
* harvested power

### Implication

* Continuous active mitigation is power-limited
* Passive mitigation scales better with time

**Forbidden:** infinite or maintenance-free active suppression

---

## Bound 7 — Locality of Effect

### Statement

Dust mitigation effects decay rapidly with distance.

### Implication

* Systems influence a **local interaction zone only**
* Site-wide control is physically unrealistic

**Forbidden:** global or regional dust control claims

---

## Hard Kill Conditions

Any proposed mechanism is **invalid** if it requires:

* atmospheric flow
* precise electrostatic tuning
* perfect material durability
* dust elimination rather than interception
* zero abrasion

These are physics violations, not engineering challenges.

---

## Survivable Design Space (High-Level)

What *does* survive physics bounds:

* sacrificial surfaces
* blunt interception geometries
* tolerance of abrasion
* acceptance of partial effectiveness
* designs that degrade gracefully

This space is narrow but real.

---

## Plain-English Summary

This document defines the physical limits that the Lunar Dust Mitigator cannot violate. It rules out airflow-based, electrostatic-control, and perfect-surface solutions, and establishes that dust mitigation on the Moon is local, abrasive, and geometry-dominated. Anything that contradicts these bounds is physically impossible, not merely hard to engineer.
