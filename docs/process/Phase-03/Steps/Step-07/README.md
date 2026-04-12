# Step 07 - Detect Drift

---

## Description

Step 07, Detect Drift, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_DRIFT_DETECTION_REQUIRED**
Phase 03 must detect distorted, weakened, strengthened, or shifted meaning between requirements and invariants.

**CDD_P03_DRIFT_CONTAINMENT_FAILURE**
Drift must be treated as loss of semantic containment.

**CDD_P03_DRIFT_REQUIREMENT_INVARIANT_TRACE**
Each drift record must link the affected requirement meaning and invariant meaning.

**CDD_P03_DRIFT_MODALITY_PRESERVATION**
Changes to required, forbidden, optional, or conditional modality must be detected as drift.

**CDD_P03_DRIFT_SCOPE_PRESERVATION**
Changes to scope boundaries, actors, conditions, outcomes, or negative space must be detected as drift.

**CDD_P03_DRIFT_RESOLUTION_REQUIRED**
Unresolved drift blocks closure approval.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Detect Drift, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Detect Drift.

**Invariants:** See step invariants above.

**Prompts**
- Detect Drift Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Detect Drift Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Detect Drift
*Execute Detect Drift with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Detect Drift while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Detect Drift with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Detect Drift Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Detect Drift Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Detect Drift.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Detect Drift Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Detect Drift Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
