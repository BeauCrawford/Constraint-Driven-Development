# Step 06 - Generate Boundary Tests

---

## Description

Step 06, Generate Boundary Tests, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_BOUNDARY_TEST_REQUIRED**
Constraints with edge conditions must have boundary proof tests.

**CDD_P06_BOUNDARY_TEST_CONSTRAINT_AUTHORITY**
Boundary tests must derive from constraint boundary semantics or contract boundary definitions.

**CDD_P06_BOUNDARY_LIMIT_EXPLICITNESS**
Limits, thresholds, transitions, empty states, and edge cases must be explicit where governed.

**CDD_P06_BOUNDARY_NO_INVENTED_EDGES**
Boundary tests must not invent edge semantics absent from constraints or contracts.

**CDD_P06_BOUNDARY_TRACEABILITY**
Each boundary test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_BOUNDARY_GAP_VISIBILITY**
Missing boundary proof must be recorded as a coverage gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Generate Boundary Tests, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Generate Boundary Tests.

**Invariants:** See step invariants above.

**Prompts**
- Generate Boundary Tests Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Generate Boundary Tests Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Generate Boundary Tests
*Execute Generate Boundary Tests with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Generate Boundary Tests while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Generate Boundary Tests with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Generate Boundary Tests Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Generate Boundary Tests Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Generate Boundary Tests.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Generate Boundary Tests Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Generate Boundary Tests Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.