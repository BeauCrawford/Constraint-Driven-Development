# Step 07 - Revalidate Closure and Coverage

---

## Description

Step 07, Revalidate Closure and Coverage, performs its Phase 11 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P11_CLOSURE_REVALIDATION_REQUIRED**
Closure must be revalidated after upstream change and re-lowering.

**CDD_P11_COVERAGE_REVALIDATION_REQUIRED**
Coverage must be revalidated after regenerated constraints and tests.

**CDD_P11_PROOF_REEXECUTION_REQUIRED**
Affected deterministic proof must be re-executed.

**CDD_P11_TRACEABILITY_REVALIDATION_REQUIRED**
Lineage must be revalidated after regenerated artifacts are produced.

**CDD_P11_REVALIDATION_GAP_VISIBILITY**
Revalidation gaps, failures, and exceptions must be visible.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Revalidate Closure and Coverage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 11 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Revalidate Closure and Coverage.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Closure and Coverage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Revalidate Closure and Coverage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Revalidate Closure and Coverage
*Execute Revalidate Closure and Coverage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Revalidate Closure and Coverage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Revalidate Closure and Coverage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Closure and Coverage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Revalidate Closure and Coverage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Revalidate Closure and Coverage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Revalidate Closure and Coverage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Revalidate Closure and Coverage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.