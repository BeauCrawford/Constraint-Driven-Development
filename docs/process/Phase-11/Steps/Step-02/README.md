# Step 02 - Classify Impact

---

## Description

Step 02, Classify Impact, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_IMPACT_CLASSIFICATION_REQUIRED**
Each change must be classified by the upstream layer it affects.

**CDD_P11_REVERSE_NAVIGATION_REQUIRED**
Traceability must be used to locate impacted upstream and downstream artifacts.

**CDD_P11_GLOSSARY_IMPACT_VISIBILITY**
Term changes must identify impacted requirements, invariants, constraints, tests, contracts, and code.

**CDD_P11_IMPACT_PATH_COMPLETENESS**
Impact classification must include all affected lineage paths or record gaps.

**CDD_P11_AMBIGUOUS_IMPACT_BLOCKS_PATCHING**
Ambiguous impact must block downstream patching until clarified.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Classify Impact, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Classify Impact.

**Invariants:** See step invariants above.

**Prompts**
- Classify Impact Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Classify Impact Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Classify Impact
*Execute Classify Impact with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Classify Impact while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Classify Impact with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Classify Impact Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Classify Impact Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Classify Impact.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Classify Impact Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Classify Impact Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
