# Step 10 - Record Results & Coverage

---

## Description

Step 10, Record Results & Coverage, performs its Phase 07 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P07_RESULT_RECORDING_REQUIRED**
Simulation results and coverage evidence must be recorded.

**CDD_P07_RESULT_CONSTRAINT_LINKAGE**
Results must remain linked to CONSTRAINT_IDs.

**CDD_P07_RESULT_CONTRACT_LINKAGE**
Results must remain linked to contract interactions and doubles.

**CDD_P07_COVERAGE_INTERACTION_INCLUDED**
Coverage evidence must include boundary interaction coverage where applicable.

**CDD_P07_COVERAGE_FAILURE_INCLUDED**
Coverage evidence must include governed failure-mode verification.

**CDD_P07_RESULT_NO_ORPHANS**
No recorded validation result may lack test, constraint, or contract lineage.

**CDD_P07_RESULT_GAP_VISIBILITY**
Skipped tests, uncovered interactions, flakes, failures, and exceptions must be recorded as visible gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Record Results & Coverage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 07 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Record Results & Coverage.

**Invariants:** See step invariants above.

**Prompts**
- Record Results & Coverage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Record Results & Coverage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Record Results & Coverage
*Execute Record Results & Coverage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Record Results & Coverage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Record Results & Coverage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Record Results & Coverage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Record Results & Coverage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Record Results & Coverage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Record Results & Coverage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Record Results & Coverage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
