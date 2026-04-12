# Step 05 - Run Tests Against Real Implementation

---

## Description

Step 05, Run Tests Against Real Implementation, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_REAL_PROOF_EXECUTION_REQUIRED**
The deterministic proof suite must execute against the real implementation.

**CDD_P08_FULL_APPLICABLE_SUITE_REQUIRED**
All applicable tests must run or be governed exceptions.

**CDD_P08_GREEN_STATE_REQUIRED**
Implementation cannot gain authority unless the applicable proof suite passes.

**CDD_P08_EXECUTION_DETERMINISM**
Proof execution against real implementation must be deterministic and reproducible.

**CDD_P08_RESULT_CAPTURE**
Test results must be captured with test, constraint, and implementation mapping evidence.

**CDD_P08_FAILURE_VISIBILITY**
Failures, skips, flakes, and environmental defects must be visible.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Run Tests Against Real Implementation, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Run Tests Against Real Implementation.

**Invariants:** See step invariants above.

**Prompts**
- Run Tests Against Real Implementation Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Run Tests Against Real Implementation Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Run Tests Against Real Implementation
*Execute Run Tests Against Real Implementation with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Run Tests Against Real Implementation while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Run Tests Against Real Implementation with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Run Tests Against Real Implementation Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Run Tests Against Real Implementation Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Run Tests Against Real Implementation.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Run Tests Against Real Implementation Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Run Tests Against Real Implementation Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.