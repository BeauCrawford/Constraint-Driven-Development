# Step 06 - Evaluate Positive Behavior

---

## Description

Step 06, Evaluate Positive Behavior, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_POSITIVE_EVALUATION_REQUIRED**
Positive behavior tests must be evaluated against the simulated boundaries.

**CDD_P07_POSITIVE_ALLOWED_BEHAVIOR_CONFIRMED**
Simulation must admit behavior that constraints and contracts allow.

**CDD_P07_POSITIVE_RESULT_TRACEABILITY**
Positive results must trace to tests, constraints, and contract interactions.

**CDD_P07_POSITIVE_NO_OVERACCEPTANCE**
Passing positive tests must not mask acceptance of behavior outside constraints.

**CDD_P07_POSITIVE_GAP_VISIBILITY**
Missing or inconclusive positive evaluation must be recorded as a validation gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Evaluate Positive Behavior, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Evaluate Positive Behavior.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Positive Behavior Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Evaluate Positive Behavior Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Evaluate Positive Behavior
*Execute Evaluate Positive Behavior with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Evaluate Positive Behavior while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Evaluate Positive Behavior with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Positive Behavior Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Evaluate Positive Behavior Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Evaluate Positive Behavior.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Positive Behavior Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Evaluate Positive Behavior Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
