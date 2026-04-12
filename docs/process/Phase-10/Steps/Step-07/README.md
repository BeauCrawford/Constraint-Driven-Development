# Step 07 - Revalidate Semantic Closure

---

## Description

Step 07, Revalidate Semantic Closure, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_CLOSURE_REVALIDATION_REQUIRED**
Closure must be revalidated across requirement, invariant, constraint, test, and code layers.

**CDD_P10_CLOSURE_PARENT_CHILD_COVERAGE**
Each child layer must preserve parent meaning.

**CDD_P10_CLOSURE_NO_SILENT_LOSS**
No parent meaning may be silently absent downstream.

**CDD_P10_CLOSURE_NO_UNAUTHORIZED_ADDITION**
No child layer may introduce unauthorized meaning.

**CDD_P10_CLOSURE_NEGATIVE_SPACE_INCLUDED**
Forbidden states and negative-space semantics must be included.

**CDD_P10_CLOSURE_EVIDENCE_REQUIRED**
Closure conclusions must be backed by reviewable evidence.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Revalidate Semantic Closure, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Revalidate Semantic Closure.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Semantic Closure Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Revalidate Semantic Closure Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Revalidate Semantic Closure
*Execute Revalidate Semantic Closure with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Revalidate Semantic Closure while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Revalidate Semantic Closure with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Semantic Closure Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Revalidate Semantic Closure Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Revalidate Semantic Closure.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Semantic Closure Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Revalidate Semantic Closure Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.