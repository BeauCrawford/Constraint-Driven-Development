# Step 01 - Load Requirement IDs

---

## Description

Step 01, Load Requirement IDs, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_REQUIREMENT_IDS_REQUIRED**
Stable requirement IDs must be loaded as source traceability anchors.

**CDD_P09_REQUIREMENT_BASELINE_VISIBLE**
The requirement baseline version, publication identity, or revision state must be visible.

**CDD_P09_REQUIREMENT_ID_UNIQUENESS_VISIBLE**
Requirement ID uniqueness must be validated or evidenced.

**CDD_P09_REQUIREMENT_NO_ORPHAN_SOURCE**
No governed requirement may lack source and governance status.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Requirement IDs, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Requirement IDs.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirement IDs Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Requirement IDs Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Requirement IDs
*Execute Load Requirement IDs with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Requirement IDs while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Requirement IDs with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirement IDs Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Requirement IDs Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Requirement IDs.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirement IDs Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Requirement IDs Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.