# Step 06 - Validate Evidence Completeness

---

## Description

Step 06, Validate Evidence Completeness, performs its Phase 12 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P12_EVIDENCE_COMPLETENESS_VALIDATION_REQUIRED**
Governance must validate evidence completeness before authority is granted.

**CDD_P12_PROOF_BOUND_AUTHORITY**
No artifact may gain authority without proof support.

**CDD_P12_EVIDENCE_COVERAGE_ACROSS_PHASES**
Evidence must cover requirement formation, invariant extraction, closure, constraints, contracts, tests, simulation, implementation, traceability, revalidation, and change as applicable.

**CDD_P12_EVIDENCE_CONTRADICTION_VISIBILITY**
Conflicting evidence must be surfaced and resolved.

**CDD_P12_EVIDENCE_STALENESS_DETECTION**
Stale evidence must be detected when artifact baselines change.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Validate Evidence Completeness, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 12 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Validate Evidence Completeness.

**Invariants:** See step invariants above.

**Prompts**
- Validate Evidence Completeness Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Validate Evidence Completeness Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Validate Evidence Completeness
*Execute Validate Evidence Completeness with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Validate Evidence Completeness while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Validate Evidence Completeness with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Validate Evidence Completeness Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Validate Evidence Completeness Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Validate Evidence Completeness.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Validate Evidence Completeness Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Validate Evidence Completeness Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
