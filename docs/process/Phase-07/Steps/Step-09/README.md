# Step 09 - Evaluate Failure Semantics

---

## Description

Step 09, Evaluate Failure Semantics, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_FAILURE_EVALUATION_REQUIRED**
Failure-path tests must be evaluated against the simulated boundaries.

**CDD_P07_FAILURE_BEHAVIOR_CONFIRMED**
Simulation must produce governed failure behavior as contracts and constraints define.

**CDD_P07_FAILURE_RESULT_TRACEABILITY**
Failure results must trace to tests, constraints, and contract interactions.

**CDD_P07_FAILURE_NO_INVENTED_FAILURE**
Simulation must not introduce failure modes absent from governing artifacts.

**CDD_P07_FAILURE_GAP_VISIBILITY**
Missing or inconclusive failure evaluation must be recorded as a validation gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Evaluate Failure Semantics, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Evaluate Failure Semantics.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Failure Semantics Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Evaluate Failure Semantics Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Evaluate Failure Semantics
*Execute Evaluate Failure Semantics with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Evaluate Failure Semantics while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Evaluate Failure Semantics with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Failure Semantics Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Evaluate Failure Semantics Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Evaluate Failure Semantics.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Evaluate Failure Semantics Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Evaluate Failure Semantics Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.