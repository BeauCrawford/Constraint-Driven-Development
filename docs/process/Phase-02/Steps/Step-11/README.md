# Step 11 - Publish Invariants

---

## Description

Step 11, Publish Invariants, releases the authoritative invariant layer for semantic closure validation and constraint derivation. It publishes statements, mappings, negative space, conflict decisions, exceptions, baseline identity, and governance status as the single downstream source of invariant truth.

---

## Invariants

**CDD_P02_PUBLICATION_REQUIRED**
The authoritative invariant set must be published before Phase 03 or constraint-oriented downstream work begins.

**CDD_P02_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve invariant truth through the published invariant set, not unapproved candidates or review notes.

**CDD_P02_PUBLICATION_CONTENT_COMPLETE**
Publication must include invariant statements, requirement mappings, negative-space definitions, conflict resolutions, and governed exceptions.

**CDD_P02_PUBLICATION_ACCESSIBILITY**
Published invariants must be accessible to downstream actors and tools that perform semantic closure validation and constraint derivation.

**CDD_P02_PUBLICATION_VERSION_VISIBILITY**
The published invariant set must expose its version, baseline identity, or revision state.

**CDD_P02_PUBLICATION_NO_ORPHAN_INVARIANTS**
No published invariant may lack requirement lineage or governance status.

**CDD_P02_PUBLICATION_CONSTRAINT_DERIVATION_BOUNDARY**
Published invariants define the allowed semantic boundary for later constraint derivation.

---

## Substeps

### 🟥 Substep 01 - Assemble Publication Content
*Package the complete invariant baseline.*

* **🟥 AI Actions:** Assemble invariant statements, requirement mappings, negative-space definitions, conflict records, exceptions, and baseline identity.
* **🟦 Human Actions:** Confirm the publication package is complete and authoritative.

**Inputs:** Finalized invariant baseline and Phase 02 evidence.

**Outputs:** Invariant publication package.

**Invariants:** CDD_P02_PUBLICATION_REQUIRED, CDD_P02_PUBLICATION_CONTENT_COMPLETE

**Prompts**
- Invariant Publication Assembler - Prepare the complete Phase 02 invariant publication package.
- Invariant Publication Completeness Review - Check that all required Phase 02 artifacts are included.

---

### 🟥 Substep 02 - Verify Authority and Access
*Make the published invariant set the single downstream source.*

* **🟥 AI Actions:** Check that candidates, notes, and unapproved review artifacts are not treated as authoritative.
* **🟦 Human Actions:** Confirm access and authority expectations for downstream work.

**Inputs:** Invariant publication package and repository/documentation locations.

**Outputs:** Publication authority and accessibility check.

**Invariants:** CDD_P02_PUBLICATION_SINGLE_AUTHORITY, CDD_P02_PUBLICATION_ACCESSIBILITY

**Prompts**
- Invariant Publication Authority Check - Verify the published invariant set is the single downstream source of invariant truth.
- Invariant Accessibility Review - Confirm downstream actors and tools can access the published invariant baseline.

---

### 🟥 Substep 03 - Verify Version and Lineage
*Preserve baseline identity and parent traceability.*

* **🟥 AI Actions:** Confirm version visibility, baseline identity, governance status, and requirement lineage for every published invariant.
* **🟦 Human Actions:** Approve publication identity and resolve lineage gaps.

**Inputs:** Invariant publication package and traceability evidence.

**Outputs:** Versioned, lineage-checked invariant publication.

**Invariants:** CDD_P02_PUBLICATION_VERSION_VISIBILITY, CDD_P02_PUBLICATION_NO_ORPHAN_INVARIANTS

**Prompts**
- Invariant Publication Lineage Audit - Find published invariants that lack requirement lineage or governance status.
- Invariant Version Visibility Check - Confirm the invariant set exposes baseline identity or revision state.

---

### 🟦 Substep 04 - Publish and Handoff
*Establish the boundary for closure validation and constraint derivation.*

* **🟥 AI Actions:** Prepare the handoff summary for downstream phases and list governed exceptions.
* **🟦 Human Actions:** Approve publication and downstream handoff.

**Inputs:** Versioned, lineage-checked invariant publication.

**Outputs:** Authoritative Phase 02 invariant set.

**Invariants:** CDD_P02_PUBLICATION_REQUIRED, CDD_P02_PUBLICATION_CONSTRAINT_DERIVATION_BOUNDARY

**Prompts**
- Phase 02 Handoff Summary - Summarize the published invariant baseline for closure validation and constraint derivation.
- Invariant Publication Exit Review - Decide whether the invariant set is ready to serve as downstream semantic authority.
