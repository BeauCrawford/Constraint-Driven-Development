# Step 02 - Align Terminology

---

## Description

Step 02, Align Terminology, performs its Phase 06 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P06_GLOSSARY_ALIGNMENT_REQUIRED**
Test names, fixtures, cases, and assertions must align with canonical glossary terms.

**CDD_P06_GLOSSARY_MEANING_PRESERVATION**
Tests must preserve constraint and contract meanings.

**CDD_P06_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms must block authoritative test publication unless resolved or explicitly excepted.

**CDD_P06_GLOSSARY_NO_TEST_TERM_INVENTION**
Tests must not introduce new domain terminology without glossary grounding.

**CDD_P06_GLOSSARY_DRIFT_VISIBILITY**
Any term meaning shift between constraints, contracts, and tests must be recorded as drift.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Align Terminology, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 06 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

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