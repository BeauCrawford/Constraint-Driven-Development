# Step 08 - Detect Orphan Artifacts

---

## Description

Step 08, Detect Orphan Artifacts, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_ORPHAN_DETECTION_REQUIRED**
Phase 09 must detect artifacts without valid lineage.

**CDD_P09_NO_ORPHAN_REQUIREMENTS**
Requirements must have governance status and downstream mapping or exception.

**CDD_P09_NO_ORPHAN_INVARIANTS**
Invariants must have requirement lineage.

**CDD_P09_NO_ORPHAN_CONSTRAINTS**
Constraints must have invariant lineage and proof mapping.

**CDD_P09_NO_ORPHAN_TESTS**
Tests must have constraint lineage.

**CDD_P09_NO_ORPHAN_CODE**
Code must have proof lineage.

**CDD_P09_ORPHAN_RESOLUTION_REQUIRED**
Unresolved orphan artifacts block traceability approval.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Orphan Artifacts, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Orphan Artifacts.

**Invariants:** See step invariants above.

**Prompts**
- Detect Orphan Artifacts Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Orphan Artifacts Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Orphan Artifacts
*Execute Detect Orphan Artifacts with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Orphan Artifacts while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Orphan Artifacts with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Orphan Artifacts Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Orphan Artifacts Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Orphan Artifacts.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Orphan Artifacts Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Orphan Artifacts Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
