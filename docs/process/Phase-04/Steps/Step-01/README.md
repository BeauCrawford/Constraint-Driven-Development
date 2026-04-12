# Step 01 - Load Validated Invariants

---

## Description

Step 01, Load Validated Invariants, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_VALIDATED_INVARIANT_SOURCE_REQUIRED**
Phase 04 must load only closure-validated invariants as its semantic source.

**CDD_P04_CLOSURE_REPORT_REQUIRED**
The closure report validating the invariant set must be available before derivation begins.

**CDD_P04_INVARIANT_BASELINE_IDENTITY_VISIBLE**
The invariant baseline version, publication identity, or revision state must be visible.

**CDD_P04_INVARIANT_LINEAGE_VISIBLE**
Requirement-to-invariant lineage must remain visible during constraint derivation.

**CDD_P04_INVARIANT_NO_UNVALIDATED_AUTHORITY**
Unvalidated invariant candidates must not grant constraint authority.

**CDD_P04_INVARIANT_INPUT_DEFECT_ESCALATION**
Missing closure evidence, missing lineage, or unresolved invariant defects must be escalated upstream rather than silently repaired in Phase 04.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Validated Invariants, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Validated Invariants.

**Invariants:** See step invariants above.

**Prompts**
- Load Validated Invariants Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Validated Invariants Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Validated Invariants
*Execute Load Validated Invariants with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Validated Invariants while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Validated Invariants with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Validated Invariants Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Validated Invariants Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Validated Invariants.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Validated Invariants Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Validated Invariants Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
