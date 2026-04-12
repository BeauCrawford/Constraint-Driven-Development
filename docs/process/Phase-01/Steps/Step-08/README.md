# Step 08 - Validate Completeness

---

## Description

Step 08, Validate Completeness, checks whether the requirement set fully captures the intent needed for downstream lowering. It surfaces missing behavior, actors, conditions, data meaning, negative space, and gap severity before governance review.

---

## Invariants

**CDD_P01_COMPLETENESS_CHECK_REQUIRED**
The requirement set must be checked for missing or underdefined intent before governance review.

**CDD_P01_COMPLETENESS_BEHAVIORAL_COVERAGE**
Required behavior, forbidden behavior, boundary behavior, and failure expectations must be evaluated for completeness.

**CDD_P01_COMPLETENESS_ACTOR_COVERAGE**
All actors referenced by the requirement set must have their relevant responsibilities and interactions defined or flagged.

**CDD_P01_COMPLETENESS_CONDITION_COVERAGE**
Important triggering conditions, preconditions, and termination conditions must be defined or flagged.

**CDD_P01_COMPLETENESS_DATA_MEANING_COVERAGE**
Domain data, states, terms, and classifications needed to understand requirements must be defined or flagged.

**CDD_P01_COMPLETENESS_NEGATIVE_SPACE_VISIBILITY**
Forbidden or excluded states implied by the intent must be captured or flagged for stakeholder decision.

**CDD_P01_COMPLETENESS_GAP_RECORDING**
Each completeness gap must be recorded with affected requirements, impact, and required decision.

**CDD_P01_COMPLETENESS_GAP_BLOCKING_CLASSIFICATION**
Each gap must be classified as blocking, non-blocking, or governed exception.

---

## Substeps

### 🟥 Substep 01 - Check Behavioral Coverage
*Ensure expected behavior has been captured.*

* **🟥 AI Actions:** Evaluate required, forbidden, boundary, and failure expectations for missing or underdefined behavior.
* **🟦 Human Actions:** Confirm missing behavior and clarify intended coverage.

**Inputs:** Normalized requirements, scope map, and conflict records.

**Outputs:** Behavioral completeness findings.

**Invariants:** CDD_P01_COMPLETENESS_CHECK_REQUIRED, CDD_P01_COMPLETENESS_BEHAVIORAL_COVERAGE

**Prompts**
- Behavioral Completeness Checker - Find missing required, forbidden, boundary, or failure behavior.
- Missing Behavior Clarifier - Draft targeted questions for underdefined behavior.

---

### 🟥 Substep 02 - Check Actor and Condition Coverage
*Ensure participants and applicability are defined.*

* **🟥 AI Actions:** Identify missing actor responsibilities, interactions, triggering conditions, preconditions, and termination conditions.
* **🟦 Human Actions:** Resolve actor or condition gaps.

**Inputs:** Normalized requirements and glossary map.

**Outputs:** Actor and condition completeness findings.

**Invariants:** CDD_P01_COMPLETENESS_ACTOR_COVERAGE, CDD_P01_COMPLETENESS_CONDITION_COVERAGE

**Prompts**
- Actor Coverage Checker - Identify actors whose responsibilities or interactions are missing.
- Condition Coverage Checker - Identify missing triggers, preconditions, termination conditions, or applicability boundaries.

---

### 🟥 Substep 03 - Check Data and Negative Space
*Ensure meaning and forbidden states are visible.*

* **🟥 AI Actions:** Identify missing domain data, states, classifications, forbidden states, and excluded states.
* **🟦 Human Actions:** Decide whether missing negative space or data meaning requires new requirements.

**Inputs:** Glossary map, scope map, assumptions, and normalized requirements.

**Outputs:** Data meaning and negative-space completeness findings.

**Invariants:** CDD_P01_COMPLETENESS_DATA_MEANING_COVERAGE, CDD_P01_COMPLETENESS_NEGATIVE_SPACE_VISIBILITY

**Prompts**
- Data Meaning Completeness Checker - Find domain data, states, or classifications that lack enough definition.
- Negative Space Finder - Identify forbidden, excluded, or invalid states implied by the requirement set.

---

### 🟥 Substep 04 - Record and Classify Gaps
*Make incompleteness governable.*

* **🟥 AI Actions:** Record completeness gaps with affected requirements, impact, and recommended blocking classification.
* **🟦 Human Actions:** Approve gap classification and decide required action.

**Inputs:** Completeness findings and requirement ID map.

**Outputs:** Completeness gap register.

**Invariants:** CDD_P01_COMPLETENESS_GAP_RECORDING, CDD_P01_COMPLETENESS_GAP_BLOCKING_CLASSIFICATION

**Prompts**
- Completeness Gap Register Builder - Convert completeness findings into explicit gap records.
- Completeness Exit Review - Decide whether the requirement set is complete enough for governance review.
