# Step 09 - Review Gate

---

## Description

Step 09, Review Gate, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_REVIEW_GATE_REQUIRED**
The closure report must pass a review gate before invariant refinement is finalized or downstream authority is granted.

**CDD_P03_REVIEW_THRESHOLD_EVIDENCE**
Review must validate that closure thresholds were met or exceptions were governed.

**CDD_P03_REVIEW_GAP_EVIDENCE**
Review must inspect gap, unauthorized addition, and drift records.

**CDD_P03_REVIEW_DECISION_AUTHORITY**
Approval, rejection, and exception decisions must identify responsible authority.

**CDD_P03_REVIEW_NO_CEREMONIAL_APPROVAL**
Approval without closure evidence does not grant downstream authority.

**CDD_P03_REVIEW_TRACEABILITY**
Review findings must link to affected requirements, invariants, glossary terms, gaps, additions, and drift records.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Review Gate, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Review Gate.

**Invariants:** See step invariants above.

**Prompts**
- Review Gate Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Review Gate Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Review Gate
*Execute Review Gate with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Review Gate while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Review Gate with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Review Gate Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Review Gate Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Review Gate.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Review Gate Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Review Gate Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
