# Step 06 - Encode Failure Semantics

---

## Description

Step 06, Encode Failure Semantics, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_FAILURE_SEMANTICS_REQUIRED**
Each constraint must define how violation is recognized or represented.

**CDD_P04_FAILURE_CONDITION_EXPLICITNESS**
Failure conditions must be explicit and tied to constraint semantics.

**CDD_P04_FAILURE_NO_IMPLEMENTATION_LOCK_IN**
Failure semantics must not prescribe implementation mechanisms unless required by upstream authority.

**CDD_P04_FAILURE_BOUNDARY_ALIGNMENT**
Failure semantics must align with negative and boundary cases.

**CDD_P04_FAILURE_DETERMINISM**
Failure semantics must be deterministic enough to support reproducible proof.

**CDD_P04_FAILURE_TRACEABILITY**
Failure semantics must remain traceable to the constraints and invariants that authorize them.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Encode Failure Semantics, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Encode Failure Semantics.

**Invariants:** See step invariants above.

**Prompts**
- Encode Failure Semantics Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Encode Failure Semantics Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Encode Failure Semantics
*Execute Encode Failure Semantics with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Encode Failure Semantics while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Encode Failure Semantics with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Encode Failure Semantics Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Encode Failure Semantics Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Encode Failure Semantics.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Encode Failure Semantics Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Encode Failure Semantics Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
