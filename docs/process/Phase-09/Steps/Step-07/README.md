# Step 07 - Validate Reverse Navigation

---

## Description

Step 07, Validate Reverse Navigation, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_REVERSE_NAVIGATION_REQUIRED**
Reverse navigation from failures or code artifacts to upstream intent must be validated.

**CDD_P09_REVERSE_FAILURE_EXPLAINABILITY**
Any failed test or behavior-bearing code path must trace back to governing constraints and requirements.

**CDD_P09_REVERSE_NO_AMBIGUOUS_PARENTAGE**
Artifacts must not have ambiguous or unverifiable upstream parentage.

**CDD_P09_REVERSE_EVIDENCE_REQUIRED**
Reverse navigation validation must produce reviewable evidence.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Validate Reverse Navigation, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Validate Reverse Navigation.

**Invariants:** See step invariants above.

**Prompts**
- Validate Reverse Navigation Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Validate Reverse Navigation Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Validate Reverse Navigation
*Execute Validate Reverse Navigation with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Validate Reverse Navigation while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Validate Reverse Navigation with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Validate Reverse Navigation Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Validate Reverse Navigation Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Validate Reverse Navigation.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Validate Reverse Navigation Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Validate Reverse Navigation Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.