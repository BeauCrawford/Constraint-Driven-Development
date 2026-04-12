# Step 03 - Align Terminology

---

## Description

Step 03, Align Terminology, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_GLOSSARY_ALIGNMENT_REQUIRED**
Requirements and invariants must be aligned through the canonical glossary before comparison.

**CDD_P03_GLOSSARY_SHARED_REFERENCE_FRAME**
The same glossary meaning must govern both parent requirement terms and child invariant terms.

**CDD_P03_GLOSSARY_SYNONYM_NORMALIZATION**
Synonymous terms must be normalized before semantic comparison.

**CDD_P03_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms in either layer must block closure approval unless resolved or explicitly excepted.

**CDD_P03_GLOSSARY_TERM_DRIFT_VISIBILITY**
Any term meaning mismatch across requirements and invariants must be recorded as drift.

**CDD_P03_GLOSSARY_SCOPE_SENSITIVITY**
Term alignment must preserve scoped definitions, exclusions, and domain boundaries.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Align Terminology, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Align Terminology.

**Invariants:** See step invariants above.

**Prompts**
- Align Terminology Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Align Terminology Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Align Terminology
*Execute Align Terminology with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Align Terminology while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Align Terminology with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Align Terminology Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Align Terminology Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Align Terminology.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Align Terminology Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Align Terminology Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
