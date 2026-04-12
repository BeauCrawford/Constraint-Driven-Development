# Step 01 - Provide Proof Suite

---

## Description

Step 01, Provide Proof Suite, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_PROOF_SUITE_SOURCE_REQUIRED**
Phase 08 must load the published Phase 06 proof suite as the implementation target.

**CDD_P08_PROOF_SUITE_BASELINE_VISIBLE**
The proof suite baseline version, publication identity, or revision state must be visible.

**CDD_P08_PROOF_CONSTRAINT_MAPPING_VISIBLE**
Test-to-CONSTRAINT_ID mappings must remain visible during implementation.

**CDD_P08_SIMULATION_VALIDATION_REQUIRED**
The Phase 07 validation report must be available before real implementation authority is claimed.

**CDD_P08_PROOF_NO_INFORMAL_AUTHORITY**
Manual expectations, exploratory checks, or unpublished tests must not authorize implementation behavior.

**CDD_P08_PROOF_INPUT_DEFECT_ESCALATION**
Missing proof mappings, nondeterministic tests, or failed simulation evidence must be escalated upstream rather than patched in code.

---

## Substeps

### 🟦 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Provide Proof Suite, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Provide Proof Suite.

**Invariants:** See step invariants above.

**Prompts**
- Provide Proof Suite Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Provide Proof Suite Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Provide Proof Suite
*Execute Provide Proof Suite with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Provide Proof Suite while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Provide Proof Suite with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Provide Proof Suite Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Provide Proof Suite Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟦 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Provide Proof Suite.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Provide Proof Suite Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Provide Proof Suite Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.