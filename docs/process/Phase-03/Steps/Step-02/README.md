# Step 02 - Load Invariants

---

## Description

Step 02, Load Invariants, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_INVARIANT_SET_REQUIRED**
Phase 03 must load the finalized Phase 02 invariant set as the candidate child representation.

**CDD_P03_INVARIANT_BASELINE_IDENTITY_VISIBLE**
The loaded invariant set must expose its version, publication identity, or revision state.

**CDD_P03_INVARIANT_REQUIREMENT_LINEAGE_VISIBLE**
Every loaded invariant must expose its requirement lineage.

**CDD_P03_INVARIANT_NEGATIVE_SPACE_VISIBLE**
Negative-space definitions from Phase 02 must be included in closure validation.

**CDD_P03_INVARIANT_NO_CANDIDATE_AUTHORITY**
Unfinalized invariant candidates must not be treated as closure-ready truth unless explicitly excepted.

**CDD_P03_INVARIANT_INPUT_DEFECT_ESCALATION**
Missing lineage, unresolved conflicts, or incomplete invariant records must be recorded as Phase 02 defects.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Load Invariants, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Load Invariants.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariants Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Load Invariants Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Load Invariants
*Execute Load Invariants with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Load Invariants while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Load Invariants with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariants Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Load Invariants Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Load Invariants.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Load Invariants Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Load Invariants Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
