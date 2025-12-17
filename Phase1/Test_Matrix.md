# LDM — Phase 1 Test Matrix

## Purpose of This Document

This document defines the **finite set of tests** performed during Phase 1 evaluation of the Lunar Dust Mitigation (LDM) concept.

The Phase 1 test matrix is intentionally small.  
It exists to validate core assumptions, not to explore every configuration.

Any test not listed here is **out of scope** for Phase 1.

---

## Test Matrix Philosophy

Phase 1 testing follows these rules:

- Each test has a clear purpose
- Each test has a measurable pass/fail outcome
- Each test maps directly to a Phase 1 success criterion
- No test is exploratory unless explicitly marked

Adding tests after execution begins is not permitted.

---

## Baseline Tests

### T-0 — Baseline Dust Behavior (No LDM)

**Purpose:**  
Establish baseline dust concentration and deposition without LDM influence.

- LDM active: No
- Environment: Nominal Phase 1 test environment
- Dust introduction: Standardized
- Measurements:
  - Airborne dust concentration (if applicable)
  - Dust deposition on witness surfaces

**Outcome:**  
Baseline reference for all subsequent tests.

---

## Core Functional Tests

### T-1 — LDM Active, Nominal Conditions

**Purpose:**  
Evaluate dust interaction under nominal conditions.

- LDM active: Yes
- Configuration: Nominal geometry
- Environment: Same as T-0
- Measurements:
  - Airborne dust concentration change
  - Dust deposition rate change
  - Qualitative flow observation

**Success Criteria:**  
SC-1.1, SC-1.2

---

### T-2 — Repeatability Test (Run 2)

**Purpose:**  
Validate repeatability of observed dust effects.

- LDM active: Yes
- Configuration: Identical to T-1
- Environment: Identical to T-1
- Measurements: Same as T-1

**Success Criteria:**  
SC-2.1

---

### T-3 — Repeatability Test (Run 3)

**Purpose:**  
Confirm consistency across multiple runs.

- LDM active: Yes
- Configuration: Identical to T-1
- Environment: Identical to T-1
- Measurements: Same as T-1

**Success Criteria:**  
SC-2.1

---

## Power and Thermal Tests

### T-4 — Power Envelope Verification

**Purpose:**  
Confirm operation within predefined Phase 1 power bounds.

- LDM active: Yes
- Configuration: Nominal
- Duration: Representative operating period
- Measurements:
  - Peak power draw
  - Average power draw

**Success Criteria:**  
SC-3.1

---

### T-5 — Thermal Stability Observation

**Purpose:**  
Identify thermal behavior during operation.

- LDM active: Yes
- Configuration: Nominal
- Duration: Representative operating period
- Measurements:
  - Temperature at defined locations
  - Visual inspection post-test

**Success Criteria:**  
SC-3.2

---

## Mechanical Survivability Tests

### T-6 — Multi-Run Mechanical Integrity

**Purpose:**  
Verify absence of irreversible mechanical failure across testing.

- LDM active: Yes
- Configuration: Nominal
- Runs: All Phase 1 test runs combined
- Observations:
  - Geometry retention
  - Clogging or fouling behavior
  - Structural integrity

**Success Criteria:**  
SC-4.1

---

## Test Matrix Summary Table

| Test ID | Description | Primary Criteria |
|------|------------|------------------|
| T-0 | Baseline (no LDM) | Reference only |
| T-1 | Nominal LDM operation | SC-1.1, SC-1.2 |
| T-2 | Repeatability run 2 | SC-2.1 |
| T-3 | Repeatability run 3 | SC-2.1 |
| T-4 | Power envelope | SC-3.1 |
| T-5 | Thermal stability | SC-3.2 |
| T-6 | Mechanical survivability | SC-4.1 |

---

## Test Completion Rules

- Tests are executed in numerical order
- Any Phase 1 kill criterion immediately terminates remaining tests
- Failed tests are not rerun without documented configuration changes

---

## Explicit Exclusions

The Phase 1 test matrix does **not** include:

- Environmental stress testing
- Long-duration endurance testing
- Configuration optimization
- Scaling or array testing
- Integration testing

These are deferred to future phases, if any.

---

## Summary

The Phase 1 LDM test matrix is **finite and complete**.

Completion of this matrix constitutes completion of Phase 1 testing.

Nothing beyond this matrix is implied or required.
