# Step 03 - Submit Exceptions

---

## Description

Step 03, Submit Exceptions, performs its Phase 12 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P12_EXCEPTION_SUBMISSION_REQUIRED**
All exceptions, bypasses, unresolved gaps, and accepted risks must be submitted.

**CDD_P12_EXCEPTION_OWNERSHIP_REQUIRED**
Each exception must have an owner.

**CDD_P12_EXCEPTION_JUSTIFICATION_REQUIRED**
Each exception must include rationale and affected artifacts.

**CDD_P12_EXCEPTION_RECONCILIATION_BOUND**
Each exception must be time-bounded, reconciliation-bound, or explicitly permanent by governance decision.

**CDD_P12_EXCEPTION_NO_HIDDEN_BYPASS**
Hidden bypasses or undocumented deviations cannot grant authority.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Submit Exceptions, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 12 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Submit Exceptions.

**Invariants:** See step invariants above.

**Prompts**
- Submit Exceptions Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Submit Exceptions Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Submit Exceptions
*Execute Submit Exceptions with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Submit Exceptions while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Submit Exceptions with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Submit Exceptions Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Submit Exceptions Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Submit Exceptions.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Submit Exceptions Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Submit Exceptions Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.