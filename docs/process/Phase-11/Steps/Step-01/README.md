# Step 01 - Submit Change Request

---

## Description

Step 01, Submit Change Request, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_CHANGE_REQUEST_REQUIRED**
Change must be captured as a governed change request before downstream artifacts are altered.

**CDD_P11_CHANGE_SOURCE_ATTRIBUTION**
Each change request must identify its source, authority, and rationale.

**CDD_P11_CHANGE_INTENT_VISIBILITY**
Requested semantic change must be visible before implementation work begins.

**CDD_P11_NO_UNRECORDED_CHANGE**
Unrecorded edits to downstream artifacts must not grant change authority.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Submit Change Request, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Submit Change Request.

**Invariants:** See step invariants above.

**Prompts**
- Submit Change Request Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Submit Change Request Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Submit Change Request
*Execute Submit Change Request with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Submit Change Request while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Submit Change Request with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Submit Change Request Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Submit Change Request Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Submit Change Request.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Submit Change Request Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Submit Change Request Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
