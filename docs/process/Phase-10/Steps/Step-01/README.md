# Step 01 - Load Traceability Matrix

---

## Description

Step 01, Load Traceability Matrix, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_TRACEABILITY_INPUT_REQUIRED**
Phase 10 must load the published Phase 09 traceability report.

**CDD_P10_TRACEABILITY_BASELINE_VISIBLE**
The traceability report baseline, version, or revision state must be visible.

**CDD_P10_TRACEABILITY_SCOPE_AUTHORITY**
Traceability must define the validation scope for coverage and closure.

**CDD_P10_TRACEABILITY_DEFECT_ESCALATION**
Traceability gaps discovered during revalidation must be escalated to Phase 09.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Traceability Matrix, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Traceability Matrix.

**Invariants:** See step invariants above.

**Prompts**
- Load Traceability Matrix Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Traceability Matrix Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Traceability Matrix
*Execute Load Traceability Matrix with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Traceability Matrix while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Traceability Matrix with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Traceability Matrix Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Traceability Matrix Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Traceability Matrix.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Traceability Matrix Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Traceability Matrix Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.