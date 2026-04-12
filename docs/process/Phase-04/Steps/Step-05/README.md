# Step 05 - Define Positive / Negative / Boundary Cases

---

## Description

Step 05, Define Positive / Negative / Boundary Cases, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_PNB_CASES_REQUIRED**
Constraints must define positive, negative, and boundary behavior when semantically applicable.

**CDD_P04_POSITIVE_CASE_AUTHORITY**
Positive cases must describe behavior admitted by invariant authority.

**CDD_P04_NEGATIVE_CASE_AUTHORITY**
Negative cases must describe behavior forbidden by invariant authority or negative-space definitions.

**CDD_P04_BOUNDARY_CASE_AUTHORITY**
Boundary cases must describe edge conditions implied by invariant meaning, scope, or glossary definitions.

**CDD_P04_PNB_NO_UNAUTHORIZED_EXPANSION**
Positive, negative, and boundary cases must not expand behavior beyond validated invariants.

**CDD_P04_PNB_COMPLETENESS**
Missing positive, negative, or boundary semantics must be recorded as a derivation gap.

**CDD_P04_PNB_TEST_READINESS**
Positive, negative, and boundary cases must be precise enough to support later proof construction.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Define Positive / Negative / Boundary Cases, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Define Positive / Negative / Boundary Cases.

**Invariants:** See step invariants above.

**Prompts**
- Define Positive / Negative / Boundary Cases Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Define Positive / Negative / Boundary Cases Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Define Positive / Negative / Boundary Cases
*Execute Define Positive / Negative / Boundary Cases with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Define Positive / Negative / Boundary Cases while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Define Positive / Negative / Boundary Cases with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Define Positive / Negative / Boundary Cases Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Define Positive / Negative / Boundary Cases Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Define Positive / Negative / Boundary Cases.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Define Positive / Negative / Boundary Cases Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Define Positive / Negative / Boundary Cases Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
