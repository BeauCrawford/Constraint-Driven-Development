# Step 07 - Report Failures

---

## Description

Step 07, Report Failures, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_FAILURE_REPORTING_REQUIRED**
Any mismatch between implementation and proof must be reported.

**CDD_P08_FAILURE_REVERSE_NAVIGATION**
Implementation failures must be traceable upstream to tests, constraints, contracts, invariants, and requirements.

**CDD_P08_FAILURE_CLASSIFICATION**
Failures must be classified as implementation defect, proof defect, contract defect, constraint defect, or upstream semantic defect.

**CDD_P08_FAILURE_NO_SILENT_PATCHING**
Failures must not be hidden or patched downstream without preserving upstream authority.

**CDD_P08_FAILURE_BLOCKS_PUBLICATION**
Unresolved proof failures block implementation publication.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Report Failures, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Report Failures.

**Invariants:** See step invariants above.

**Prompts**
- Report Failures Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Report Failures Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Report Failures
*Execute Report Failures with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Report Failures while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Report Failures with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Report Failures Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Report Failures Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Report Failures.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Report Failures Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Report Failures Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
