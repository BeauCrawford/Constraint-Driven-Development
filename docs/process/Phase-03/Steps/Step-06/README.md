# Step 06 - Detect Unauthorized Additions

---

## Description

Step 06, Detect Unauthorized Additions, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_ADDITION_DETECTION_REQUIRED**
Phase 03 must detect invariant meaning not authorized by parent requirements.

**CDD_P03_ADDITION_INVARIANT_LINEAGE**
Each unauthorized addition candidate must identify the affected invariant IDs or statements and missing parent authority.

**CDD_P03_ADDITION_NO_SILENT_EXPANSION**
Invariant meaning must not broaden parent intent without visible governance.

**CDD_P03_ADDITION_GLOSSARY_LIMIT**
Glossary meaning may clarify terms but must not authorize new system behavior absent from requirements.

**CDD_P03_ADDITION_RESOLUTION_PATH**
Each addition must be removed, traced to valid parent intent, escalated upstream, or recorded as an exception.

**CDD_P03_ADDITION_BLOCKS_CLOSURE**
Unresolved unauthorized additions block closure approval.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Unauthorized Additions, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Unauthorized Additions.

**Invariants:** See step invariants above.

**Prompts**
- Detect Unauthorized Additions Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Unauthorized Additions Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Unauthorized Additions
*Execute Detect Unauthorized Additions with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Unauthorized Additions while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Unauthorized Additions with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Unauthorized Additions Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Unauthorized Additions Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Unauthorized Additions.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Unauthorized Additions Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Unauthorized Additions Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
