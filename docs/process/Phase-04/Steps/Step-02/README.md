# Step 02 - Resolve Terminology

---

## Description

Step 02, Resolve Terminology, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_GLOSSARY_ALIGNMENT_REQUIRED**
Constraint language must align with canonical glossary terms used by the validated invariants.

**CDD_P04_GLOSSARY_MEANING_PRESERVATION**
Constraint wording must preserve invariant meaning and glossary definitions.

**CDD_P04_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms must block constraint publication unless resolved or explicitly excepted.

**CDD_P04_GLOSSARY_NO_TERM_INVENTION**
Constraint derivation must not introduce new domain terminology without glossary grounding.

**CDD_P04_GLOSSARY_EXECUTION_TERM_BOUNDARY**
Executable precision may add operational structure but must not change domain meaning.

**CDD_P04_GLOSSARY_DRIFT_VISIBILITY**
Any term meaning shift between invariants and constraints must be recorded as drift.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Resolve Terminology, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Resolve Terminology.

**Invariants:** See step invariants above.

**Prompts**
- Resolve Terminology Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Resolve Terminology Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Resolve Terminology
*Execute Resolve Terminology with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Resolve Terminology while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Resolve Terminology with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Resolve Terminology Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Resolve Terminology Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Resolve Terminology.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Resolve Terminology Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Resolve Terminology Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
