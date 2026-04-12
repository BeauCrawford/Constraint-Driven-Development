# Step 11 - Publish Requirements

---

## Description

Step 11, Publish Requirements, produces the authoritative Phase 01 output for Phase 02. It makes the requirement baseline accessible, complete, version-visible, traceable, and clearly separated from drafts or informal notes.

---

## Invariants

**CDD_P01_PUBLICATION_REQUIRED**
The authoritative requirement set must be published before Phase 02 begins.

**CDD_P01_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve Phase 01 intent through the published requirement set, not informal notes or unapproved drafts.

**CDD_P01_PUBLICATION_CONTENT_COMPLETE**
Publication must include normalized requirements, requirement IDs, glossary grounding, assumptions, scope boundaries, conflict resolutions, and unresolved governed exceptions.

**CDD_P01_PUBLICATION_ACCESSIBILITY**
Published requirements must be accessible to downstream actors and tools that perform invariant extraction.

**CDD_P01_PUBLICATION_VERSION_VISIBILITY**
The published requirement set must expose its version, baseline identity, or revision state.

**CDD_P01_PUBLICATION_NO_ORPHAN_REQUIREMENTS**
No published requirement may lack raw intent lineage or governance status.

---

## Substeps

### 🟥 Substep 01 - Assemble Published Content
*Package the complete requirement baseline.*

* **🟥 AI Actions:** Assemble normalized requirements, IDs, glossary grounding, assumptions, scope boundaries, conflict resolutions, and exceptions.
* **🟦 Human Actions:** Confirm the publication package is complete and authoritative.

**Inputs:** Stabilized requirement baseline and Phase 01 evidence.

**Outputs:** Requirement publication package.

**Invariants:** CDD_P01_PUBLICATION_REQUIRED, CDD_P01_PUBLICATION_CONTENT_COMPLETE

**Prompts**
- Requirement Publication Assembler - Prepare the complete Phase 01 requirement publication package.
- Publication Completeness Review - Check that all required Phase 01 artifacts are included.

---

### 🟥 Substep 02 - Verify Authority and Accessibility
*Make the published set the single downstream source.*

* **🟥 AI Actions:** Check that drafts, notes, and unapproved artifacts are not treated as authoritative.
* **🟦 Human Actions:** Confirm access and authority expectations for downstream teams or tools.

**Inputs:** Requirement publication package and repository/documentation locations.

**Outputs:** Publication authority and accessibility check.

**Invariants:** CDD_P01_PUBLICATION_SINGLE_AUTHORITY, CDD_P01_PUBLICATION_ACCESSIBILITY

**Prompts**
- Publication Authority Checker - Verify the published requirement set is the single source for downstream lowering.
- Accessibility Review - Confirm downstream actors and tools can access the published requirement baseline.

---

### 🟥 Substep 03 - Verify Version and Lineage
*Preserve identity and source traceability.*

* **🟥 AI Actions:** Confirm version visibility, baseline identity, governance status, and raw intent lineage for every published requirement.
* **🟦 Human Actions:** Approve publication identity and resolve lineage gaps.

**Inputs:** Requirement publication package, raw intent register, and governance evidence.

**Outputs:** Versioned, lineage-checked requirement publication.

**Invariants:** CDD_P01_PUBLICATION_VERSION_VISIBILITY, CDD_P01_PUBLICATION_NO_ORPHAN_REQUIREMENTS

**Prompts**
- Publication Lineage Audit - Find published requirements that lack raw intent lineage or governance status.
- Version Visibility Check - Confirm the published requirement set exposes baseline identity or revision state.

---

### 🟦 Substep 04 - Publish and Handoff
*Establish authoritative input for invariant extraction.*

* **🟥 AI Actions:** Prepare the handoff summary for Phase 02 and list any governed exceptions.
* **🟦 Human Actions:** Approve publication and downstream handoff.

**Inputs:** Versioned, lineage-checked requirement publication.

**Outputs:** Authoritative Phase 01 requirement set for invariant extraction.

**Invariants:** CDD_P01_PUBLICATION_REQUIRED, CDD_P01_PUBLICATION_SINGLE_AUTHORITY

**Prompts**
- Phase 01 Handoff Summary - Summarize the published requirement baseline for invariant extraction.
- Publication Exit Review - Decide whether the requirement set is ready to serve as Phase 02 input.
