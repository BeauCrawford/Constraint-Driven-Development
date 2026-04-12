# Step 06 - Measure Constraint Coverage

---

## Description

Step 06, Measure Constraint Coverage, performs its Phase 10 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P10_COVERAGE_MEASUREMENT_REQUIRED**
Constraint-level semantic coverage must be measured after implementation proof.

**CDD_P10_COVERAGE_CONSTRAINT_COMPLETE**
Every constraint must have passing proof coverage or a governed exception.

**CDD_P10_COVERAGE_PNB_FAILURE_INCLUDED**
Coverage must include positive, negative, boundary, and failure semantics where applicable.

**CDD_P10_COVERAGE_ID_LINKED**
Coverage evidence must link to CONSTRAINT_IDs.

**CDD_P10_COVERAGE_NOT_LINE_BASED**
Coverage must be measured against semantics, not code lines.

**CDD_P10_COVERAGE_RECOMPUTABLE**
Coverage conclusions must be reproducible from traceability and test evidence.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Measure Constraint Coverage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 10 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Measure Constraint Coverage.

**Invariants:** See step invariants above.

**Prompts**
- Measure Constraint Coverage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Measure Constraint Coverage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Measure Constraint Coverage
*Execute Measure Constraint Coverage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Measure Constraint Coverage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Measure Constraint Coverage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Measure Constraint Coverage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Measure Constraint Coverage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Measure Constraint Coverage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Measure Constraint Coverage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Measure Constraint Coverage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.