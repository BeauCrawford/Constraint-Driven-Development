# Step 11 - Publish Constraint Set

---

## Description

Step 11, Publish Constraint Set, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_PUBLICATION_REQUIRED**
The authoritative constraint set must be published before test generation begins.

**CDD_P04_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve executable rule authority through the published constraint set.

**CDD_P04_PUBLICATION_CONTENT_COMPLETE**
Publication must include constraint statements, CONSTRAINT_IDs, invariant mappings, positive/negative/boundary cases, failure semantics, consistency report, gaps, and governed exceptions.

**CDD_P04_PUBLICATION_ACCESSIBILITY**
Published constraints must be accessible to downstream actors and tools that perform test generation.

**CDD_P04_PUBLICATION_VERSION_VISIBILITY**
The published constraint set must expose its version, baseline identity, or revision state.

**CDD_P04_PUBLICATION_NO_ORPHAN_CONSTRAINTS**
No published constraint may lack invariant lineage or governance status.

**CDD_P04_PUBLICATION_EXECUTION_AUTHORITY_BOUNDARY**
Published constraints define the first executable authority boundary for downstream tests and implementation.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Publish Constraint Set, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Publish Constraint Set.

**Invariants:** See step invariants above.

**Prompts**
- Publish Constraint Set Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Publish Constraint Set Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Publish Constraint Set
*Execute Publish Constraint Set with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Publish Constraint Set while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Publish Constraint Set with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Publish Constraint Set Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Publish Constraint Set Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Publish Constraint Set.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Publish Constraint Set Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Publish Constraint Set Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
