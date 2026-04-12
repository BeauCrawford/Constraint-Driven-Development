# Step 08 - Resolve Conflicts

---

## Description

Step 08, Resolve Conflicts, detects contradictions inside the invariant set and between positive truths and negative-space definitions. It escalates upstream ambiguity when needed and blocks finalization until conflicts have visible decisions.

---

## Invariants

**CDD_P02_INVARIANT_CONFLICT_DETECTION_REQUIRED**
The invariant set must be checked for contradictions before review.

**CDD_P02_INVARIANT_CONFLICT_PARENT_TRACE**
Each detected invariant conflict must identify the affected invariants, semantic units, and parent requirement IDs.

**CDD_P02_INVARIANT_CONFLICT_NO_SILENT_OVERRIDE**
One invariant must not override another without a visible resolution artifact.

**CDD_P02_INVARIANT_CONFLICT_UPSTREAM_ESCALATION**
Conflicts caused by parent requirement ambiguity or contradiction must be escalated upstream rather than patched in Phase 02.

**CDD_P02_INVARIANT_CONFLICT_RESOLUTION_AUTHORITY**
Each conflict resolution must identify the authority or decision source that resolved it.

**CDD_P02_INVARIANT_CONFLICT_BLOCKS_FINALIZATION**
Unresolved invariant conflicts block invariant finalization.

**CDD_P02_INVARIANT_CONSISTENCY_WITH_NEGATIVE_SPACE**
Positive invariant truths and negative-space definitions must not contradict each other.

---

## Substeps

### 🟥 Substep 01 - Detect Invariant Contradictions
*Find truths that cannot hold together.*

* **🟥 AI Actions:** Compare invariants for contradictory, mutually exclusive, or incompatible meanings.
* **🟦 Human Actions:** Confirm true conflicts versus acceptable scoped distinctions.

**Inputs:** Minimal invariant set and trace map.

**Outputs:** Invariant conflict candidate register.

**Invariants:** CDD_P02_INVARIANT_CONFLICT_DETECTION_REQUIRED, CDD_P02_INVARIANT_CONFLICT_PARENT_TRACE

**Prompts**
- Invariant Conflict Scanner - Detect contradictions across invariant statements.
- Conflict Scope Review - Distinguish actual contradictions from scoped variants.

---

### 🟥 Substep 02 - Check Negative-Space Consistency
*Ensure positive truth and forbidden states agree.*

* **🟥 AI Actions:** Compare positive invariants against negative-space definitions for contradictions.
* **🟦 Human Actions:** Resolve or escalate contradictory meanings.

**Inputs:** Minimal invariant set and negative-space definitions.

**Outputs:** Positive-negative consistency findings.

**Invariants:** CDD_P02_INVARIANT_CONSISTENCY_WITH_NEGATIVE_SPACE, CDD_P02_INVARIANT_CONFLICT_DETECTION_REQUIRED

**Prompts**
- Positive Negative Consistency Check - Find contradictions between invariants and negative-space definitions.
- Negative Space Conflict Brief - Summarize conflicts between allowed truths and forbidden states.

---

### 🟦 Substep 03 - Resolve or Escalate Conflicts
*Record the authority behind each decision.*

* **🟥 AI Actions:** Propose conflict resolutions and identify upstream ambiguity or contradiction.
* **🟦 Human Actions:** Decide whether to resolve in Phase 02, escalate upstream, or block finalization.

**Inputs:** Invariant conflict candidate register and consistency findings.

**Outputs:** Conflict resolution records.

**Invariants:** CDD_P02_INVARIANT_CONFLICT_UPSTREAM_ESCALATION, CDD_P02_INVARIANT_CONFLICT_RESOLUTION_AUTHORITY, CDD_P02_INVARIANT_CONFLICT_NO_SILENT_OVERRIDE

**Prompts**
- Invariant Conflict Resolution Options - Generate resolution and escalation options for invariant conflicts.
- Conflict Decision Recorder - Capture authority, decision, rejected alternatives, and affected lineage.

---

### 🟦 Substep 04 - Gate Unresolved Conflicts
*Prevent unresolved contradiction from finalizing.*

* **🟥 AI Actions:** Identify unresolved conflicts and classify their blocking impact.
* **🟦 Human Actions:** Approve blocking status or governed exception.

**Inputs:** Conflict resolution records.

**Outputs:** Conflict gate decision.

**Invariants:** CDD_P02_INVARIANT_CONFLICT_BLOCKS_FINALIZATION, CDD_P02_INVARIANT_CONFLICT_PARENT_TRACE

**Prompts**
- Invariant Conflict Gate Review - Decide whether unresolved conflicts block finalization.
- Conflict Escalation Summary - Prepare unresolved invariant conflicts for upstream or governance review.
