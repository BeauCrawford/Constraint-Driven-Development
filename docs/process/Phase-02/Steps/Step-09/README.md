# Step 09 - Review Gate

---

## Description

Step 09, Review Gate, validates the invariant set before finalization. It checks evidence for coverage, implementation independence, minimality, negative space, traceability, exceptions, and prevents approval without substantive review evidence.

---

## Invariants

**CDD_P02_REVIEW_GATE_REQUIRED**
The invariant set must pass a review gate before finalization.

**CDD_P02_REVIEW_COVERAGE_EVIDENCE**
Review must include evidence that invariants cover parent requirement intent.

**CDD_P02_REVIEW_IMPLEMENTATION_INDEPENDENCE_EVIDENCE**
Review must include evidence that invariants remain implementation-independent.

**CDD_P02_REVIEW_MINIMALITY_EVIDENCE**
Review must include evidence that invariants are necessary, minimal, and non-redundant.

**CDD_P02_REVIEW_NEGATIVE_SPACE_EVIDENCE**
Review must include evidence that forbidden states were captured or explicitly marked as gaps.

**CDD_P02_REVIEW_TRACEABILITY_EVIDENCE**
Review must include requirement-to-invariant lineage evidence.

**CDD_P02_REVIEW_EXCEPTION_VISIBILITY**
Any exception to Phase 02 invariants must be visible, justified, owned, and reconciliation-bound.

**CDD_P02_REVIEW_NO_CEREMONIAL_APPROVAL**
Review approval without evidence does not grant downstream authority.

---

## Substeps

### 🟥 Substep 01 - Assemble Review Evidence
*Bring invariant integrity evidence into one reviewable surface.*

* **🟥 AI Actions:** Gather coverage, independence, minimality, redundancy, negative-space, conflict, and traceability evidence.
* **🟦 Human Actions:** Confirm evidence completeness and identify missing materials.

**Inputs:** Invariant set, trace maps, negative-space records, conflict records, and minimality decisions.

**Outputs:** Invariant review evidence packet.

**Invariants:** CDD_P02_REVIEW_GATE_REQUIRED, CDD_P02_REVIEW_COVERAGE_EVIDENCE, CDD_P02_REVIEW_TRACEABILITY_EVIDENCE

**Prompts**
- Invariant Review Evidence Assembler - Gather Phase 02 review evidence into a single packet.
- Invariant Evidence Completeness Check - Find missing review evidence before finalization.

---

### 🟥 Substep 02 - Validate Invariant Quality
*Check the set is independent, minimal, and complete.*

* **🟥 AI Actions:** Summarize evidence for implementation independence, minimality, non-redundancy, and negative space.
* **🟦 Human Actions:** Review and challenge quality evidence.

**Inputs:** Invariant review evidence packet.

**Outputs:** Invariant quality review findings.

**Invariants:** CDD_P02_REVIEW_IMPLEMENTATION_INDEPENDENCE_EVIDENCE, CDD_P02_REVIEW_MINIMALITY_EVIDENCE, CDD_P02_REVIEW_NEGATIVE_SPACE_EVIDENCE

**Prompts**
- Invariant Quality Review - Assess implementation independence, minimality, non-redundancy, and negative-space evidence.
- Review Risk Finder - Identify invariant quality risks that should block or require exception.

---

### 🟦 Substep 03 - Govern Exceptions
*Make deviations visible and owned.*

* **🟥 AI Actions:** Summarize exceptions, owners, rationale, affected lineage, and reconciliation obligations.
* **🟦 Human Actions:** Accept, reject, defer, or mark exceptions as blocking.

**Inputs:** Invariant quality review findings and exception register.

**Outputs:** Reviewed Phase 02 exception register.

**Invariants:** CDD_P02_REVIEW_EXCEPTION_VISIBILITY, CDD_P02_REVIEW_NO_CEREMONIAL_APPROVAL

**Prompts**
- Phase 02 Exception Brief - Summarize invariant extraction exceptions and their impact.
- Exception Disposition Recorder - Capture exception status, owner, rationale, and reconciliation path.

---

### 🟦 Substep 04 - Decide Review Gate
*Grant or deny readiness based on evidence.*

* **🟥 AI Actions:** Present gate decision options and evidence links.
* **🟦 Human Actions:** Approve, reject, or send the invariant set back for rework.

**Inputs:** Review evidence packet and reviewed exception register.

**Outputs:** Phase 02 review gate decision.

**Invariants:** CDD_P02_REVIEW_GATE_REQUIRED, CDD_P02_REVIEW_NO_CEREMONIAL_APPROVAL

**Prompts**
- Phase 02 Gate Decision Brief - Summarize whether the invariant set can proceed and why.
- Review Finding Mapper - Link review findings to invariant, requirement, gap, conflict, or exception records.
