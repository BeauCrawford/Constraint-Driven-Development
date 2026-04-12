# Step 03 - Decompose Requirements

---

## Description

Step 03, Decompose Requirements, breaks the stabilized requirement baseline into semantic units that are small enough for invariant extraction while preserving all parent meaning. It keeps conditions, actors, outcomes, scope, modality, and gaps visible.

---

## Invariants

**CDD_P02_SEMANTIC_UNIT_DECOMPOSITION_REQUIRED**
Requirements must be decomposed into semantic units before invariant extraction.

**CDD_P02_SEMANTIC_UNIT_PARENT_BINDING**
Each semantic unit must link to its parent requirement ID.

**CDD_P02_SEMANTIC_UNIT_ATOMICITY**
Each semantic unit must represent the smallest meaningful intent segment suitable for invariant extraction.

**CDD_P02_SEMANTIC_UNIT_NO_LOSS**
Decomposition must not drop parent requirement meaning.

**CDD_P02_SEMANTIC_UNIT_NO_ADDITION**
Decomposition must not add meaning not present in the parent requirement or governed glossary.

**CDD_P02_SEMANTIC_UNIT_CONDITION_RETENTION**
Conditions, triggers, actors, outcomes, and scope boundaries from parent requirements must remain visible in semantic units.

**CDD_P02_SEMANTIC_UNIT_MODALITY_RETENTION**
Required, forbidden, optional, and conditional modalities must remain distinguishable after decomposition.

**CDD_P02_SEMANTIC_UNIT_GAP_VISIBILITY**
Semantic units that cannot be extracted cleanly must be recorded as gaps or upstream clarification needs.

---

## Substeps

### 🟥 Substep 01 - Segment Requirement Meaning
*Break requirements into extraction-ready semantic units.*

* **🟥 AI Actions:** Split parent requirements into coherent semantic units.
* **🟦 Human Actions:** Confirm segmentation preserves intended domain meaning.

**Inputs:** Requirement baseline and term glossary map.

**Outputs:** Semantic unit candidates.

**Invariants:** CDD_P02_SEMANTIC_UNIT_DECOMPOSITION_REQUIRED, CDD_P02_SEMANTIC_UNIT_ATOMICITY

**Prompts**
- Semantic Unit Segmenter - Break requirements into smallest meaningful units for invariant extraction.
- Decomposition Granularity Review - Check whether semantic units are too broad, too narrow, or distorted.

---

### 🟥 Substep 02 - Bind Units to Parents
*Preserve requirement lineage during decomposition.*

* **🟥 AI Actions:** Link each semantic unit to parent requirement IDs.
* **🟦 Human Actions:** Resolve ambiguous or missing parent links.

**Inputs:** Semantic unit candidates and requirement ID map.

**Outputs:** Parent-bound semantic unit map.

**Invariants:** CDD_P02_SEMANTIC_UNIT_PARENT_BINDING, CDD_P02_SEMANTIC_UNIT_NO_LOSS

**Prompts**
- Semantic Unit Parent Mapper - Map each semantic unit to its parent requirement IDs.
- Decomposition Lineage Audit - Find semantic units that lack clear parent lineage.

---

### 🟥 Substep 03 - Preserve Conditions and Modality
*Keep behavioral shape intact after splitting.*

* **🟥 AI Actions:** Verify actors, triggers, conditions, outcomes, scope, and modalities remain visible.
* **🟦 Human Actions:** Clarify missing or ambiguous behavioral shape.

**Inputs:** Parent-bound semantic unit map and requirement baseline.

**Outputs:** Condition- and modality-checked semantic units.

**Invariants:** CDD_P02_SEMANTIC_UNIT_CONDITION_RETENTION, CDD_P02_SEMANTIC_UNIT_MODALITY_RETENTION

**Prompts**
- Semantic Unit Condition Retention Check - Ensure actors, triggers, conditions, outcomes, and scope remain visible.
- Semantic Unit Modality Check - Ensure required, forbidden, optional, and conditional meanings remain distinct.

---

### 🟥 Substep 04 - Detect Decomposition Drift
*Prevent loss, addition, and unclear units.*

* **🟥 AI Actions:** Identify dropped meaning, added meaning, or units that cannot be decomposed cleanly.
* **🟦 Human Actions:** Decide whether to revise units or escalate upstream.

**Inputs:** Condition- and modality-checked semantic units.

**Outputs:** Decomposition gap and drift register.

**Invariants:** CDD_P02_SEMANTIC_UNIT_NO_LOSS, CDD_P02_SEMANTIC_UNIT_NO_ADDITION, CDD_P02_SEMANTIC_UNIT_GAP_VISIBILITY

**Prompts**
- Decomposition Drift Audit - Find semantic loss or unauthorized addition introduced during decomposition.
- Semantic Unit Gap Register Builder - Record semantic units that require clarification before extraction.
