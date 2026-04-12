# Step 04 - Define Contract Interfaces

---

## Description

Step 04, Define Contract Interfaces, performs its Phase 05 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P05_CONTRACT_DEFINITION_REQUIRED**
Each governed boundary must have an explicit contract definition.

**CDD_P05_CONTRACT_SEMANTIC_CARRIER**
Contracts must encode interaction semantics, not merely type shapes.

**CDD_P05_CONTRACT_IMPLEMENTATION_SEPARATION**
Contracts must be isolated from implementation decisions and concrete provider behavior.

**CDD_P05_CONTRACT_OPERATION_EXPLICITNESS**
Operations, messages, events, inputs, outputs, states, and obligations must be explicit where applicable.

**CDD_P05_CONTRACT_PRE_POST_CONDITION_VISIBILITY**
Preconditions, postconditions, invariants, and state transition expectations must be explicit when they affect behavior.

**CDD_P05_CONTRACT_REPLACEABILITY**
Contracts must allow conforming real implementations and test doubles to be substitutable.

**CDD_P05_CONTRACT_NO_UNAUTHORIZED_BEHAVIOR**
Contract definitions must not introduce behavior beyond constraint authority.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Define Contract Interfaces, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 05 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Define Contract Interfaces.

**Invariants:** See step invariants above.

**Prompts**
- Define Contract Interfaces Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Define Contract Interfaces Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Define Contract Interfaces
*Execute Define Contract Interfaces with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Define Contract Interfaces while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Define Contract Interfaces with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Define Contract Interfaces Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Define Contract Interfaces Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Define Contract Interfaces.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Define Contract Interfaces Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Define Contract Interfaces Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
