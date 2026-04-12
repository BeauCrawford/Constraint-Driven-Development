# Step 01 - Load Requirements

---

## Description

Step 01, Load Requirements, establishes the stabilized Phase 01 requirement baseline as the only semantic authority for invariant extraction. It preserves requirement IDs, baseline identity, lineage, and upstream gap visibility before invariant candidates are created.

---

## Invariants

**CDD_P02_REQUIREMENT_BASELINE_REQUIRED**
Phase 02 must load only a stabilized Phase 01 requirement baseline as its semantic input.

**CDD_P02_REQUIREMENT_SOURCE_AUTHORITY**
The loaded requirement baseline is the authoritative source for invariant extraction.

**CDD_P02_REQUIREMENT_ID_PRESERVATION**
All requirement IDs from the loaded baseline must remain visible during invariant extraction.

**CDD_P02_REQUIREMENT_LINEAGE_INITIALIZATION**
Every invariant candidate must be traceable to one or more loaded requirement IDs.

**CDD_P02_REQUIREMENT_NO_DRAFT_AUTHORITY**
Unapproved drafts, notes, or informal stakeholder comments must not grant invariant authority.

**CDD_P02_REQUIREMENT_BASELINE_VERSION_VISIBILITY**
The requirement baseline version, revision state, or publication identity must be visible.

**CDD_P02_REQUIREMENT_INPUT_COMPLETENESS_CHECK**
Missing requirements, missing IDs, unresolved Phase 01 blockers, or unpublished baselines must block extraction.

**CDD_P02_REQUIREMENT_UPSTREAM_GAP_VISIBILITY**
Any defect discovered in the Phase 01 baseline must be recorded as an upstream gap rather than silently repaired in Phase 02.

---

## Substeps

### 🟥 Substep 01 - Load Baseline
*Bring the stabilized requirement baseline into the extraction workspace.*

* **🟥 AI Actions:** Load the published Phase 01 requirement set and identify baseline/version status.
* **🟦 Human Actions:** Confirm the baseline is the approved Phase 01 output.

**Inputs:** Published Phase 01 requirement set and governance status.

**Outputs:** Loaded requirement baseline.

**Invariants:** CDD_P02_REQUIREMENT_BASELINE_REQUIRED, CDD_P02_REQUIREMENT_SOURCE_AUTHORITY, CDD_P02_REQUIREMENT_BASELINE_VERSION_VISIBILITY

**Prompts**
- Requirement Baseline Loader - Load the stabilized requirement set and summarize its baseline identity.
- Baseline Authority Review - Confirm whether the loaded requirements are the authoritative Phase 01 output.

---

### 🟥 Substep 02 - Preserve IDs and Lineage
*Keep requirement identity visible before extraction begins.*

* **🟥 AI Actions:** Verify requirement IDs and initialize trace links for future invariant candidates.
* **🟦 Human Actions:** Resolve missing, duplicate, or unclear requirement identity issues.

**Inputs:** Loaded requirement baseline.

**Outputs:** Requirement ID and lineage map.

**Invariants:** CDD_P02_REQUIREMENT_ID_PRESERVATION, CDD_P02_REQUIREMENT_LINEAGE_INITIALIZATION

**Prompts**
- Requirement Lineage Initializer - Build the requirement ID map needed for invariant extraction.
- Requirement ID Visibility Check - Find requirements whose IDs or lineage are missing or unclear.

---

### 🟥 Substep 03 - Exclude Draft Authority
*Prevent informal inputs from becoming invariant truth.*

* **🟥 AI Actions:** Detect drafts, notes, or unapproved source material being used as extraction authority.
* **🟦 Human Actions:** Decide whether informal material must be promoted upstream or excluded.

**Inputs:** Loaded requirement baseline and available supporting notes.

**Outputs:** Draft authority exclusion notes.

**Invariants:** CDD_P02_REQUIREMENT_NO_DRAFT_AUTHORITY, CDD_P02_REQUIREMENT_SOURCE_AUTHORITY

**Prompts**
- Draft Authority Detector - Identify unapproved sources that should not grant invariant authority.
- Informal Input Disposition - Decide whether informal material needs upstream Phase 01 handling.

---

### 🟥 Substep 04 - Check Input Completeness
*Stop extraction when Phase 01 defects remain.*

* **🟥 AI Actions:** Check for missing requirements, missing IDs, unresolved blockers, unpublished baselines, or upstream defects.
* **🟦 Human Actions:** Confirm blockers and route defects back upstream.

**Inputs:** Requirement ID and lineage map, Phase 01 governance status, and gap records.

**Outputs:** Input completeness and upstream gap register.

**Invariants:** CDD_P02_REQUIREMENT_INPUT_COMPLETENESS_CHECK, CDD_P02_REQUIREMENT_UPSTREAM_GAP_VISIBILITY

**Prompts**
- Phase 02 Input Completeness Check - Find missing or unresolved Phase 01 inputs that block extraction.
- Upstream Gap Register Builder - Record requirement baseline defects that must be handled upstream.
