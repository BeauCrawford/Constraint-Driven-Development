# Step 09 - Publish Change Report

---

## Description

Step 09, Publish Change Report, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_PUBLICATION_REQUIRED**
An authoritative change report must be published.

**CDD_P11_PUBLICATION_CONTENT_COMPLETE**
Publication must include change request, impact classification, upstream updates, regenerated artifacts, stale artifact detection, drift resolution, revalidation evidence, and exceptions.

**CDD_P11_PUBLICATION_SINGLE_AUTHORITY**
Governance must resolve change integrity through the published change report.

**CDD_P11_PUBLICATION_VERSION_VISIBILITY**
The change report must identify before and after artifact baselines.

**CDD_P11_PUBLICATION_NO_ORPHAN_CHANGE_EVIDENCE**
No change evidence may lack affected artifact lineage.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Publish Change Report, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Publish Change Report.

**Invariants:** See step invariants above.

**Prompts**
- Publish Change Report Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Publish Change Report Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Publish Change Report
*Execute Publish Change Report with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Publish Change Report while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Publish Change Report with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Publish Change Report Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Publish Change Report Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Publish Change Report.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Publish Change Report Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Publish Change Report Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
