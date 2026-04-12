# Step 02 - Load Invariant Mappings

---

## Description

Step 02, Load Invariant Mappings, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_REQUIREMENT_TO_INVARIANT_MAPPING_REQUIRED**
Requirement-to-invariant mappings must be loaded.

**CDD_P09_INVARIANT_BASELINE_VISIBLE**
The invariant baseline version, publication identity, or revision state must be visible.

**CDD_P09_INVARIANT_LINEAGE_COMPLETE**
Every invariant must map to one or more requirements or a governed exception.

**CDD_P09_REQUIREMENT_INVARIANT_GAP_VISIBILITY**
Requirements without invariant representation must be recorded as gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Invariant Mappings, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Invariant Mappings.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariant Mappings Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Invariant Mappings Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Invariant Mappings
*Execute Load Invariant Mappings with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Invariant Mappings while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Invariant Mappings with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariant Mappings Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Invariant Mappings Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Invariant Mappings.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariant Mappings Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Invariant Mappings Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
