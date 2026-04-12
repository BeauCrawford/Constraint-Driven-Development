# Step 01 - Load Constraints

---

## Description

Step 01, Load Constraints, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_CONSTRAINT_SOURCE_REQUIRED**
Phase 06 must load the published Phase 04 constraint set as the proof authority.

**CDD_P06_CONSTRAINT_ID_REQUIRED**
Only constraints with stable CONSTRAINT_IDs may be used for authoritative test generation.

**CDD_P06_CONSTRAINT_BASELINE_VISIBLE**
The constraint baseline version, publication identity, or revision state must be visible.

**CDD_P06_CONSTRAINT_PNB_FAILURE_VISIBLE**
Positive, negative, boundary, and failure semantics must be available to test generation.

**CDD_P06_CONSTRAINT_NO_INFORMAL_AUTHORITY**
Unpublished constraints, notes, or manual expectations must not authorize tests.

**CDD_P06_CONSTRAINT_INPUT_DEFECT_ESCALATION**
Missing IDs, missing failure semantics, contradictions, or incomplete mappings must be escalated upstream rather than silently patched in tests.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Constraints, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Constraints.

**Invariants:** See step invariants above.

**Prompts**
- Load Constraints Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Constraints Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Constraints
*Execute Load Constraints with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Constraints while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Constraints with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Constraints Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Constraints Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Constraints.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Constraints Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Constraints Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
