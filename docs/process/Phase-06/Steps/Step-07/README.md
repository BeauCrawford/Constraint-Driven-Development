# Step 07 - Generate Failure-Path Tests

---

## Description

Step 07, Generate Failure-Path Tests, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_FAILURE_TEST_REQUIRED**
Constraints with failure semantics must have failure-path proof tests.

**CDD_P06_FAILURE_TEST_CONSTRAINT_AUTHORITY**
Failure tests must derive from explicit constraint or contract failure semantics.

**CDD_P06_FAILURE_ASSERTION_EXPLICITNESS**
Failure tests must assert failure behavior, detection, response, or containment explicitly.

**CDD_P06_FAILURE_NO_INVENTED_FAILURE**
Failure tests must not create failure modes absent from governing artifacts.

**CDD_P06_FAILURE_TRACEABILITY**
Each failure-path test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_FAILURE_GAP_VISIBILITY**
Missing failure proof must be recorded as a coverage gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Generate Failure-Path Tests, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Generate Failure-Path Tests.

**Invariants:** See step invariants above.

**Prompts**
- Generate Failure-Path Tests Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Generate Failure-Path Tests Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Generate Failure-Path Tests
*Execute Generate Failure-Path Tests with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Generate Failure-Path Tests while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Generate Failure-Path Tests with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Generate Failure-Path Tests Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Generate Failure-Path Tests Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Generate Failure-Path Tests.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Generate Failure-Path Tests Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Generate Failure-Path Tests Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
