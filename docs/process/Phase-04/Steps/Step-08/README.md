# Step 08 - Check Non-Contradiction & Satisfiability

---

## Description

Step 08, Check Non-Contradiction & Satisfiability, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_CONSISTENCY_CHECK_REQUIRED**
The constraint set must be checked for contradiction before publication.

**CDD_P04_CONSTRAINT_NON_CONTRADICTION**
No constraint may make another constraint impossible to satisfy unless the conflict is resolved.

**CDD_P04_SATISFIABILITY_REQUIRED**
The constraint set must admit at least one valid implementation or explicitly identify an upstream contradiction.

**CDD_P04_CONFLICT_LINEAGE**
Constraint conflicts must identify affected constraints, invariants, and requirement lineage.

**CDD_P04_CONFLICT_NO_SILENT_OVERRIDE**
A constraint must not override another constraint without a visible resolution artifact.

**CDD_P04_CONFLICT_UPSTREAM_ESCALATION**
Conflicts caused by invariant or requirement issues must be escalated upstream rather than patched in Phase 04.

**CDD_P04_CONFLICT_BLOCKS_PUBLICATION**
Unresolved constraint contradictions block publication.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Check Non-Contradiction & Satisfiability, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Check Non-Contradiction & Satisfiability.

**Invariants:** See step invariants above.

**Prompts**
- Check Non-Contradiction & Satisfiability Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Check Non-Contradiction & Satisfiability Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Check Non-Contradiction & Satisfiability
*Execute Check Non-Contradiction & Satisfiability with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Check Non-Contradiction & Satisfiability while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Check Non-Contradiction & Satisfiability with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Check Non-Contradiction & Satisfiability Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Check Non-Contradiction & Satisfiability Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Check Non-Contradiction & Satisfiability.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Check Non-Contradiction & Satisfiability Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Check Non-Contradiction & Satisfiability Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
