# Phase 11 — Change & Recompilation

## Overview

This phase governs system evolution by forcing change to originate upstream and propagate through re-lowering.
CDD treats patching downstream artifacts as a source of drift unless upstream intent is updated first.

No stale artifact may survive upstream change.

---

## Objective

Apply change through requirements or invariants, regenerate downstream artifacts, and revalidate closure, coverage, proof, and implementation conformance.

---

## Inputs

- Change request or updated intent
- Existing requirement, invariant, constraint, test, and code artifacts
- Traceability and coverage reports
- Canonical glossary

---

## Outputs

- Updated upstream artifacts
- Regenerated downstream artifacts
- Drift resolution report
- Revalidation evidence

---

## Mermaid Sequence Diagram

```mermaid
sequenceDiagram
    autonumber
    actor CH as Change Source
    participant UP as Upstream Intent Layer
    participant LG as Lowering Pipeline
    participant RV as Revalidation Gate
    participant DS as Downstream Artifacts
    participant CR as Change Report

    CH->>UP: 1. Submit change request
    UP->>UP: 2. Classify upstream impact
    UP->>UP: 3. Update requirement or invariant source
    UP->>LG: 4. Re-lower affected artifacts
    LG->>DS: 5. Regenerate constraints, tests, and code
    DS->>RV: 6. Submit regenerated artifacts
    RV->>RV: 7. Revalidate closure and coverage
    RV->>RV: 8. Detect stale artifacts and drift
    RV-->>CR: 9. Publish change report
```

---

## Step Summary Table

| # | Step | What is happening |
|---:|---|---|
| 1 | Submit change | Capture requested evolution |
| 2 | Classify impact | Identify upstream source and affected paths |
| 3 | Update upstream | Change requirements or invariants first |
| 4 | Re-lower artifacts | Propagate through the CDD pipeline |
| 5 | Regenerate downstream | Recreate constraints, tests, and code |
| 6 | Submit artifacts | Move regenerated outputs to review |
| 7 | Revalidate | Confirm closure and coverage |
| 8 | Detect stale artifacts | Remove drift and obsolete outputs |
| 9 | Publish report | Record change integrity |

---

## Step Sequence

### STEP 01 — Submit Change Request
**Tagline:** Capture evolution

**Description:**  
Record the desired change before altering downstream artifacts.

**Associated Invariants:**  
CDD_CHANGE_UPSTREAM_INITIATION

---

### STEP 02 — Classify Impact
**Tagline:** Find the source layer

**Description:**  
Determine whether the change belongs in requirements, invariants, glossary, or another upstream artifact.

**Associated Invariants:**  
CDD_TRACEABILITY_REVERSE_NAVIGATION

---

### STEP 03 — Update Upstream Source
**Tagline:** Change authority first

**Description:**  
Apply the change at the governing semantic layer.

**Associated Invariants:**  
CDD_FOUNDATION_INTENT_PRECEDENCE, CDD_CHANGE_UPSTREAM_INITIATION

---

### STEP 04 — Re-Lower Affected Artifacts
**Tagline:** Propagate meaning

**Description:**  
Derive downstream artifacts again instead of patching them manually.

**Associated Invariants:**  
CDD_LOWERING_RECOMPILATION_OVER_PATCHING, CDD_CHANGE_DOWNSTREAM_RECOMPILATION

---

### STEP 05 — Regenerate Constraints, Tests, and Code
**Tagline:** Refresh proof chain

**Description:**  
Regenerate affected executable rules, proofs, and implementation.

**Associated Invariants:**  
CDD_TEST_REGENERABILITY, CDD_CHANGE_TEST_REGENERATION

---

### STEP 06 — Submit Regenerated Artifacts
**Tagline:** Re-enter governance

**Description:**  
Move regenerated outputs through review gates.

**Associated Invariants:**  
CDD_GOVERNANCE_ENTRY_EXIT_GATES

---

### STEP 07 — Revalidate Closure and Coverage
**Tagline:** Confirm containment

**Description:**  
Ensure the updated system remains semantically closed and fully covered.

**Associated Invariants:**  
CDD_CLOSURE_REVALIDATION_REQUIRED, CDD_COVERAGE_REVALIDATION

---

### STEP 08 — Detect Stale Artifacts and Drift
**Tagline:** Remove divergence

**Description:**  
Identify obsolete artifacts or semantic drift introduced by the change.

**Associated Invariants:**  
CDD_CHANGE_NO_SILENT_DIVERGENCE, CDD_CHANGE_DRIFT_DETECTION

---

### STEP 09 — Publish Change Report
**Tagline:** Record evolution

**Description:**  
Document what changed, what was regenerated, and what evidence proves integrity.

**Associated Invariants:**  
CDD_GOVERNANCE_EVIDENCE_REQUIRED

---

## Exit Criteria

- Change originates upstream  
- Downstream artifacts are regenerated, not patched  
- Closure and coverage are revalidated  
- No stale artifacts remain  
- Drift is eliminated  

---

## Final Compression

This phase keeps evolution inside the constraint system,
ensuring change flows through authority instead of bypassing it.
