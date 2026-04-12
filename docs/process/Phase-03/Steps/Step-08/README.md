# Step 08 - Score Closure

---

## Description

Step 08, Score Closure, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_CLOSURE_SCORE_REQUIRED**
Closure validation must produce a measurable closure score or threshold result.

**CDD_P03_CLOSURE_SCORE_DEFINITION_VISIBLE**
The scoring method, threshold, or pass/fail criteria must be visible.

**CDD_P03_CLOSURE_SCORE_EVIDENCE_LINKED**
Closure scores must link to coverage, gap, addition, and drift evidence.

**CDD_P03_CLOSURE_SCORE_NO_CONFIDENCE_SUBSTITUTION**
Subjective confidence must not substitute for closure evidence.

**CDD_P03_CLOSURE_SCORE_THRESHOLD_BOUND**
Closure approval must be bound to explicit thresholds or explicit governance exception.

**CDD_P03_CLOSURE_SCORE_RECOMPUTABLE**
Closure scoring must be reproducible from the published inputs and recorded evidence.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Score Closure, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Score Closure.

**Invariants:** See step invariants above.

**Prompts**
- Score Closure Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Score Closure Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Score Closure
*Execute Score Closure with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Score Closure while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Score Closure with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Score Closure Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Score Closure Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Score Closure.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Score Closure Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Score Closure Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
