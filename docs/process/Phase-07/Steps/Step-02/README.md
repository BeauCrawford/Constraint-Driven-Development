# Step 02 - Provide Contracts

---

## Description

Step 02, Provide Contracts, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_CONTRACT_SOURCE_REQUIRED**
Phase 07 must load the published Phase 05 contract set as the boundary authority for doubles.

**CDD_P07_CONTRACT_BASELINE_VISIBLE**
The contract baseline version, publication identity, or revision state must be visible.

**CDD_P07_CONTRACT_SEMANTIC_AVAILABILITY**
Contract operations, interactions, edge behavior, and failure semantics must be available for double generation.

**CDD_P07_CONTRACT_CONSTRAINT_LINEAGE_VISIBLE**
Contract-to-constraint mappings must remain visible during validation.

**CDD_P07_CONTRACT_NO_UNPUBLISHED_AUTHORITY**
Unpublished contracts or informal interface assumptions must not authorize test doubles.

**CDD_P07_CONTRACT_INPUT_DEFECT_ESCALATION**
Missing contract semantics, side channels, or unresolved boundary gaps must be escalated upstream.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Provide Contracts, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Provide Contracts.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contracts Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Provide Contracts Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Provide Contracts
*Execute Provide Contracts with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Provide Contracts while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Provide Contracts with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contracts Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Provide Contracts Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Provide Contracts.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Provide Contracts Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Provide Contracts Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
