# Step 05 - Execute Test Suite

---

## Description

Step 05, Execute Test Suite, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_EXECUTION_REQUIRED**
The full applicable test suite must execute against the registered doubles.

**CDD_P07_EXECUTION_DETERMINISM**
Execution must be deterministic and reproducible.

**CDD_P07_EXECUTION_NO_RUNTIME_INTERPRETATION**
Test execution must not require unresolved runtime interpretation.

**CDD_P07_EXECUTION_COMPLETE_SCOPE**
All tests in the Phase 06 suite applicable to simulation must be run or explicitly excepted.

**CDD_P07_EXECUTION_RESULT_CAPTURE**
Execution results must be captured with test IDs, CONSTRAINT_ID mappings, and contract bindings.

**CDD_P07_EXECUTION_FAILURE_VISIBILITY**
Any execution failure, skip, flake, or environmental defect must be visible.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Execute Test Suite, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Execute Test Suite.

**Invariants:** See step invariants above.

**Prompts**
- Execute Test Suite Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Execute Test Suite Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Execute Test Suite
*Execute Execute Test Suite with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Execute Test Suite while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Execute Test Suite with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Execute Test Suite Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Execute Test Suite Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Execute Test Suite.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Execute Test Suite Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Execute Test Suite Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.