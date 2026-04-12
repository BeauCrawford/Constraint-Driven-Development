# Step 10 - Review Gate

---

## Description

Step 10, Review Gate, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_REVIEW_GATE_REQUIRED**
The constraint set must pass a review gate before publication.

**CDD_P04_REVIEW_PRECISION_EVIDENCE**
Review must include evidence that constraints are executable and precise.

**CDD_P04_REVIEW_COVERAGE_EVIDENCE**
Review must include invariant-to-constraint coverage evidence.

**CDD_P04_REVIEW_ID_EVIDENCE**
Review must validate CONSTRAINT_ID uniqueness, stability, and addressability.

**CDD_P04_REVIEW_CONSISTENCY_EVIDENCE**
Review must validate non-contradiction and satisfiability evidence.

**CDD_P04_REVIEW_TRACEABILITY_EVIDENCE**
Review must validate requirement-to-invariant-to-constraint lineage.

**CDD_P04_REVIEW_EXCEPTION_VISIBILITY**
Any exception to Phase 04 invariants must be visible, justified, owned, and reconciliation-bound.

**CDD_P04_REVIEW_NO_CEREMONIAL_APPROVAL**
Review approval without evidence does not grant downstream authority.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Review Gate, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

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
