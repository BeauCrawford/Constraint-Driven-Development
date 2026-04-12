# Step 09 - Build Impact Paths

---

## Description

Step 09, Build Impact Paths, performs its Phase 09 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P09_IMPACT_PATHS_REQUIRED**
Impact paths must be built across requirement, invariant, constraint, test, and code layers.

**CDD_P09_CHANGE_PROPAGATION_VISIBILITY**
Impact paths must show what downstream artifacts require revalidation after upstream change.

**CDD_P09_IMPACT_PATH_BIDIRECTIONALITY**
Impact paths must support upstream and downstream navigation.

**CDD_P09_IMPACT_PATH_NO_SILENT_GAPS**
Missing impact links must be recorded as traceability gaps.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Build Impact Paths, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 09 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Build Impact Paths.

**Invariants:** See step invariants above.

**Prompts**
- Build Impact Paths Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Build Impact Paths Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Build Impact Paths
*Execute Build Impact Paths with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Build Impact Paths while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Build Impact Paths with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Build Impact Paths Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Build Impact Paths Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Build Impact Paths.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Build Impact Paths Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Build Impact Paths Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.