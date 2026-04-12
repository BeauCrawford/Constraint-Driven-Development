# Step 08 - Detect Coverage Gaps

---

## Description

Step 08, Detect Coverage Gaps, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_GAP_DETECTION_REQUIRED**
Phase 10 must detect uncovered constraints and semantic areas.

**CDD_P10_GAP_CONSTRAINT_LINEAGE**
Coverage gaps must identify affected CONSTRAINT_IDs and upstream lineage.

**CDD_P10_GAP_CLASSIFICATION**
Gaps must be classified as blocking, non-blocking, or governed exception.

**CDD_P10_GAP_NO_SILENT_DEFERRAL**
Coverage gaps must not be hidden or deferred without governance.

**CDD_P10_GAP_RESOLUTION_PATH**
Each gap must identify the phase or artifact requiring correction.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Coverage Gaps, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Coverage Gaps.

**Invariants:** See step invariants above.

**Prompts**
- Detect Coverage Gaps Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Coverage Gaps Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Coverage Gaps
*Execute Detect Coverage Gaps with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Coverage Gaps while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Coverage Gaps with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Coverage Gaps Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Coverage Gaps Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Coverage Gaps.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Coverage Gaps Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Coverage Gaps Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.