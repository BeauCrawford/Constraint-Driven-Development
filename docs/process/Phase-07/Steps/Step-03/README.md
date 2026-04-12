# Step 03 - Generate Test Doubles

---

## Description

Step 03, Generate Test Doubles, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_DOUBLE_GENERATION_REQUIRED**
Contract-bound test doubles must be generated or defined for simulated boundary behavior required by the tests.

**CDD_P07_DOUBLE_CONTRACT_BOUND**
Each test double must derive from and conform to a published contract.

**CDD_P07_DOUBLE_NO_SEMANTIC_INVENTION**
Test doubles must not introduce behavior absent from contracts, constraints, or tests.

**CDD_P07_DOUBLE_DETERMINISTIC_BEHAVIOR**
Test doubles must behave deterministically for the same inputs and controlled state.

**CDD_P07_DOUBLE_FAILURE_MODELING**
Test doubles must model governed failure conditions where required by contracts and tests.

**CDD_P07_DOUBLE_REPLACEABILITY**
Doubles must preserve substitutability with future real implementations under the same contracts.

**CDD_P07_DOUBLE_TRACEABILITY**
Each double behavior must trace to contract interactions and governing constraints.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Generate Test Doubles, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Generate Test Doubles.

**Invariants:** See step invariants above.

**Prompts**
- Generate Test Doubles Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Generate Test Doubles Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Generate Test Doubles
*Execute Generate Test Doubles with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Generate Test Doubles while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Generate Test Doubles with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Generate Test Doubles Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Generate Test Doubles Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Generate Test Doubles.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Generate Test Doubles Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Generate Test Doubles Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
