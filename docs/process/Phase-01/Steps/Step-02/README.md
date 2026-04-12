# Step 02 - Normalize Language

---

## Description

Step 02, Normalize Language, turns captured raw intent into structured requirement statements without changing meaning. It removes ambiguity, narrative drift, mixed intent, and implicit modality while preserving traceability to the original raw source.

---

## Invariants

**CDD_P01_REQUIREMENT_STATEMENT_STRUCTURE**
Each normalized requirement must be expressed as a structured statement of intended system behavior.

**CDD_P01_REQUIREMENT_SINGLE_INTENT**
Each normalized requirement should contain one coherent intent unit suitable for invariant extraction.

**CDD_P01_REQUIREMENT_AMBIGUITY_REDUCTION**
Ambiguous language must be rewritten or flagged before the requirement can proceed.

**CDD_P01_REQUIREMENT_NARRATIVE_DRIFT_REMOVAL**
Narrative, motivational, or incidental language must not remain in the requirement body unless it carries required domain meaning.

**CDD_P01_REQUIREMENT_IMPLEMENTATION_ABSTINENCE**
Requirements must not prescribe implementation mechanisms unless the mechanism itself is a stakeholder intent or domain constraint.

**CDD_P01_REQUIREMENT_MODALITY_EXPLICITNESS**
Required, forbidden, optional, and conditional behavior must be explicitly distinguished.

**CDD_P01_REQUIREMENT_ACTOR_EXPLICITNESS**
Actors, systems, users, or external parties referenced by a requirement must be explicit or recorded as unresolved.

**CDD_P01_REQUIREMENT_CONDITION_EXPLICITNESS**
Triggering conditions, preconditions, and applicability boundaries must be explicit or recorded as gaps.

**CDD_P01_REQUIREMENT_OUTCOME_EXPLICITNESS**
Expected outcomes and externally observable effects must be explicit or recorded as gaps.

**CDD_P01_REQUIREMENT_RAW_TRACE_RETENTION**
Each normalized requirement must remain traceable to the raw intent it came from.

---

## Substeps

### 🟥 Substep 01 - Structure Requirements
*Turn raw intent into requirement-shaped statements.*

* **🟥 AI Actions:** Rewrite raw intent into structured requirement statements while preserving source meaning.
* **🟦 Human Actions:** Confirm that structured statements still express the intended domain behavior.

**Inputs:** Raw intent capture set and attribution records.

**Outputs:** Structured requirement candidates.

**Invariants:** CDD_P01_REQUIREMENT_STATEMENT_STRUCTURE, CDD_P01_REQUIREMENT_RAW_TRACE_RETENTION

**Prompts**
- Requirement Statement Normalizer - Convert raw intent into structured requirement statements without adding implementation detail.
- Raw Trace Preservation Review - Check that each normalized statement retains a clear link to its original raw source.

---

### 🟥 Substep 02 - Split Mixed Intent
*Make each requirement carry one coherent intent.*

* **🟥 AI Actions:** Detect combined behaviors, bundled conditions, and compound outcomes, then split them into coherent requirement units.
* **🟦 Human Actions:** Approve splits that affect domain meaning or stakeholder review boundaries.

**Inputs:** Structured requirement candidates.

**Outputs:** Single-intent requirement candidates.

**Invariants:** CDD_P01_REQUIREMENT_SINGLE_INTENT, CDD_P01_REQUIREMENT_STATEMENT_STRUCTURE

**Prompts**
- Mixed Intent Splitter - Find requirement candidates that contain multiple behavior units and propose clean splits.
- Requirement Granularity Review - Assess whether each candidate is decomposed enough for invariant extraction.

---

### 🟥 Substep 03 - Reduce Ambiguity
*Make unclear language explicit or visible as a gap.*

* **🟥 AI Actions:** Identify vague terms, unresolved references, unclear actors, hidden conditions, and uncertain outcomes.
* **🟦 Human Actions:** Resolve domain ambiguity or mark it as a governed gap.

**Inputs:** Single-intent requirement candidates.

**Outputs:** Ambiguity-reduced requirements and ambiguity gap records.

**Invariants:** CDD_P01_REQUIREMENT_AMBIGUITY_REDUCTION, CDD_P01_REQUIREMENT_ACTOR_EXPLICITNESS, CDD_P01_REQUIREMENT_CONDITION_EXPLICITNESS, CDD_P01_REQUIREMENT_OUTCOME_EXPLICITNESS

**Prompts**
- Ambiguity Detector - Identify unclear actors, terms, conditions, outcomes, and references in normalized requirements.
- Requirement Clarification Draft - Generate concise clarification questions for unresolved ambiguity.

---

### 🟥 Substep 04 - Remove Narrative Drift
*Separate requirement truth from explanation.*

* **🟥 AI Actions:** Remove narrative, motivation, examples, and incidental phrasing unless they carry required domain meaning.
* **🟦 Human Actions:** Confirm that removed text is context rather than required behavior.

**Inputs:** Ambiguity-reduced requirements and raw intent sources.

**Outputs:** Drift-reduced normalized requirements.

**Invariants:** CDD_P01_REQUIREMENT_NARRATIVE_DRIFT_REMOVAL, CDD_P01_REQUIREMENT_RAW_TRACE_RETENTION

**Prompts**
- Narrative Drift Trimmer - Separate behavioral requirement text from explanatory or motivational language.
- Meaning Loss Check - Verify that removing narrative text did not drop required domain meaning.

---

### 🟥 Substep 05 - Preserve Requirement Purity
*Keep requirements out of implementation and make modality explicit.*

* **🟥 AI Actions:** Detect implementation prescription and distinguish required, forbidden, optional, and conditional behavior.
* **🟦 Human Actions:** Decide whether mechanism language is true stakeholder intent or implementation leakage.

**Inputs:** Drift-reduced normalized requirements.

**Outputs:** Implementation-independent normalized requirements with explicit modality.

**Invariants:** CDD_P01_REQUIREMENT_IMPLEMENTATION_ABSTINENCE, CDD_P01_REQUIREMENT_MODALITY_EXPLICITNESS

**Prompts**
- Implementation Leakage Audit - Find requirement wording that prescribes mechanisms, technologies, or design choices.
- Modality Clarifier - Classify requirement language as required, forbidden, optional, or conditional behavior.
