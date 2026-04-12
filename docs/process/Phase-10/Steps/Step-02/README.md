# Step 02 - Load Test Results

---

## Description

Step 02, Load Test Results, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_TEST_RESULTS_REQUIRED**
Implementation proof results from Phase 08 must be loaded.

**CDD_P10_TEST_RESULT_BASELINE_VISIBLE**
The test result baseline, run identity, or revision state must be visible.

**CDD_P10_TEST_RESULT_DETERMINISM_VISIBLE**
Determinism and reproducibility evidence must be available.

**CDD_P10_TEST_RESULT_FAILURE_VISIBILITY**
Failures, skips, flakes, and governed exceptions must be visible.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Test Results, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Test Results.

**Invariants:** See step invariants above.

**Prompts**
- Load Test Results Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Test Results Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Test Results
*Execute Load Test Results with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Test Results while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Test Results with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Test Results Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Test Results Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Test Results.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Test Results Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Test Results Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
