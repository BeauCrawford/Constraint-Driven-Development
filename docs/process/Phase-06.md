# Phase 06 — Test Generation (Proof Construction)

## Overview

This phase compiles constraints into deterministic, executable tests.
It transforms enforceable rules into mechanical proof artifacts.

No test suite that fails determinism, coverage, or traceability may proceed.

---

## Objective

Generate a complete, deterministic, and traceable test suite from constraints that proves allowed, forbidden, boundary, and failure behavior.

---

## Inputs

- Constraint set with CONSTRAINT_IDs (Phase 04)
- Contract set (Phase 05)
- Canonical glossary

---

## Outputs

- Test suite mapped to CONSTRAINT_IDs
- Positive / Negative / Boundary / Failure tests
- Deterministic execution configuration
- Coverage report (constraint-level)

---

## Mermaid Sequence Diagram

```mermaid
sequenceDiagram
    autonumber
    participant CS as Constraint Set
    participant TS as Test Synthesizer
    participant CT as Contracts
    participant GL as Glossary
    participant RV as Review Gate
    participant SU as Test Suite

    CS->>TS: 1. Load constraints (with IDs)
    TS->>GL: 2. Align terminology
    GL-->>TS: Return canonical mappings
    TS->>CT: 3. Bind to contracts/interfaces
    CT-->>TS: Provide boundary definitions
    TS->>TS: 4. Generate positive tests (allowed behavior)
    TS->>TS: 5. Generate negative tests (forbidden behavior)
    TS->>TS: 6. Generate boundary tests (edge conditions)
    TS->>TS: 7. Generate failure-path tests
    TS->>TS: 8. Map tests to CONSTRAINT_IDs
    TS->>TS: 9. Enforce determinism (no runtime interpretation)
    TS->>TS: 10. Compute constraint-level coverage
    TS->>RV: 11. Submit for review
    RV->>TS: Validate coverage, determinism, mapping
    TS-->>SU: 12. Publish test suite
```

---

## Step Summary Table

| # | Step | What is happening |
|---:|---|---|
| 1 | Load constraints | Use constraints as the source of truth for test generation |
| 2 | Align terminology | Ensure tests use canonical glossary terms |
| 3 | Bind to contracts | Anchor tests to explicit boundaries/interfaces |
| 4 | Generate positive tests | Prove required behavior is satisfied |
| 5 | Generate negative tests | Prove forbidden behavior is rejected |
| 6 | Generate boundary tests | Prove edge conditions behave correctly |
| 7 | Generate failure tests | Prove explicit failure semantics |
| 8 | Map tests to IDs | Ensure each test links to CONSTRAINT_ID(s) |
| 9 | Enforce determinism | Remove non-determinism and runtime interpretation |
| 10 | Compute coverage | Measure semantic coverage over constraints |
| 11 | Review gate | Validate completeness and integrity |
| 12 | Publish suite | Produce authoritative proof artifacts |

---

## Step Sequence

### STEP 01 — Load Constraints
**Tagline:** Establish proof authority

**Description:**  
Use the constraint set (with IDs) as the sole source for test generation.

**Associated Invariants:**  
CDD_CONSTRAINT_UNIQUE_IDENTITY, CDD_CONSTRAINT_ADDRESSABILITY

---

### STEP 02 — Align Terminology
**Tagline:** Maintain semantic consistency

**Description:**  
Ensure all generated tests use glossary-aligned terms.

**Associated Invariants:**  
CDD_GLOSSARY_SHARED_REFERENCE_FRAME

---

### STEP 03 — Bind to Contracts
**Tagline:** Anchor tests at boundaries

**Description:**  
Attach tests to contract interfaces to validate interaction semantics.

**Associated Invariants:**  
CDD_CONTRACT_BOUNDARY_EXTERNALIZATION, CDD_ARCH_BOUNDARY_FIRST

---

### STEP 04 — Generate Positive Tests
**Tagline:** Prove allowed behavior

**Description:**  
Create tests that assert required outcomes for valid inputs and states.

**Associated Invariants:**  
CDD_TEST_POSITIVE_PROOF

---

### STEP 05 — Generate Negative Tests
**Tagline:** Forbid invalid behavior

**Description:**  
Create tests that assert rejection of invalid states and inputs.

**Associated Invariants:**  
CDD_TEST_NEGATIVE_PROOF

---

### STEP 06 — Generate Boundary Tests
**Tagline:** Validate edge conditions

**Description:**  
Create tests around limits, thresholds, and transitions.

**Associated Invariants:**  
CDD_TEST_BOUNDARY_PROOF

---

### STEP 07 — Generate Failure-Path Tests
**Tagline:** Prove failure semantics

**Description:**  
Create tests that assert defined failure modes and responses.

**Associated Invariants:**  
CDD_TEST_FAILURE_PROOF

---

### STEP 08 — Map Tests to CONSTRAINT_IDs
**Tagline:** Ensure traceability

**Description:**  
Link each test to one or more CONSTRAINT_IDs.

**Associated Invariants:**  
CDD_TEST_CONSTRAINT_MAPPING, CDD_TRACEABILITY_CONSTRAINT_TO_TEST

---

### STEP 09 — Enforce Determinism
**Tagline:** Eliminate runtime interpretation

**Description:**  
Ensure tests are stable, reproducible, and free of non-deterministic inputs.

**Associated Invariants:**  
CDD_TEST_RUNTIME_DETERMINISM, CDD_DETERMINISM_REPEATABILITY

---

### STEP 10 — Compute Coverage
**Tagline:** Measure semantic completeness

**Description:**  
Verify all constraints are covered by at least one test.

**Associated Invariants:**  
CDD_COVERAGE_CONSTRAINT_COMPLETE, CDD_COVERAGE_ID_LINKED

---

### STEP 11 — Review Gate
**Tagline:** Enforce proof integrity

**Description:**  
Validate mapping, coverage, determinism, and boundary anchoring.

**Associated Invariants:**  
CDD_GOVERNANCE_ENTRY_EXIT_GATES

---

### STEP 12 — Publish Test Suite
**Tagline:** Establish executable proof

**Description:**  
Release the authoritative, constraint-mapped test suite.

**Associated Invariants:**  
CDD_TEST_NO_ORPHANS, CDD_FOUNDATION_PROOF_BOUND_AUTHORITY

---

## Exit Criteria

- Every constraint has ≥1 mapped test  
- Positive, negative, boundary, and failure cases exist  
- Tests are deterministic and reproducible  
- Tests are bound to contracts (where applicable)  
- Full traceability from CONSTRAINT_ID → TEST  

---

## Final Compression

This phase turns constraints into executable proof,
making correctness mechanically enforceable before any implementation exists.
