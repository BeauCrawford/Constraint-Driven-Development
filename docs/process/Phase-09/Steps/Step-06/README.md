# Step 06 - Validate Forward Lineage

---

## Description

Step 06, Validate Forward Lineage, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_FORWARD_LINEAGE_REQUIRED**
Forward lineage from requirement to implementation must be validated.

**CDD_P09_FORWARD_REQUIREMENT_COVERAGE**
Every requirement must navigate downstream through invariants, constraints, tests, and code or governed exception.

**CDD_P09_FORWARD_NO_BROKEN_LINKS**
Lineage links must not terminate unexpectedly before the appropriate downstream layer.

**CDD_P09_FORWARD_EVIDENCE_REQUIRED**
Forward lineage validation must produce reviewable evidence.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Validate Forward Lineage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Validate Forward Lineage.

**Invariants:** See step invariants above.

**Prompts**
- Validate Forward Lineage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Validate Forward Lineage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Validate Forward Lineage
*Execute Validate Forward Lineage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Validate Forward Lineage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Validate Forward Lineage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Validate Forward Lineage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Validate Forward Lineage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Validate Forward Lineage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Validate Forward Lineage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Validate Forward Lineage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.