# Step 05 - Regenerate Constraints, Tests, and Code

---

## Description

Step 05, Regenerate Constraints, Tests, and Code, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_REGENERATION_REQUIRED**
Affected constraints, contracts, tests, doubles, and code must be regenerated or reconformed from updated upstream authority.

**CDD_P11_REGENERATION_OVER_PATCHING**
Regeneration is preferred over manual downstream patching.

**CDD_P11_TEST_REGENERATION_REQUIRED**
Affected tests must be regenerated from updated constraints.

**CDD_P11_CODE_RECONFORMANCE_REQUIRED**
Affected code must be reconformed to regenerated proof.

**CDD_P11_REGENERATION_NO_STALE_AUTHORITY**
Old artifacts must not retain authority when their upstream lineage changed.

**CDD_P11_REGENERATION_EVIDENCE_REQUIRED**
Regeneration must produce evidence of affected artifacts and unchanged artifacts.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Regenerate Constraints, Tests, and Code, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Regenerate Constraints, Tests, and Code.

**Invariants:** See step invariants above.

**Prompts**
- Regenerate Constraints, Tests, and Code Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Regenerate Constraints, Tests, and Code Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Regenerate Constraints, Tests, and Code
*Execute Regenerate Constraints, Tests, and Code with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Regenerate Constraints, Tests, and Code while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Regenerate Constraints, Tests, and Code with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Regenerate Constraints, Tests, and Code Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Regenerate Constraints, Tests, and Code Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Regenerate Constraints, Tests, and Code.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Regenerate Constraints, Tests, and Code Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Regenerate Constraints, Tests, and Code Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.