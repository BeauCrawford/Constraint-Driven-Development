# Step 04 - Re-Lower Affected Artifacts

---

## Description

Step 04, Re-Lower Affected Artifacts, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_RELOWERING_REQUIRED**
Affected artifacts must be re-lowered through the CDD pipeline.

**CDD_P11_MONOTONIC_RELOWERING**
Re-lowering must refine upstream meaning without expansion or invention.

**CDD_P11_NO_LAYER_SKIP**
Change propagation must not skip required intermediate layers.

**CDD_P11_RELOWERING_TRACEABILITY**
Each re-lowered artifact must retain lineage to the changed upstream source.

**CDD_P11_RELOWERING_GAP_VISIBILITY**
Artifacts that cannot be re-lowered cleanly must be recorded as gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Re-Lower Affected Artifacts, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Re-Lower Affected Artifacts.

**Invariants:** See step invariants above.

**Prompts**
- Re-Lower Affected Artifacts Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Re-Lower Affected Artifacts Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Re-Lower Affected Artifacts
*Execute Re-Lower Affected Artifacts with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Re-Lower Affected Artifacts while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Re-Lower Affected Artifacts with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Re-Lower Affected Artifacts Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Re-Lower Affected Artifacts Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Re-Lower Affected Artifacts.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Re-Lower Affected Artifacts Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Re-Lower Affected Artifacts Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.