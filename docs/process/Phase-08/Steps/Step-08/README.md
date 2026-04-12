# Step 08 - Reconform Implementation

---

## Description

Step 08, Reconform Implementation, performs its Phase 08 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P08_RECONFORMANCE_REQUIRED**
Implementation must be adjusted until it conforms to proof, contracts, and constraints.

**CDD_P08_RECONFORMANCE_CONSTRAINT_BOUND**
Reconformance changes must stay within existing constraint authority.

**CDD_P08_RECONFORMANCE_NO_SEMANTIC_INVENTION**
Reconformance must not introduce new behavior to force test passage.

**CDD_P08_RECONFORMANCE_UPSTREAM_ESCALATION**
If reconformance requires new meaning, the issue must be escalated upstream.

**CDD_P08_RECONFORMANCE_RETEST_REQUIRED**
Any reconformance change must trigger proof re-execution.

**CDD_P08_RECONFORMANCE_TRACE_PRESERVATION**
Reconformance history must preserve mappings from failure to correction.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Reconform Implementation, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 08 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Reconform Implementation.

**Invariants:** See step invariants above.

**Prompts**
- Reconform Implementation Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Reconform Implementation Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Reconform Implementation
*Execute Reconform Implementation with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Reconform Implementation while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Reconform Implementation with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Reconform Implementation Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Reconform Implementation Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Reconform Implementation.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Reconform Implementation Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Reconform Implementation Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
