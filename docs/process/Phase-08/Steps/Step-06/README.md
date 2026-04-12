# Step 06 - Evaluate Defined Behavior

---

## Description

Step 06, Evaluate Defined Behavior, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_DEFINED_BEHAVIOR_EVALUATION_REQUIRED**
Allowed, forbidden, boundary, and failure behavior must be evaluated against the real implementation.

**CDD_P08_POSITIVE_BEHAVIOR_CONFIRMED**
Implementation must admit behavior required or allowed by constraints.

**CDD_P08_NEGATIVE_BEHAVIOR_REJECTED**
Implementation must reject behavior forbidden by constraints.

**CDD_P08_BOUNDARY_BEHAVIOR_CONFIRMED**
Implementation must handle governed edge conditions as specified.

**CDD_P08_FAILURE_BEHAVIOR_CONFIRMED**
Implementation must manifest governed failure semantics as specified.

**CDD_P08_DEFINED_BEHAVIOR_TRACEABILITY**
Evaluation evidence must trace to tests, constraints, contracts, and code artifacts.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Evaluate Defined Behavior, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Evaluate Defined Behavior.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Defined Behavior Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Evaluate Defined Behavior Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Evaluate Defined Behavior
*Execute Evaluate Defined Behavior with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Evaluate Defined Behavior while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Evaluate Defined Behavior with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Defined Behavior Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Evaluate Defined Behavior Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Evaluate Defined Behavior.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Defined Behavior Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Evaluate Defined Behavior Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
