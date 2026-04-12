# Step 08 - Map Tests to CONSTRAINT_IDs

---

## Description

Step 08, Map Tests to CONSTRAINT_IDs, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_TEST_MAPPING_REQUIRED**
Every authoritative test must map to one or more CONSTRAINT_IDs.

**CDD_P06_TEST_NO_ORPHANS**
No published test may lack constraint lineage.

**CDD_P06_CONSTRAINT_TO_TEST_TRACEABILITY**
Each constraint must expose its mapped tests.

**CDD_P06_TEST_TO_CONSTRAINT_TRACEABILITY**
Each test must expose its governing constraints.

**CDD_P06_MAPPING_STABILITY**
Mappings must remain stable across wording refinements unless authority changes.

**CDD_P06_MAPPING_GAP_VISIBILITY**
Unmapped tests and untested constraints must be recorded as gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Map Tests to CONSTRAINT_IDs, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Map Tests to CONSTRAINT_IDs.

**Invariants:** See step invariants above.

**Prompts**
- Map Tests to CONSTRAINT_IDs Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Map Tests to CONSTRAINT_IDs Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Map Tests to CONSTRAINT_IDs
*Execute Map Tests to CONSTRAINT_IDs with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Map Tests to CONSTRAINT_IDs while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Map Tests to CONSTRAINT_IDs with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Map Tests to CONSTRAINT_IDs Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Map Tests to CONSTRAINT_IDs Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Map Tests to CONSTRAINT_IDs.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Map Tests to CONSTRAINT_IDs Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Map Tests to CONSTRAINT_IDs Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.