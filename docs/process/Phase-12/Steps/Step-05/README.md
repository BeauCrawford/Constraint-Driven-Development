# Step 05 - Validate Entry and Exit Gates

---

## Description

Step 05, Validate Entry and Exit Gates, performs its Phase 12 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P12_GATE_VALIDATION_REQUIRED**
Entry and exit gates for applicable phases must be validated.

**CDD_P12_GATE_EVIDENCE_REQUIRED**
Gate status must be supported by phase evidence.

**CDD_P12_GATE_NO_LAYER_BYPASS**
Skipped phases or layer jumps must be explicitly governed.

**CDD_P12_GATE_FAILURE_BLOCKS_AUTHORITY**
Failed gates block release or require governed exception.

**CDD_P12_GATE_STATUS_TRACEABILITY**
Gate decisions must link to affected artifacts, evidence, owners, and exceptions.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Validate Entry and Exit Gates, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 12 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Validate Entry and Exit Gates.

**Invariants:** See step invariants above.

**Prompts**
- Validate Entry and Exit Gates Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Validate Entry and Exit Gates Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Validate Entry and Exit Gates
*Execute Validate Entry and Exit Gates with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Validate Entry and Exit Gates while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Validate Entry and Exit Gates with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Validate Entry and Exit Gates Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Validate Entry and Exit Gates Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Validate Entry and Exit Gates.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Validate Entry and Exit Gates Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Validate Entry and Exit Gates Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
