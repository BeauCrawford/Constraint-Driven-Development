# Step 07 - Define Negative Space

---

## Description

Step 07, Define Negative Space, captures forbidden, invalid, excluded, and out-of-scope states implied by parent requirements. It keeps negative space derived, traceable, boundary-visible, and ready for downstream constraint derivation without inventing new forbidden behavior.

---

## Invariants

**CDD_P02_NEGATIVE_SPACE_REQUIRED**
Forbidden states implied by requirements must be represented as invariants or explicit negative-space records.

**CDD_P02_NEGATIVE_SPACE_PARENT_DERIVATION**
Negative-space definitions must derive from parent requirements, glossary meaning, scope exclusions, or approved assumptions.

**CDD_P02_NEGATIVE_SPACE_NO_INVENTION**
Phase 02 must not invent forbidden states beyond upstream intent.

**CDD_P02_NEGATIVE_SPACE_BOUNDARY_VISIBILITY**
Invalid, excluded, and out-of-scope states must be distinguishable.

**CDD_P02_NEGATIVE_SPACE_TRACEABILITY**
Each negative-space definition must link to the requirement IDs and semantic units that justify it.

**CDD_P02_NEGATIVE_SPACE_CONSTRAINT_READINESS**
Negative-space definitions must be precise enough to support later forbidden-state constraint derivation.

**CDD_P02_NEGATIVE_SPACE_GAP_VISIBILITY**
Missing or unclear forbidden states must be recorded as gaps rather than inferred silently.

---

## Substeps

### 🟥 Substep 01 - Extract Forbidden States
*Find what parent intent says must not exist.*

* **🟥 AI Actions:** Identify forbidden, invalid, excluded, and failure-related states implied by requirements.
* **🟦 Human Actions:** Confirm whether each forbidden state is authorized by upstream intent.

**Inputs:** Minimal invariant set, semantic units, scope records, glossary, and approved assumptions.

**Outputs:** Negative-space candidate register.

**Invariants:** CDD_P02_NEGATIVE_SPACE_REQUIRED, CDD_P02_NEGATIVE_SPACE_PARENT_DERIVATION

**Prompts**
- Negative Space Extractor - Identify forbidden or invalid states implied by parent requirements.
- Forbidden State Authority Review - Confirm whether each negative-space candidate has upstream authority.

---

### 🟥 Substep 02 - Distinguish Boundary Types
*Separate invalid, excluded, and out-of-scope meanings.*

* **🟥 AI Actions:** Classify negative-space candidates as invalid, excluded, out-of-scope, or unclear.
* **🟦 Human Actions:** Resolve classification decisions.

**Inputs:** Negative-space candidate register and scope records.

**Outputs:** Classified negative-space register.

**Invariants:** CDD_P02_NEGATIVE_SPACE_BOUNDARY_VISIBILITY, CDD_P02_NEGATIVE_SPACE_NO_INVENTION

**Prompts**
- Negative Space Classifier - Distinguish invalid, excluded, and out-of-scope states.
- Negative Space Invention Audit - Find forbidden states that exceed upstream authority.

---

### 🟥 Substep 03 - Preserve Traceability
*Link forbidden states to parent meaning.*

* **🟥 AI Actions:** Map each negative-space definition to requirement IDs and semantic units.
* **🟦 Human Actions:** Confirm mappings and resolve missing lineage.

**Inputs:** Classified negative-space register and semantic unit map.

**Outputs:** Traceable negative-space definitions.

**Invariants:** CDD_P02_NEGATIVE_SPACE_TRACEABILITY, CDD_P02_NEGATIVE_SPACE_PARENT_DERIVATION

**Prompts**
- Negative Space Trace Mapper - Link negative-space definitions to parent requirement IDs and semantic units.
- Forbidden State Lineage Review - Find negative-space items without clear parent authority.

---

### 🟥 Substep 04 - Check Constraint Readiness
*Make forbidden states precise enough for later rules.*

* **🟥 AI Actions:** Evaluate whether negative-space definitions are precise enough for constraint derivation.
* **🟦 Human Actions:** Resolve missing or unclear forbidden-state meaning.

**Inputs:** Traceable negative-space definitions.

**Outputs:** Constraint-ready negative-space definitions and gaps.

**Invariants:** CDD_P02_NEGATIVE_SPACE_CONSTRAINT_READINESS, CDD_P02_NEGATIVE_SPACE_GAP_VISIBILITY

**Prompts**
- Negative Space Precision Check - Assess whether forbidden states are precise enough for constraint derivation.
- Negative Space Gap Register Builder - Record unclear or missing forbidden-state definitions.
