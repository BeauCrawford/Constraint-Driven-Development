# Step 04 - Register Doubles

---

## Description

Step 04, Register Doubles, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_DOUBLE_REGISTRATION_REQUIRED**
Generated doubles must be registered in the execution environment before test execution.

**CDD_P07_DOUBLE_BOUNDARY_ISOLATION**
Registration must isolate boundary behavior through the configured doubles.

**CDD_P07_DOUBLE_BINDING_VISIBILITY**
The mapping between tests, contracts, and registered doubles must be visible.

**CDD_P07_DOUBLE_NO_HIDDEN_REAL_DEPENDENCIES**
Simulation must not accidentally call real external dependencies or hidden side channels.

**CDD_P07_DOUBLE_REGISTRATION_DETERMINISM**
Double registration and lifecycle setup must be deterministic and reproducible.

**CDD_P07_DOUBLE_REGISTRATION_GAP_VISIBILITY**
Missing or ambiguous double bindings must be recorded as validation gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Register Doubles, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Register Doubles.

**Invariants:** See step invariants above.

**Prompts**
- Register Doubles Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Register Doubles Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Register Doubles
*Execute Register Doubles with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Register Doubles while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Register Doubles with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Register Doubles Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Register Doubles Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Register Doubles.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Register Doubles Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Register Doubles Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
