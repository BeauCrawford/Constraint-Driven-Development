# Step 05 - Remove Redundancy

---

## Description

Step 05, Remove Redundancy, reduces the invariant candidate set by eliminating duplicates and clarifying overlaps without losing parent requirement coverage. It preserves lineage for merged or removed candidates and records decisions for review.

---

## Invariants

**CDD_P02_REDUNDANCY_ANALYSIS_REQUIRED**
The invariant candidate set must be checked for duplicate and overlapping truths.

**CDD_P02_DUPLICATE_INVARIANT_ELIMINATION**
Duplicate invariant candidates must be merged or removed without semantic loss.

**CDD_P02_OVERLAP_RESOLUTION**
Overlapping invariant candidates must be separated, merged, or clarified so each remaining invariant has a distinct semantic role.

**CDD_P02_REDUNDANCY_TRACE_RETENTION**
Merged or removed invariant candidates must retain traceability to the requirements they covered.

**CDD_P02_REDUNDANCY_NO_COVERAGE_LOSS**
Removing redundancy must not remove coverage of parent requirement intent.

**CDD_P02_REDUNDANCY_DECISION_VISIBILITY**
Redundancy decisions that affect wording, merging, or removal must be visible for review.

---

## Substeps

### 🟥 Substep 01 - Detect Duplicates
*Find invariant candidates that state the same truth.*

* **🟥 AI Actions:** Compare invariant candidates for exact and semantic duplication.
* **🟦 Human Actions:** Confirm true duplicates versus intentionally distinct truths.

**Inputs:** Invariant candidate set and trace map.

**Outputs:** Duplicate candidate findings.

**Invariants:** CDD_P02_REDUNDANCY_ANALYSIS_REQUIRED, CDD_P02_DUPLICATE_INVARIANT_ELIMINATION

**Prompts**
- Duplicate Invariant Detector - Find invariant candidates that state the same truth.
- Duplicate Disposition Review - Decide whether duplicates should merge, remove, or remain distinct.

---

### 🟥 Substep 02 - Resolve Overlap
*Clarify candidates that partially cover the same meaning.*

* **🟥 AI Actions:** Identify overlapping candidates and propose merge, split, or wording changes.
* **🟦 Human Actions:** Approve the semantic role of each remaining invariant.

**Inputs:** Duplicate candidate findings and invariant candidate set.

**Outputs:** Overlap resolution plan.

**Invariants:** CDD_P02_OVERLAP_RESOLUTION, CDD_P02_REDUNDANCY_DECISION_VISIBILITY

**Prompts**
- Invariant Overlap Mapper - Identify partially overlapping invariant candidates.
- Overlap Resolution Options - Propose merge, split, or clarification options for overlapping candidates.

---

### 🟥 Substep 03 - Preserve Coverage and Trace
*Ensure reduction does not drop parent meaning.*

* **🟥 AI Actions:** Track lineage from removed or merged candidates to remaining invariants.
* **🟦 Human Actions:** Confirm that coverage is preserved after redundancy removal.

**Inputs:** Overlap resolution plan and requirement-to-candidate mappings.

**Outputs:** Reduced invariant set with retained traceability.

**Invariants:** CDD_P02_REDUNDANCY_TRACE_RETENTION, CDD_P02_REDUNDANCY_NO_COVERAGE_LOSS

**Prompts**
- Redundancy Trace Retention Check - Ensure merged or removed candidates retain requirement lineage.
- Coverage Loss Audit - Find parent requirement meaning lost during redundancy removal.
