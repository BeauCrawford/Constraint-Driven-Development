# Step 10 - Refine Invariants

---

## Description

Step 10, Refine Invariants, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_REFINEMENT_ONLY**
Invariant refinement must repair closure issues without adding unauthorized meaning.

**CDD_P03_REFINEMENT_GAP_CLOSURE**
Refinement must address recorded gaps, additions, or drift through traceable changes.

**CDD_P03_REFINEMENT_UPSTREAM_ESCALATION**
Issues caused by requirement ambiguity or contradiction must be escalated upstream rather than patched as invariant invention.

**CDD_P03_REFINEMENT_REVALIDATION_REQUIRED**
Any invariant refinement must trigger closure revalidation.

**CDD_P03_REFINEMENT_TRACE_PRESERVATION**
Refinement must preserve requirement-to-invariant lineage and decision history.

**CDD_P03_REFINEMENT_NO_UNREVIEWED_AUTHORITY**
Refined invariants must not gain authority until closure evidence and review are updated.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Refine Invariants, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Refine Invariants.

**Invariants:** See step invariants above.

**Prompts**
- Refine Invariants Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Refine Invariants Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Refine Invariants
*Execute Refine Invariants with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Refine Invariants while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Refine Invariants with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Refine Invariants Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Refine Invariants Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Refine Invariants.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Refine Invariants Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Refine Invariants Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
