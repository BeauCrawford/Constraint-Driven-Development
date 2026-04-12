# Step 07 - Review Exceptions

---

## Description

Step 07, Review Exceptions, performs its Phase 12 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P12_EXCEPTION_REVIEW_REQUIRED**
Governance must review all submitted exceptions.

**CDD_P12_EXCEPTION_BLOCKING_CLASSIFICATION**
Each exception must be classified as blocking, accepted, deferred, or resolved.

**CDD_P12_EXCEPTION_RISK_VISIBILITY**
Exception risk and affected CDD invariants must be visible.

**CDD_P12_EXCEPTION_DECISION_AUTHORITY**
Exception decisions must identify responsible authority.

**CDD_P12_EXCEPTION_REVIEW_TRACEABILITY**
Exception decisions must link to artifacts, evidence, owners, and reconciliation obligations.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Review Exceptions, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 12 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Review Exceptions.

**Invariants:** See step invariants above.

**Prompts**
- Review Exceptions Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Review Exceptions Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Review Exceptions
*Execute Review Exceptions with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Review Exceptions while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Review Exceptions with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Review Exceptions Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Review Exceptions Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Review Exceptions.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Review Exceptions Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Review Exceptions Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.