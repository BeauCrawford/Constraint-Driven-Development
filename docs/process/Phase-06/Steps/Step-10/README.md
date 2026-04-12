# Step 10 - Compute Coverage

---

## Description

Step 10, Compute Coverage, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_COVERAGE_COMPUTATION_REQUIRED**
Constraint-level coverage must be computed before review.

**CDD_P06_COVERAGE_CONSTRAINT_COMPLETE**
Every constraint must have at least one mapped proof test or a governed exception.

**CDD_P06_COVERAGE_PNB_FAILURE_INCLUDED**
Coverage must include positive, negative, boundary, and failure semantics where applicable.

**CDD_P06_COVERAGE_ID_LINKED**
Coverage evidence must be linked to CONSTRAINT_IDs.

**CDD_P06_COVERAGE_SEMANTIC_NOT_LINE_BASED**
Coverage must be measured against constraint semantics, not source lines.

**CDD_P06_COVERAGE_GAP_VISIBILITY**
Coverage gaps must be recorded with affected CONSTRAINT_IDs.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Compute Coverage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Compute Coverage.

**Invariants:** See step invariants above.

**Prompts**
- Compute Coverage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Compute Coverage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Compute Coverage
*Execute Compute Coverage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Compute Coverage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Compute Coverage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Compute Coverage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Compute Coverage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Compute Coverage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Compute Coverage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Compute Coverage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.