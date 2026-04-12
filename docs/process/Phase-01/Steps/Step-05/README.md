# Step 05 - Declare Scope Boundaries

---

## Description

Step 05, Declare Scope Boundaries, defines what Phase 01 requirements include, exclude, and leave unresolved. It prevents silent scope expansion or contraction by linking boundaries, edge questions, and external dependencies back to affected intent.

---

## Invariants

**CDD_P01_SCOPE_INCLUSION_EXPLICITNESS**
In-scope behavior must be explicitly identified.

**CDD_P01_SCOPE_EXCLUSION_EXPLICITNESS**
Out-of-scope behavior must be explicitly identified when raw intent or domain context could otherwise imply inclusion.

**CDD_P01_SCOPE_BOUNDARY_REQUIREMENT_LINKAGE**
Scope declarations must link to the affected requirement IDs or raw intent items.

**CDD_P01_SCOPE_EDGE_VISIBILITY**
Boundary cases that are neither clearly in scope nor out of scope must be recorded as open scope questions.

**CDD_P01_SCOPE_NO_SILENT_EXPANSION**
Normalization must not expand the system boundary beyond captured or approved intent.

**CDD_P01_SCOPE_NO_SILENT_CONTRACTION**
Normalization must not remove expected behavior from scope without recording the decision.

**CDD_P01_SCOPE_EXTERNAL_DEPENDENCY_VISIBILITY**
External systems, actors, data sources, and organizational boundaries must be visible when they affect requirement meaning.

---

## Substeps

### 🟥 Substep 01 - Identify In-Scope Behavior
*Make included behavior explicit.*

* **🟥 AI Actions:** Extract behaviors, actors, data, states, and interactions that are clearly in scope.
* **🟦 Human Actions:** Confirm inclusion decisions and add missing in-scope behavior.

**Inputs:** Normalized requirements and raw intent register.

**Outputs:** In-scope behavior list.

**Invariants:** CDD_P01_SCOPE_INCLUSION_EXPLICITNESS, CDD_P01_SCOPE_BOUNDARY_REQUIREMENT_LINKAGE

**Prompts**
- In-Scope Behavior Mapper - Identify behavior explicitly included by the requirement set.
- Scope Inclusion Review - Check whether any expected behavior is missing from the in-scope list.

---

### 🟥 Substep 02 - Identify Out-of-Scope Behavior
*Make exclusions explicit where ambiguity could imply inclusion.*

* **🟥 AI Actions:** Detect exclusions, deferred behavior, non-goals, and implied out-of-scope areas.
* **🟦 Human Actions:** Approve exclusions and resolve disputed boundaries.

**Inputs:** Raw intent, normalized requirements, and domain context.

**Outputs:** Out-of-scope behavior list.

**Invariants:** CDD_P01_SCOPE_EXCLUSION_EXPLICITNESS, CDD_P01_SCOPE_NO_SILENT_CONTRACTION

**Prompts**
- Out-of-Scope Detector - Find behavior that should be explicitly excluded from the requirement set.
- Exclusion Authority Review - Verify that each exclusion has stakeholder or scope authority.

---

### 🟥 Substep 03 - Link Scope to Requirements
*Tie scope decisions to affected intent.*

* **🟥 AI Actions:** Map each scope boundary to requirement IDs or raw intent items.
* **🟦 Human Actions:** Confirm boundary mappings and resolve missing links.

**Inputs:** In-scope list, out-of-scope list, requirement IDs, and raw intent register.

**Outputs:** Requirement-linked scope map.

**Invariants:** CDD_P01_SCOPE_BOUNDARY_REQUIREMENT_LINKAGE, CDD_P01_SCOPE_EXTERNAL_DEPENDENCY_VISIBILITY

**Prompts**
- Scope Boundary Mapper - Link scope inclusions and exclusions to affected requirements and raw intent.
- External Dependency Scope Pass - Identify external systems, actors, data sources, or organizational boundaries that affect scope.

---

### 🟥 Substep 04 - Surface Scope Edges
*Expose unclear boundary cases.*

* **🟥 AI Actions:** Identify cases that are neither clearly included nor excluded and record open scope questions.
* **🟦 Human Actions:** Decide whether edge cases become in scope, out of scope, or governed gaps.

**Inputs:** Requirement-linked scope map and domain context.

**Outputs:** Scope edge register.

**Invariants:** CDD_P01_SCOPE_EDGE_VISIBILITY, CDD_P01_SCOPE_NO_SILENT_EXPANSION

**Prompts**
- Scope Edge Finder - Identify unclear boundary cases that need stakeholder decision.
- Scope Drift Audit - Check whether normalization expanded or contracted scope without a recorded decision.
