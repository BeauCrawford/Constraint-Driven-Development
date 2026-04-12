# Step 06 - Surface Assumptions

---

## Description

Step 06, Surface Assumptions, makes hidden meaning explicit before downstream lowering. It records assumption source, affected requirements, approval state, conflicts, and retirement history so unreviewed inference cannot grant execution authority.

---

## Invariants

**CDD_P01_ASSUMPTION_EXPLICITNESS**
Any meaning required to understand a requirement but absent from raw intent must be recorded as an assumption.

**CDD_P01_ASSUMPTION_SOURCE_CLASSIFICATION**
Each assumption must identify whether it came from domain knowledge, existing system context, analyst inference, or stakeholder confirmation.

**CDD_P01_ASSUMPTION_REQUIREMENT_LINKAGE**
Each assumption must link to the requirement IDs it affects.

**CDD_P01_ASSUMPTION_APPROVAL_REQUIRED**
An assumption that affects behavior must be reviewed before the requirement set is stabilized.

**CDD_P01_ASSUMPTION_NO_HIDDEN_AUTHORITY**
Unreviewed assumptions must not grant downstream execution authority.

**CDD_P01_ASSUMPTION_CONFLICT_VISIBILITY**
Assumptions that conflict with raw intent, glossary definitions, or other assumptions must be recorded as conflicts.

**CDD_P01_ASSUMPTION_RETIREMENT_TRACE**
When an assumption is replaced by confirmed intent, the decision must remain traceable.

---

## Substeps

### 🟥 Substep 01 - Identify Assumptions
*Find meaning that was inferred rather than stated.*

* **🟥 AI Actions:** Detect unstated conditions, implied actors, inferred behavior, and context-dependent meaning.
* **🟦 Human Actions:** Confirm whether each inference is valid, invalid, or needs stakeholder clarification.

**Inputs:** Normalized requirements, raw intent, scope map, and glossary.

**Outputs:** Assumption candidate register.

**Invariants:** CDD_P01_ASSUMPTION_EXPLICITNESS, CDD_P01_ASSUMPTION_NO_HIDDEN_AUTHORITY

**Prompts**
- Hidden Assumption Finder - Identify unstated meanings needed to understand the requirement set.
- Assumption Clarification Draft - Generate concise questions for assumptions requiring stakeholder confirmation.

---

### 🟥 Substep 02 - Classify Assumption Sources
*Show where every assumption came from.*

* **🟥 AI Actions:** Classify assumptions by source type: domain knowledge, existing system context, analyst inference, or stakeholder confirmation.
* **🟦 Human Actions:** Correct source classification and confirm authority.

**Inputs:** Assumption candidate register and source inventory.

**Outputs:** Source-classified assumption register.

**Invariants:** CDD_P01_ASSUMPTION_SOURCE_CLASSIFICATION, CDD_P01_ASSUMPTION_APPROVAL_REQUIRED

**Prompts**
- Assumption Source Classifier - Classify each assumption by origin and authority level.
- Assumption Authority Review - Identify assumptions that lack enough authority to proceed.

---

### 🟥 Substep 03 - Link Assumptions to Requirements
*Make assumption impact traceable.*

* **🟥 AI Actions:** Map assumptions to affected requirement IDs and related glossary or scope decisions.
* **🟦 Human Actions:** Confirm impact links and add missing affected requirements.

**Inputs:** Source-classified assumption register and requirement ID map.

**Outputs:** Requirement-linked assumption register.

**Invariants:** CDD_P01_ASSUMPTION_REQUIREMENT_LINKAGE, CDD_P01_ASSUMPTION_RETIREMENT_TRACE

**Prompts**
- Assumption Impact Mapper - Link each assumption to affected requirements and decisions.
- Assumption Traceability Review - Find assumptions that lack requirement lineage.

---

### 🟥 Substep 04 - Detect Assumption Conflicts
*Expose assumptions that contradict governed meaning.*

* **🟥 AI Actions:** Compare assumptions against raw intent, glossary definitions, scope boundaries, and other assumptions.
* **🟦 Human Actions:** Resolve conflicts or classify them for governance.

**Inputs:** Requirement-linked assumption register, glossary, raw intent, and scope map.

**Outputs:** Assumption conflict register.

**Invariants:** CDD_P01_ASSUMPTION_CONFLICT_VISIBILITY, CDD_P01_ASSUMPTION_APPROVAL_REQUIRED

**Prompts**
- Assumption Conflict Detector - Find assumptions that conflict with sources, glossary, scope, or each other.
- Assumption Exit Review - Decide which assumptions are approved, rejected, retired, or blocking.
