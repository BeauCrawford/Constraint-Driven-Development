# Step 09 - Governance Review

---

## Description

Step 09, Governance Review, verifies that the requirement set is ready to proceed. It checks evidence for explicitness, glossary grounding, IDs, scope, assumptions, conflicts, completeness, and stability, and ensures exceptions are visible rather than ceremonial.

---

## Invariants

**CDD_P01_GOVERNANCE_REVIEW_REQUIRED**
The requirement set must pass a governance review before downstream lowering.

**CDD_P01_GOVERNANCE_EVIDENCE_REQUIRED**
Review must have evidence for explicitness, glossary grounding, IDs, scope, assumptions, conflicts, completeness, and stability.

**CDD_P01_GOVERNANCE_DECISION_AUTHORITY**
Review approval, rejection, and exception decisions must identify the responsible authority.

**CDD_P01_GOVERNANCE_EXCEPTION_VISIBILITY**
Any exception to Phase 01 invariants must be visible, justified, owned, and time-bounded or reconciliation-bound.

**CDD_P01_GOVERNANCE_NO_CEREMONIAL_APPROVAL**
Approval without evidence does not grant downstream authority.

**CDD_P01_GOVERNANCE_REVIEW_TRACEABILITY**
Review findings must link to affected requirement IDs, gaps, assumptions, conflicts, or glossary terms.

---

## Substeps

### 🟥 Substep 01 - Assemble Review Evidence
*Bring gate evidence into one reviewable surface.*

* **🟥 AI Actions:** Gather evidence for explicitness, glossary grounding, IDs, scope, assumptions, conflicts, completeness, and stability.
* **🟦 Human Actions:** Confirm evidence completeness and identify missing review materials.

**Inputs:** Phase 01 step outputs and gap registers.

**Outputs:** Governance evidence packet.

**Invariants:** CDD_P01_GOVERNANCE_REVIEW_REQUIRED, CDD_P01_GOVERNANCE_EVIDENCE_REQUIRED

**Prompts**
- Governance Evidence Assembler - Gather Phase 01 evidence into a review packet.
- Evidence Completeness Checker - Identify missing evidence needed for governance review.

---

### 🟦 Substep 02 - Review Exceptions
*Make deviations visible and owned.*

* **🟥 AI Actions:** Summarize exceptions, unresolved gaps, risks, owners, and reconciliation needs.
* **🟦 Human Actions:** Decide whether exceptions are accepted, blocking, deferred, or resolved.

**Inputs:** Governance evidence packet, gap registers, and exception records.

**Outputs:** Reviewed exception register.

**Invariants:** CDD_P01_GOVERNANCE_EXCEPTION_VISIBILITY, CDD_P01_GOVERNANCE_DECISION_AUTHORITY

**Prompts**
- Exception Review Brief - Summarize Phase 01 exceptions with affected artifacts and risks.
- Exception Decision Recorder - Capture exception disposition, owner, rationale, and reconciliation obligation.

---

### 🟦 Substep 03 - Decide Gate Status
*Grant or deny readiness based on evidence.*

* **🟥 AI Actions:** Present approval, rejection, and rework options with evidence links.
* **🟦 Human Actions:** Approve, reject, or require rework with accountable authority.

**Inputs:** Governance evidence packet and reviewed exception register.

**Outputs:** Governance review decision.

**Invariants:** CDD_P01_GOVERNANCE_NO_CEREMONIAL_APPROVAL, CDD_P01_GOVERNANCE_REVIEW_TRACEABILITY

**Prompts**
- Gate Decision Brief - Summarize whether Phase 01 can proceed and why.
- Review Finding Mapper - Link review findings to affected requirements, gaps, assumptions, conflicts, or glossary terms.
