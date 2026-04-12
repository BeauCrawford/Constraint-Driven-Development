# Step 01 - Provide Contract-Bound Tests

---

## Description

Step 01, Provide Contract-Bound Tests, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_TEST_SUITE_SOURCE_REQUIRED**
Phase 07 must load the published Phase 06 test suite as the simulation proof driver.

**CDD_P07_TEST_SUITE_BASELINE_VISIBLE**
The test suite baseline version, publication identity, or revision state must be visible.

**CDD_P07_TEST_CONSTRAINT_MAPPING_VISIBLE**
Test-to-CONSTRAINT_ID mappings must remain visible during simulation.

**CDD_P07_TEST_CONTRACT_BINDING_VISIBLE**
Contract bindings for boundary-relevant tests must be visible.

**CDD_P07_TEST_NO_UNPUBLISHED_AUTHORITY**
Unpublished tests, exploratory checks, or manual expectations must not grant validation authority.

**CDD_P07_TEST_INPUT_DEFECT_ESCALATION**
Missing mappings, nondeterminism, or incomplete test coverage must be escalated upstream rather than silently patched in Phase 07.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Provide Contract-Bound Tests, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Provide Contract-Bound Tests.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contract-Bound Tests Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Provide Contract-Bound Tests Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Provide Contract-Bound Tests
*Execute Provide Contract-Bound Tests with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Provide Contract-Bound Tests while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Provide Contract-Bound Tests with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contract-Bound Tests Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Provide Contract-Bound Tests Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Provide Contract-Bound Tests.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contract-Bound Tests Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Provide Contract-Bound Tests Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
