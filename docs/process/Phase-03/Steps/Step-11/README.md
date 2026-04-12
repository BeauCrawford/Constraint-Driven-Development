# Step 11 - Publish Closure Report

---

## Description

Step 11, Publish Closure Report, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_PUBLICATION_REQUIRED**
An authoritative closure report must be published before downstream constraint derivation.

**CDD_P03_PUBLICATION_CONTENT_COMPLETE**
The closure report must include coverage evidence, gaps, unauthorized additions, drift records, score or threshold result, refinements, and governed exceptions.

**CDD_P03_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve closure status through the published closure report.

**CDD_P03_PUBLICATION_ACCESSIBILITY**
The closure report must be accessible to downstream actors and tools that perform constraint derivation.

**CDD_P03_PUBLICATION_VERSION_VISIBILITY**
The published closure report must expose the requirement and invariant baselines it validates.

**CDD_P03_PUBLICATION_NO_ORPHAN_FINDINGS**
No closure finding may lack linkage to affected requirements, invariants, glossary terms, or governance records.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Publish Closure Report, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Publish Closure Report.

**Invariants:** See step invariants above.

**Prompts**
- Publish Closure Report Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Publish Closure Report Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Publish Closure Report
*Execute Publish Closure Report with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Publish Closure Report while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Publish Closure Report with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Publish Closure Report Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Publish Closure Report Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Publish Closure Report.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Publish Closure Report Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Publish Closure Report Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
