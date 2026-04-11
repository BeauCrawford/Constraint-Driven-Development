# Phase 02 — Invariant Extraction

## Overview

This phase converts structured requirements into irreducible semantic truths (invariants).  
It is the compression layer where intent becomes governable.

No invariant set that fails this phase may proceed.

---

## Objective

Transform normalized requirements into minimal, non-redundant, implementation-independent invariants that fully preserve intent.

---

## Inputs

- Stable requirement set (Phase 01 output)
- Canonical glossary

---

## Outputs

- Invariant set
- Invariant-to-requirement mappings
- Conflict resolution artifacts
- Negative-space definitions

---

## Mermaid Sequence Diagram

```mermaid
sequenceDiagram
    autonumber
    participant RF as Requirement Set
    participant IE as Invariant Extraction Layer
    participant GL as Glossary
    participant RV as Review Gate
    participant IV as Invariant Set

    RF->>IE: 1. Load normalized requirements
    IE->>GL: 2. Resolve domain terminology
    GL-->>IE: Return canonical terms
    IE->>IE: 3. Decompose requirements into semantic units
    IE->>IE: 4. Extract invariant candidates
    IE->>IE: 5. Remove redundancy and overlap
    IE->>IE: 6. Validate minimality and necessity
    IE->>IE: 7. Define negative space (forbidden states)
    IE->>IE: 8. Detect and resolve invariant conflicts
    IE->>RV: 9. Submit invariants for review
    RV->>IE: Validate coverage, independence, clarity
    IE->>IE: 10. Finalize invariant set
    IE-->>IV: 11. Publish invariant set
```

---

## Step Summary Table

| # | Step | What is happening |
|---:|---|---|
| 1 | Load requirements | Bring in stable, normalized requirements from Phase 01 |
| 2 | Resolve terminology | Ensure all semantics align with glossary |
| 3 | Decompose requirements | Break into atomic semantic units |
| 4 | Extract invariants | Convert units into irreducible truths |
| 5 | Remove redundancy | Eliminate duplicate or overlapping invariants |
| 6 | Validate minimality | Ensure each invariant is necessary and sufficient |
| 7 | Define negative space | Capture forbidden or invalid states |
| 8 | Resolve conflicts | Eliminate contradictions |
| 9 | Review gate | Validate completeness and correctness |
| 10 | Finalize invariants | Lock invariant set |
| 11 | Publish invariants | Output authoritative invariant layer |

---

## Step Sequence

### STEP 01 — Load Requirements  
**Tagline:** Establish semantic input  

**Description:**  
Load stable requirements from Phase 01.

**Associated Invariants:**  
CDD_TRACEABILITY_REQUIREMENT_TO_INVARIANT  

---

### STEP 02 — Resolve Terminology  
**Tagline:** Align semantic language  

**Description:**  
Ensure all terms match glossary definitions.

**Associated Invariants:**  
CDD_GLOSSARY_CANONICAL_VOCABULARY  

---

### STEP 03 — Decompose Requirements  
**Tagline:** Break intent into atomic meaning  

**Description:**  
Split requirements into smallest meaningful units.

**Associated Invariants:**  
CDD_REQUIREMENT_GRANULARITY_FIT  

---

### STEP 04 — Extract Invariants  
**Tagline:** Capture irreducible truths  

**Description:**  
Transform semantic units into invariant statements.

**Associated Invariants:**  
CDD_INVARIANT_IRREDUCIBLE_TRUTH, CDD_INVARIANT_DERIVATION_REQUIRED  

---

### STEP 05 — Remove Redundancy  
**Tagline:** Eliminate duplication  

**Description:**  
Merge or remove overlapping invariants.

**Associated Invariants:**  
CDD_INVARIANT_NON_REDUNDANCY  

---

### STEP 06 — Validate Minimality  
**Tagline:** Ensure necessity  

**Description:**  
Each invariant must be essential and minimal.

**Associated Invariants:**  
CDD_INVARIANT_MINIMALITY, CDD_INVARIANT_NECESSITY  

---

### STEP 07 — Define Negative Space  
**Tagline:** Capture what must not exist  

**Description:**  
Explicitly define forbidden states.

**Associated Invariants:**  
CDD_INVARIANT_NEGATIVE_SPACE  

---

### STEP 08 — Resolve Conflicts  
**Tagline:** Remove contradictions  

**Description:**  
Ensure invariants are consistent.

**Associated Invariants:**  
CDD_INVARIANT_CONFLICT_RESOLUTION  

---

### STEP 09 — Review Gate  
**Tagline:** Validate integrity  

**Description:**  
Check coverage and clarity.

**Associated Invariants:**  
CDD_CLOSURE_PARENT_CHILD_COVERAGE  

---

### STEP 10 — Finalize Invariants  
**Tagline:** Lock semantic truth  

**Description:**  
Freeze invariant set.

**Associated Invariants:**  
CDD_CLOSURE_BEFORE_AUTHORITY  

---

### STEP 11 — Publish Invariants  
**Tagline:** Enable constraint derivation  

**Description:**  
Provide invariant set for next phase.

**Associated Invariants:**  
CDD_TRACEABILITY_INVARIANT_TO_CONSTRAINT  

---

## Exit Criteria

- Invariants are minimal, non-redundant, and complete  
- Fully traceable to requirements  
- No conflicts  
- Negative space defined  
- Ready for constraint derivation  

---

## Final Compression

This phase transforms structured intent into irreducible semantic truth that governs all downstream behavior.
