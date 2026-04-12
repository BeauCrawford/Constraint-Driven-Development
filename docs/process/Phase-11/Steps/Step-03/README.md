# Step 03 - Update Upstream Source

---

## Description

Step 03, Update Upstream Source, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_UPSTREAM_UPDATE_REQUIRED**
Behavioral change must originate in requirements, invariants, glossary, or another governing upstream artifact.

**CDD_P11_INTENT_PRECEDENCE**
Updated upstream intent governs all downstream regeneration.

**CDD_P11_NO_DOWNSTREAM_FIRST_CHANGE**
Constraints, tests, contracts, or code must not be patched first to create new authority.

**CDD_P11_UPSTREAM_CHANGE_TRACEABILITY**
Upstream changes must retain lineage to the change request and affected artifacts.

**CDD_P11_UPSTREAM_CONFLICT_VISIBILITY**
Conflicts introduced by upstream change must be detected and governed.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Update Upstream Source, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Update Upstream Source.

**Invariants:** See step invariants above.

**Prompts**
- Update Upstream Source Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Update Upstream Source Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Update Upstream Source
*Execute Update Upstream Source with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Update Upstream Source while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Update Upstream Source with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Update Upstream Source Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Update Upstream Source Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Update Upstream Source.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Update Upstream Source Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Update Upstream Source Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
