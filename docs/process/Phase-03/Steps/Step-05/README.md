# Step 05 - Detect Gaps

---

## Description

Step 05, Detect Gaps, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_GAP_DETECTION_REQUIRED**
Phase 03 must detect requirement meaning not represented in the invariant set.

**CDD_P03_GAP_REQUIREMENT_LINEAGE**
Each semantic gap must identify the affected requirement IDs and missing meaning.

**CDD_P03_GAP_NO_SILENT_LOSS**
Missing requirement meaning must not be ignored, absorbed into review notes, or deferred without governance.

**CDD_P03_GAP_CLASSIFICATION**
Each gap must be classified as blocking, non-blocking, or governed exception.

**CDD_P03_GAP_RESOLUTION_PATH**
Each gap must identify whether resolution requires invariant refinement, requirement clarification, glossary update, or governance exception.

**CDD_P03_GAP_TRACE_RETENTION**
Gap records must remain traceable after invariant refinement or upstream correction.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Gaps, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Gaps.

**Invariants:** See step invariants above.

**Prompts**
- Detect Gaps Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Gaps Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Gaps
*Execute Detect Gaps with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Gaps while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Gaps with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Gaps Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Gaps Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Gaps.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Gaps Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Gaps Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
