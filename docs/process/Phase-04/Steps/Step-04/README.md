# Step 04 - Derive Constraint Candidates

---

## Description

Step 04, Derive Constraint Candidates, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_CONSTRAINT_DERIVATION_REQUIRED**
Each rule unit must be evaluated for constraint derivation.

**CDD_P04_CONSTRAINT_INVARIANT_AUTHORITY**
Every constraint candidate must derive from one or more validated invariants.

**CDD_P04_CONSTRAINT_EXECUTABLE_PRECISION**
Each constraint candidate must be precise enough to define enforceable behavior.

**CDD_P04_CONSTRAINT_NO_INVENTED_BEHAVIOR**
Constraint candidates must not introduce behavior beyond invariant authority.

**CDD_P04_CONSTRAINT_ALLOWED_FORBIDDEN_BOUNDARY_ORIENTATION**
Constraint candidates must orient toward allowed, forbidden, and boundary behavior.

**CDD_P04_CONSTRAINT_FAILURE_DETECTABILITY**
Constraint candidates must be capable of producing detectable pass or failure semantics downstream.

**CDD_P04_CONSTRAINT_TRACEABILITY**
Each constraint candidate must retain lineage to invariant IDs or statements and parent requirement IDs.

**CDD_P04_CONSTRAINT_REVIEWABILITY**
Constraint candidates must be inspectable before publication.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Derive Constraint Candidates, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Derive Constraint Candidates.

**Invariants:** See step invariants above.

**Prompts**
- Derive Constraint Candidates Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Derive Constraint Candidates Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Derive Constraint Candidates
*Execute Derive Constraint Candidates with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Derive Constraint Candidates while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Derive Constraint Candidates with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Derive Constraint Candidates Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Derive Constraint Candidates Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Derive Constraint Candidates.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Derive Constraint Candidates Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Derive Constraint Candidates Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
