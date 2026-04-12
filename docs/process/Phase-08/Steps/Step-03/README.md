# Step 03 - Generate or Implement Minimal Code

---

## Description

Step 03, Generate or Implement Minimal Code, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_CODE_GENERATION_AUTHORITY**
Code may be generated or implemented only to satisfy published constraints, contracts, and proof.

**CDD_P08_CODE_AS_RESIDUE**
Implementation code must be the residual output of satisfied constraints and proof.

**CDD_P08_CODE_MINIMAL_FREEDOM**
Implementation must minimize interpretive freedom beyond the proof suite.

**CDD_P08_CODE_NO_UNPROVEN_BEHAVIOR**
Code must not introduce behavior outside the closed constraint system.

**CDD_P08_CODE_IMPLEMENTATION_DETAIL_BOUNDARY**
Implementation details may vary only where constraints and contracts leave replaceable freedom.

**CDD_P08_CODE_TRACEABILITY**
Code behavior must remain traceable to tests, constraints, contracts, invariants, and requirements.

**CDD_P08_CODE_GAP_VISIBILITY**
Any behavior needed to pass proof but not authorized upstream must be recorded as a semantic gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Generate or Implement Minimal Code, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Generate or Implement Minimal Code.

**Invariants:** See step invariants above.

**Prompts**
- Generate or Implement Minimal Code Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Generate or Implement Minimal Code Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Generate or Implement Minimal Code
*Execute Generate or Implement Minimal Code with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Generate or Implement Minimal Code while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Generate or Implement Minimal Code with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Generate or Implement Minimal Code Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Generate or Implement Minimal Code Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Generate or Implement Minimal Code.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Generate or Implement Minimal Code Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Generate or Implement Minimal Code Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.