# Step 05 - Map Constraints to Interactions

---

## Description

Step 05, Map Constraints to Interactions, performs its Phase 05 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P05_CONSTRAINT_INTERACTION_MAPPING_REQUIRED**
Each boundary interaction must map to the constraints that govern it.

**CDD_P05_CONSTRAINT_COVERAGE_BY_CONTRACTS**
Every constraint with boundary impact must be represented by one or more contract interactions or a governed exception.

**CDD_P05_CONTRACT_TO_CONSTRAINT_TRACEABILITY**
Every contract interaction must trace back to one or more constraints.

**CDD_P05_DEPENDENCY_EXPLICITNESS**
Dependencies required by interactions must be visible at the contract level.

**CDD_P05_MAPPING_NO_ORPHAN_INTERACTIONS**
No contract interaction may exist without constraint lineage.

**CDD_P05_MAPPING_GAP_VISIBILITY**
Unmapped constraints and ungoverned interactions must be recorded as gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Map Constraints to Interactions, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 05 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Map Constraints to Interactions.

**Invariants:** See step invariants above.

**Prompts**
- Map Constraints to Interactions Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Map Constraints to Interactions Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Map Constraints to Interactions
*Execute Map Constraints to Interactions with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Map Constraints to Interactions while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Map Constraints to Interactions with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Map Constraints to Interactions Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Map Constraints to Interactions Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Map Constraints to Interactions.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Map Constraints to Interactions Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Map Constraints to Interactions Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
