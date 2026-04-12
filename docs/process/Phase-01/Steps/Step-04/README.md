# Step 04 - Assign Requirement IDs

---

## Description

Step 04, Assign Requirement IDs, makes each normalized requirement stable, addressable, and traceable. It prevents identity reuse, preserves raw-intent lineage, and ensures downstream artifacts can refer to requirements unambiguously.

---

## Invariants

**CDD_P01_REQUIREMENT_ID_REQUIRED**
Every normalized requirement must have a stable requirement ID before publication.

**CDD_P01_REQUIREMENT_ID_UNIQUENESS**
No two requirements may share the same requirement ID.

**CDD_P01_REQUIREMENT_ID_STABILITY**
Requirement IDs must not change because wording is refined.

**CDD_P01_REQUIREMENT_ID_NON_REUSE**
Retired or rejected requirement IDs must not be reused for different intent.

**CDD_P01_REQUIREMENT_ID_TRACE_BINDING**
Each requirement ID must bind normalized requirement text to its raw intent source.

**CDD_P01_REQUIREMENT_ID_ADDRESSABILITY**
Each requirement must be directly referable by ID in downstream artifacts, review comments, gaps, exceptions, and decisions.

---

## Substeps

### 🟥 Substep 01 - Identify ID Candidates
*Determine which requirement statements need stable IDs.*

* **🟥 AI Actions:** Identify normalized requirements that require IDs and flag duplicates or fragments.
* **🟦 Human Actions:** Confirm ID granularity and requirement boundaries.

**Inputs:** Normalized requirement set.

**Outputs:** Requirement ID assignment candidate list.

**Invariants:** CDD_P01_REQUIREMENT_ID_REQUIRED, CDD_P01_REQUIREMENT_ID_ADDRESSABILITY

**Prompts**
- Requirement ID Candidate Finder - Identify every normalized requirement that needs a stable ID.
- ID Granularity Review - Check whether each requirement boundary is appropriate for stable identification.

---

### 🟥 Substep 02 - Assign Stable IDs
*Make every requirement directly addressable.*

* **🟥 AI Actions:** Assign stable IDs according to the local naming scheme and check uniqueness.
* **🟦 Human Actions:** Approve the ID scheme and resolve collisions.

**Inputs:** Requirement ID assignment candidate list.

**Outputs:** ID-tagged requirement set.

**Invariants:** CDD_P01_REQUIREMENT_ID_REQUIRED, CDD_P01_REQUIREMENT_ID_UNIQUENESS, CDD_P01_REQUIREMENT_ID_STABILITY

**Prompts**
- Stable ID Assigner - Assign IDs to requirement candidates using the local convention.
- ID Collision Audit - Detect duplicate, unstable, or malformed requirement IDs.

---

### 🟥 Substep 03 - Bind IDs to Sources
*Tie requirement identity back to raw intent.*

* **🟥 AI Actions:** Map each requirement ID to normalized text and raw source lineage.
* **🟦 Human Actions:** Confirm that source lineage is correct and complete.

**Inputs:** ID-tagged requirements and raw intent register.

**Outputs:** Requirement ID trace map.

**Invariants:** CDD_P01_REQUIREMENT_ID_TRACE_BINDING, CDD_P01_REQUIREMENT_ID_ADDRESSABILITY

**Prompts**
- Requirement Lineage Binder - Map each requirement ID to normalized text and raw source material.
- Source Binding Review - Find requirement IDs that lack clear raw intent lineage.

---

### 🟥 Substep 04 - Protect ID Lifecycle
*Prevent accidental identity drift.*

* **🟥 AI Actions:** Detect renamed, retired, rejected, or reused IDs and record lifecycle status.
* **🟦 Human Actions:** Decide whether an ID is active, retired, superseded, or rejected.

**Inputs:** Requirement ID trace map and prior ID records if available.

**Outputs:** Requirement ID lifecycle register.

**Invariants:** CDD_P01_REQUIREMENT_ID_STABILITY, CDD_P01_REQUIREMENT_ID_NON_REUSE

**Prompts**
- ID Lifecycle Auditor - Find reused, renamed, retired, or unstable requirement IDs.
- Requirement ID Exit Review - Check that every requirement can be referenced safely downstream.
