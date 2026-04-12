# Step 04 - Measure Coverage

---

## Description

Step 04, Measure Coverage, performs its Phase 03 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P03_COVERAGE_MEASUREMENT_REQUIRED**
Semantic coverage must be measured between the requirement baseline and invariant set.

**CDD_P03_COVERAGE_REQUIREMENT_TO_INVARIANT**
Each requirement must be covered by one or more invariants or explicitly marked as a governed gap.

**CDD_P03_COVERAGE_INVARIANT_TO_REQUIREMENT**
Each invariant must map back to one or more parent requirements or be flagged as unauthorized addition.

**CDD_P03_COVERAGE_NEGATIVE_SPACE_INCLUDED**
Coverage measurement must include required behavior, forbidden behavior, boundary behavior, and negative-space definitions.

**CDD_P03_COVERAGE_CONTAINMENT_OVER_SIMILARITY**
Coverage must be evaluated as semantic containment, not textual similarity.

**CDD_P03_COVERAGE_EVIDENCE_REQUIRED**
Coverage decisions must include evidence sufficient for review.

**CDD_P03_COVERAGE_GAP_CANDIDATE_VISIBILITY**
Potential coverage gaps must be visible even before they are classified as blocking.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Measure Coverage, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 03 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Measure Coverage.

**Invariants:** See step invariants above.

**Prompts**
- Measure Coverage Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Measure Coverage Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Measure Coverage
*Execute Measure Coverage with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Measure Coverage while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Measure Coverage with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Measure Coverage Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Measure Coverage Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Measure Coverage.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Measure Coverage Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Measure Coverage Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
