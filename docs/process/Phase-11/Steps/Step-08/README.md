# Step 08 - Detect Stale Artifacts and Drift

---

## Description

Step 08, Detect Stale Artifacts and Drift, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_STALE_ARTIFACT_DETECTION_REQUIRED**
Phase 11 must detect artifacts whose upstream authority changed without regeneration.

**CDD_P11_NO_STALE_ARTIFACT_AUTHORITY**
Stale artifacts must not retain execution or proof authority.

**CDD_P11_DRIFT_DETECTION_REQUIRED**
Semantic drift introduced or exposed by change must be detected.

**CDD_P11_DRIFT_RESOLUTION_REQUIRED**
Unresolved drift blocks change completion.

**CDD_P11_OBSOLETE_ARTIFACT_VISIBILITY**
Retired or superseded artifacts must be marked and traceable.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Stale Artifacts and Drift, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Stale Artifacts and Drift.

**Invariants:** See step invariants above.

**Prompts**
- Detect Stale Artifacts and Drift Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Stale Artifacts and Drift Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Stale Artifacts and Drift
*Execute Detect Stale Artifacts and Drift with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Stale Artifacts and Drift while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Stale Artifacts and Drift with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Stale Artifacts and Drift Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Stale Artifacts and Drift Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Stale Artifacts and Drift.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Stale Artifacts and Drift Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Stale Artifacts and Drift Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.