# Step 09 - Ensure Completeness vs Invariants

---

## Description

Step 09, Ensure Completeness vs Invariants, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_COMPLETENESS_CHECK_REQUIRED**
The constraint set must be checked for complete enforcement of validated invariants.

**CDD_P04_INVARIANT_TO_CONSTRAINT_COVERAGE**
Every validated invariant must map to one or more constraints or a governed exception.

**CDD_P04_CONSTRAINT_TO_INVARIANT_COVERAGE**
Every constraint must map back to one or more validated invariants.

**CDD_P04_NEGATIVE_SPACE_ENFORCEMENT**
Negative-space definitions must be enforced by constraints where applicable.

**CDD_P04_COMPLETENESS_NO_ORPHAN_RULES**
No constraint may exist without invariant authority.

**CDD_P04_COMPLETENESS_GAP_VISIBILITY**
Missing constraint coverage must be recorded as a gap with impacted invariants.

**CDD_P04_COMPLETENESS_GATE_BOUND**
Blocking completeness gaps must prevent review approval and publication.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Ensure Completeness vs Invariants, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Ensure Completeness vs Invariants.

**Invariants:** See step invariants above.

**Prompts**
- Ensure Completeness vs Invariants Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Ensure Completeness vs Invariants Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Ensure Completeness vs Invariants
*Execute Ensure Completeness vs Invariants with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Ensure Completeness vs Invariants while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Ensure Completeness vs Invariants with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Ensure Completeness vs Invariants Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Ensure Completeness vs Invariants Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Ensure Completeness vs Invariants.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Ensure Completeness vs Invariants Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Ensure Completeness vs Invariants Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
