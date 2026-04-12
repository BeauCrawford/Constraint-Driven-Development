# Step 07 - Detect Conflicts

---

## Description

Step 07, Detect Conflicts, identifies and resolves contradictions before they propagate downstream. It checks raw intent, normalized requirements, glossary meanings, scope declarations, and assumptions, then records decisions with authority and traceability.

---

## Invariants

**CDD_P01_CONFLICT_DETECTION_REQUIRED**
The requirement set must be checked for contradictions before publication.

**CDD_P01_CONFLICT_RAW_NORMALIZED_PARITY**
Conflicts must be detected across raw intent, normalized requirements, glossary meanings, scope declarations, and assumptions.

**CDD_P01_CONFLICT_REQUIREMENT_LINKAGE**
Each detected conflict must identify the affected requirement IDs or raw intent items.

**CDD_P01_CONFLICT_DECISION_RECORD**
Each resolved conflict must include the resolution decision and authority for that decision.

**CDD_P01_CONFLICT_NO_SILENT_OVERRIDE**
A requirement must not override another requirement without a visible resolution artifact.

**CDD_P01_CONFLICT_BLOCKS_STABILIZATION**
Unresolved behavioral conflicts block requirement stabilization.

**CDD_P01_CONFLICT_RESOLUTION_TRACE_RETENTION**
Rejected alternatives and superseded wording must remain traceable to the conflict record.

---

## Substeps

### 🟥 Substep 01 - Scan Conflict Surfaces
*Check every requirement formation layer for contradictions.*

* **🟥 AI Actions:** Compare raw intent, normalized requirements, glossary terms, scope declarations, and assumptions for conflicts.
* **🟦 Human Actions:** Confirm true conflicts versus acceptable distinctions.

**Inputs:** Raw intent, normalized requirements, glossary map, scope map, and assumption register.

**Outputs:** Conflict candidate register.

**Invariants:** CDD_P01_CONFLICT_DETECTION_REQUIRED, CDD_P01_CONFLICT_RAW_NORMALIZED_PARITY

**Prompts**
- Requirement Conflict Scanner - Detect contradictions across raw and normalized requirement artifacts.
- Cross-Layer Conflict Review - Compare glossary, scope, and assumption records for inconsistent meaning.

---

### 🟥 Substep 02 - Link Conflicts to Intent
*Make every conflict addressable.*

* **🟥 AI Actions:** Map each conflict to affected requirement IDs, raw intent items, and related glossary or scope decisions.
* **🟦 Human Actions:** Confirm affected artifacts and missing links.

**Inputs:** Conflict candidate register and requirement ID map.

**Outputs:** Requirement-linked conflict register.

**Invariants:** CDD_P01_CONFLICT_REQUIREMENT_LINKAGE, CDD_P01_CONFLICT_RESOLUTION_TRACE_RETENTION

**Prompts**
- Conflict Lineage Mapper - Link each detected conflict to affected requirements and source intent.
- Conflict Scope Review - Identify whether each conflict is behavioral, terminology, scope, or assumption driven.

---

### 🟦 Substep 03 - Resolve Conflicts
*Record the decision authority for each contradiction.*

* **🟥 AI Actions:** Propose resolution options, identify rejected alternatives, and update conflict records.
* **🟦 Human Actions:** Choose the authoritative resolution or mark the conflict as blocking.

**Inputs:** Requirement-linked conflict register.

**Outputs:** Conflict resolution records.

**Invariants:** CDD_P01_CONFLICT_DECISION_RECORD, CDD_P01_CONFLICT_NO_SILENT_OVERRIDE

**Prompts**
- Conflict Resolution Options - Generate resolution choices and the downstream impact of each.
- Conflict Decision Recorder - Capture the chosen resolution, authority, rejected alternatives, and affected requirements.

---

### 🟦 Substep 04 - Gate Unresolved Conflicts
*Prevent unresolved contradiction from stabilizing.*

* **🟥 AI Actions:** Identify unresolved conflicts and classify their blocking impact.
* **🟦 Human Actions:** Decide whether to resolve, escalate, or stop progression.

**Inputs:** Conflict resolution records and unresolved conflict list.

**Outputs:** Conflict gate decision.

**Invariants:** CDD_P01_CONFLICT_BLOCKS_STABILIZATION, CDD_P01_CONFLICT_RESOLUTION_TRACE_RETENTION

**Prompts**
- Conflict Gate Review - Determine whether unresolved conflicts block requirement stabilization.
- Conflict Escalation Brief - Summarize unresolved conflicts for stakeholder or governance decision.
