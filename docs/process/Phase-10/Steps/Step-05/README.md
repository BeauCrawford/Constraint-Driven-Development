# Step 05 - Load Requirements

---

## Description

Step 05, Load Requirements, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_REQUIREMENT_INPUT_REQUIRED**
The published requirement set must be loaded as source intent.

**CDD_P10_REQUIREMENT_ID_VISIBILITY**
Requirement IDs must remain visible for closure revalidation.

**CDD_P10_REQUIREMENT_SCOPE_VISIBLE**
Scope, assumptions, conflict decisions, and governed exceptions must be available.

**CDD_P10_REQUIREMENT_BASELINE_VISIBLE**
The requirement baseline version, publication identity, or revision state must be visible.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Requirements, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Requirements.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirements Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Requirements Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Requirements
*Execute Load Requirements with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Requirements while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Requirements with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirements Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Requirements Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Requirements.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Requirements Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Requirements Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.