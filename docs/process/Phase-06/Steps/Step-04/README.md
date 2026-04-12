# Step 04 - Generate Positive Tests

---

## Description

Step 04, Generate Positive Tests, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_POSITIVE_TEST_REQUIRED**
Constraints with required or allowed behavior must have positive proof tests.

**CDD_P06_POSITIVE_TEST_CONSTRAINT_AUTHORITY**
Positive tests must derive from constraint-admitted behavior.

**CDD_P06_POSITIVE_ASSERTION_EXPLICITNESS**
Positive tests must assert expected outcomes explicitly.

**CDD_P06_POSITIVE_NO_OVERBROAD_ACCEPTANCE**
Positive tests must not admit behavior beyond the governing constraints.

**CDD_P06_POSITIVE_TRACEABILITY**
Each positive test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_POSITIVE_GAP_VISIBILITY**
Missing positive proof must be recorded as a coverage gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Generate Positive Tests, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Generate Positive Tests.

**Invariants:** See step invariants above.

**Prompts**
- Generate Positive Tests Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Generate Positive Tests Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Generate Positive Tests
*Execute Generate Positive Tests with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Generate Positive Tests while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Generate Positive Tests with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Generate Positive Tests Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Generate Positive Tests Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Generate Positive Tests.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Generate Positive Tests Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Generate Positive Tests Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.