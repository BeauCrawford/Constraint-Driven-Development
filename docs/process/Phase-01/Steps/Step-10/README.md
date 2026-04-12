# Step 10 - Stabilize Requirements

---

## Description

Step 10, Stabilize Requirements, freezes the reviewed requirement set as a semantic baseline for invariant extraction. It ensures no blocking gaps remain, preserves traceability, and places post-stabilization changes under governed revision instead of silent editing.

---

## Invariants

**CDD_P01_STABILITY_GATE_REQUIRED**
Requirements must pass a stability gate before they can serve as input to invariant extraction.

**CDD_P01_STABILITY_NO_OPEN_BLOCKERS**
No unresolved blocking gaps, conflicts, undefined terms, or unapproved assumptions may remain at stabilization.

**CDD_P01_STABILITY_BASELINE_DECLARATION**
The stabilized requirement set must be identified as a semantic baseline.

**CDD_P01_STABILITY_CHANGE_CONTROL**
Changes after stabilization must occur through governed revision rather than silent editing.

**CDD_P01_STABILITY_TRACE_PRESERVATION**
Stabilization must preserve traceability to raw intent, glossary terms, assumptions, scope decisions, and conflict decisions.

**CDD_P01_STABILITY_DOWNSTREAM_READINESS**
Each stabilized requirement must be fit for invariant extraction without requiring runtime interpretation.

---

## Substeps

### 🟥 Substep 01 - Check Blockers
*Ensure nothing blocking remains open.*

* **🟥 AI Actions:** Identify unresolved blocking gaps, conflicts, undefined terms, and unapproved assumptions.
* **🟦 Human Actions:** Resolve or govern remaining blockers.

**Inputs:** Governance review decision, gap registers, conflict records, glossary gaps, and assumption register.

**Outputs:** Stability blocker assessment.

**Invariants:** CDD_P01_STABILITY_GATE_REQUIRED, CDD_P01_STABILITY_NO_OPEN_BLOCKERS

**Prompts**
- Stability Blocker Checker - Find unresolved blockers that prevent requirement stabilization.
- Stabilization Readiness Review - Decide whether remaining items block the semantic baseline.

---

### 🟥 Substep 02 - Declare Baseline
*Identify the stabilized requirement set.*

* **🟥 AI Actions:** Prepare baseline identity and summarize included requirement IDs and governed exceptions.
* **🟦 Human Actions:** Approve baseline identity and stabilization decision.

**Inputs:** Requirement set and stability blocker assessment.

**Outputs:** Requirement semantic baseline declaration.

**Invariants:** CDD_P01_STABILITY_BASELINE_DECLARATION, CDD_P01_STABILITY_TRACE_PRESERVATION

**Prompts**
- Requirement Baseline Drafter - Prepare a baseline declaration for the stabilized requirement set.
- Baseline Scope Review - Verify which requirements, exceptions, and gaps are included in the baseline.

---

### 🟦 Substep 03 - Establish Change Control
*Prevent silent edits after stabilization.*

* **🟥 AI Actions:** Identify post-stabilization change rules and affected traceability surfaces.
* **🟦 Human Actions:** Approve change-control expectations and ownership.

**Inputs:** Requirement semantic baseline declaration.

**Outputs:** Stabilization change-control note.

**Invariants:** CDD_P01_STABILITY_CHANGE_CONTROL, CDD_P01_STABILITY_TRACE_PRESERVATION

**Prompts**
- Change-Control Note Drafter - Define how post-stabilization requirement changes must be governed.
- Silent Edit Risk Review - Identify places where requirement edits could bypass stabilization.

---

### 🟥 Substep 04 - Confirm Downstream Readiness
*Ensure invariant extraction can begin without interpretation.*

* **🟥 AI Actions:** Check whether each stabilized requirement is explicit, traceable, and ready for invariant extraction.
* **🟦 Human Actions:** Approve readiness or send requirements back to earlier steps.

**Inputs:** Stabilized requirement baseline and traceability evidence.

**Outputs:** Downstream readiness decision.

**Invariants:** CDD_P01_STABILITY_DOWNSTREAM_READINESS, CDD_P01_STABILITY_GATE_REQUIRED

**Prompts**
- Invariant Extraction Readiness Check - Assess whether requirements are fit for invariant extraction.
- Stabilization Exit Review - Decide whether Phase 01 can proceed to publication.
