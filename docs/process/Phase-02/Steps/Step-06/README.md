# Step 06 - Validate Minimality

---

## Description

Step 06, Validate Minimality, ensures each invariant is necessary, sufficient, and no broader than parent meaning requires. It removes incidental context, splits composite truths, merges inseparable truths, and records minimality decisions for review.

---

## Invariants

**CDD_P02_MINIMALITY_VALIDATION_REQUIRED**
Each invariant must be evaluated for minimality before finalization.

**CDD_P02_INVARIANT_MINIMAL_FORM**
Each invariant must be no broader than required to preserve its parent meaning.

**CDD_P02_INVARIANT_SUFFICIENCY**
The invariant set must be sufficient to preserve all parent requirement intent needed for downstream constraint derivation.

**CDD_P02_INVARIANT_NON_INCIDENTALITY**
Incidental explanation, examples, rationale, and narrative context must not remain in invariant statements.

**CDD_P02_INVARIANT_SPLIT_WHEN_COMPOSITE**
Composite invariants must be split when they contain multiple independently governed truths.

**CDD_P02_INVARIANT_MERGE_WHEN_INSEPARABLE**
Candidate invariants must be merged when separating them would distort a single irreducible truth.

**CDD_P02_MINIMALITY_REVIEWABILITY**
Minimality decisions must be inspectable by reviewers.

---

## Substeps

### 🟥 Substep 01 - Remove Incidental Content
*Strip context that is not invariant truth.*

* **🟥 AI Actions:** Identify rationale, examples, explanatory text, and incidental details in invariant statements.
* **🟦 Human Actions:** Confirm that removed text is not required semantic truth.

**Inputs:** Reduced invariant set.

**Outputs:** Non-incidental invariant set.

**Invariants:** CDD_P02_INVARIANT_NON_INCIDENTALITY, CDD_P02_INVARIANT_MINIMAL_FORM

**Prompts**
- Incidental Content Filter - Find examples, rationale, or narrative text inside invariant statements.
- Minimal Wording Review - Check whether invariant statements can be reduced without semantic loss.

---

### 🟥 Substep 02 - Split Composite Truths
*Separate independent invariant truths.*

* **🟥 AI Actions:** Detect invariants that contain multiple independently governed truths and propose splits.
* **🟦 Human Actions:** Approve splits that preserve parent meaning.

**Inputs:** Non-incidental invariant set.

**Outputs:** Split-ready invariant revisions.

**Invariants:** CDD_P02_INVARIANT_SPLIT_WHEN_COMPOSITE, CDD_P02_INVARIANT_MINIMAL_FORM

**Prompts**
- Composite Invariant Detector - Find invariants that should be split into independent truths.
- Invariant Split Review - Evaluate whether proposed splits preserve the original semantic meaning.

---

### 🟥 Substep 03 - Merge Inseparable Truths
*Keep a single truth together when separation distorts it.*

* **🟥 AI Actions:** Identify candidates whose separation damages a single irreducible truth.
* **🟦 Human Actions:** Approve merges and resolve semantic boundaries.

**Inputs:** Split-ready invariant revisions and overlap decisions.

**Outputs:** Minimal coherent invariant set.

**Invariants:** CDD_P02_INVARIANT_MERGE_WHEN_INSEPARABLE, CDD_P02_MINIMALITY_REVIEWABILITY

**Prompts**
- Inseparable Truth Finder - Identify invariant candidates that should remain merged.
- Minimality Decision Recorder - Record why a split or merge preserves invariant truth.

---

### 🟥 Substep 04 - Check Sufficiency
*Ensure the minimal set still preserves parent intent.*

* **🟥 AI Actions:** Compare the minimal invariant set against parent requirement coverage.
* **🟦 Human Actions:** Confirm sufficiency or require additional refinement.

**Inputs:** Minimal coherent invariant set and requirement lineage map.

**Outputs:** Minimality validation evidence.

**Invariants:** CDD_P02_INVARIANT_SUFFICIENCY, CDD_P02_MINIMALITY_VALIDATION_REQUIRED

**Prompts**
- Minimal Set Sufficiency Check - Verify the invariant set still covers parent requirement intent.
- Minimality Exit Review - Decide whether invariants are necessary, sufficient, and reviewable.
