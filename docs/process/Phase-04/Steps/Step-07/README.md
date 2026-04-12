# Step 07 - Assign CONSTRAINT_IDs

---

## Description

Step 07, Assign CONSTRAINT_IDs, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_CONSTRAINT_ID_REQUIRED**
Every published constraint must have a stable CONSTRAINT_ID.

**CDD_P04_CONSTRAINT_ID_UNIQUENESS**
No two constraints may share the same CONSTRAINT_ID.

**CDD_P04_CONSTRAINT_ID_STABILITY**
CONSTRAINT_IDs must not change because wording is refined.

**CDD_P04_CONSTRAINT_ID_NON_REUSE**
Retired or rejected CONSTRAINT_IDs must not be reused for different rule authority.

**CDD_P04_CONSTRAINT_ID_TRACE_BINDING**
Each CONSTRAINT_ID must bind constraint text to its authorizing invariant lineage.

**CDD_P04_CONSTRAINT_ID_ADDRESSABILITY**
Each constraint must be directly referable by ID in tests, coverage reports, reviews, gaps, and exceptions.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Assign CONSTRAINT_IDs, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Assign CONSTRAINT_IDs.

**Invariants:** See step invariants above.

**Prompts**
- Assign CONSTRAINT_IDs Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Assign CONSTRAINT_IDs Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Assign CONSTRAINT_IDs
*Execute Assign CONSTRAINT_IDs with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Assign CONSTRAINT_IDs while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Assign CONSTRAINT_IDs with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Assign CONSTRAINT_IDs Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Assign CONSTRAINT_IDs Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Assign CONSTRAINT_IDs.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Assign CONSTRAINT_IDs Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Assign CONSTRAINT_IDs Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
