# Step 06 - Encode Edge and Failure Behavior

---

## Description

Step 06, Encode Edge and Failure Behavior, performs its Phase 05 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P05_EDGE_FAILURE_REQUIRED**
Contracts must encode relevant edge and failure behavior.

**CDD_P05_BOUNDARY_CONDITION_ALIGNMENT**
Edge and failure interactions must align with constraint boundary and failure semantics.

**CDD_P05_FAILURE_MODE_EXPLICITNESS**
Failure modes, invalid inputs, unavailable dependencies, rejected states, and recovery expectations must be explicit where governed.

**CDD_P05_EDGE_CASE_TRACEABILITY**
Each edge or failure behavior must trace to its governing constraints.

**CDD_P05_EDGE_FAILURE_NO_INVENTION**
Edge and failure behavior must not introduce semantics absent from constraints.

**CDD_P05_TEST_DOUBLE_READINESS**
Edge and failure behavior must be precise enough for later deterministic test doubles.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Encode Edge and Failure Behavior, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 05 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Encode Edge and Failure Behavior.

**Invariants:** See step invariants above.

**Prompts**
- Encode Edge and Failure Behavior Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Encode Edge and Failure Behavior Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Encode Edge and Failure Behavior
*Execute Encode Edge and Failure Behavior with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Encode Edge and Failure Behavior while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Encode Edge and Failure Behavior with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Encode Edge and Failure Behavior Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Encode Edge and Failure Behavior Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Encode Edge and Failure Behavior.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Encode Edge and Failure Behavior Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Encode Edge and Failure Behavior Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
