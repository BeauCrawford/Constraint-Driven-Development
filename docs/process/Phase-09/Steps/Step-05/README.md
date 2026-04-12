# Step 05 - Load Code Mappings

---

## Description

Step 05, Load Code Mappings, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_TEST_TO_CODE_MAPPING_REQUIRED**
Test-to-code or proof-to-implementation mappings must be loaded.

**CDD_P09_IMPLEMENTATION_BASELINE_VISIBLE**
The implementation baseline version, publication identity, or revision state must be visible.

**CDD_P09_CODE_LINEAGE_COMPLETE**
Every behavior-bearing code artifact must map to proof.

**CDD_P09_CODE_MAPPING_GAP_VISIBILITY**
Code without proof lineage must be recorded as an orphan candidate.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Code Mappings, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Code Mappings.

**Invariants:** See step invariants above.

**Prompts**
- Load Code Mappings Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Code Mappings Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Code Mappings
*Execute Load Code Mappings with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Code Mappings while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Code Mappings with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Code Mappings Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Code Mappings Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Code Mappings.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Code Mappings Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Code Mappings Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
