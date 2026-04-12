# Step 03 - Identify Boundaries

---

## Description

Step 03, Identify Boundaries, performs its Phase 05 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P05_BOUNDARY_IDENTIFICATION_REQUIRED**
All system interaction points implied by the constraint set must be identified.

**CDD_P05_BOUNDARY_FIRSTNESS**
Boundary identification must precede implementation or test double construction.

**CDD_P05_BOUNDARY_CONSTRAINT_LINEAGE**
Each identified boundary must link to the constraints that require or govern it.

**CDD_P05_BOUNDARY_ACTOR_VISIBILITY**
Actors, components, external systems, data sources, and consumers at each boundary must be explicit.

**CDD_P05_BOUNDARY_DIRECTION_VISIBILITY**
Input, output, bidirectional, event, request, response, and dependency directions must be explicit where relevant.

**CDD_P05_BOUNDARY_SCOPE_ALIGNMENT**
Boundaries must remain within the scope authorized by requirements, invariants, and constraints.

**CDD_P05_BOUNDARY_GAP_VISIBILITY**
Potential interactions that cannot be classified must be recorded as boundary gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Identify Boundaries, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 05 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Identify Boundaries.

**Invariants:** See step invariants above.

**Prompts**
- Identify Boundaries Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Identify Boundaries Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Identify Boundaries
*Execute Identify Boundaries with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Identify Boundaries while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Identify Boundaries with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Identify Boundaries Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Identify Boundaries Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Identify Boundaries.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Identify Boundaries Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Identify Boundaries Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
