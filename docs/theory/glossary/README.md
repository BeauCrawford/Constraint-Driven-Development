# **Constraint-Driven Development — Glossary**

See [Constraint-Driven Development Invariants](/docs/invariants/README.md) for the canonical invariant catalog that defines the non-negotiable semantic rules behind these terms and governs how CDD lowers intent into proof-backed implementation.

---

## **Requirement**

**Definition:**  
A structured, explicitly defined statement of intended system behavior grounded in domain terminology and suitable for semantic lowering.

**Invariants:**  
CDD_REQUIREMENT_EXPLICITNESS, CDD_REQUIREMENT_ADDRESSABILITY, CDD_REQUIREMENT_SOURCE_AUTHORITY

**Constraints Impacted:**  
All constraints derive (indirectly) from requirements via invariants.

**Notes:**  
Requirements do not execute and must not contain implementation detail.

**Synonyms (disallowed or mapped):**  
- Spec → REQUIREMENT  
- User Story → REQUIREMENT  

---

## **Invariant**

**Definition:**  
An irreducible, implementation-independent truth that must always hold for the system.

**Invariants:**  
CDD_INVARIANT_IRREDUCIBLE_TRUTH, CDD_INVARIANT_IMPLEMENTATION_INDEPENDENCE, CDD_INVARIANT_EXHAUSTIVENESS

**Constraints Impacted:**  
All constraints must derive from invariants.

**Notes:**  
This is the semantic compression layer where intent becomes governable.

**Synonyms (disallowed or mapped):**  
- Rule → INVARIANT  
- Principle → INVARIANT  

---

## **Constraint**

**Definition:**  
An executable, enforceable rule derived from invariants that defines allowed, forbidden, and boundary behavior.

**Invariants:**  
CDD_CONSTRAINT_DERIVED_FROM_INVARIANTS, CDD_CONSTRAINT_UNIQUE_IDENTITY, CDD_CONSTRAINT_EXECUTABLE_PRECISION

**Constraints Impacted:**  
All system behavior is defined by constraints.

**Notes:**  
Constraints are the first mechanically enforceable form of truth.

**Synonyms (disallowed or mapped):**  
- Validation Rule → CONSTRAINT  
- Guard → CONSTRAINT  

---

## **Constraint ID**

**Definition:**  
A unique, stable identifier assigned to a constraint to enable traceability and mechanical enforcement.

**Invariants:**  
CDD_CONSTRAINT_UNIQUE_IDENTITY, CDD_TRACEABILITY_STABLE_IDS

**Constraints Impacted:**  
All constraints must have IDs.

**Notes:**  
Without IDs, traceability and coverage collapse.

**Synonyms (disallowed or mapped):**  
- Rule ID → CONSTRAINT_ID  

---

## **Test**

**Definition:**  
A deterministic executable artifact generated from constraints that proves constraint satisfaction.

**Invariants:**  
CDD_TEST_DERIVED_FROM_CONSTRAINTS, CDD_TEST_RUNTIME_DETERMINISM, CDD_TEST_CONSTRAINT_MAPPING

**Constraints Impacted:**  
All constraints must map to tests.

**Notes:**  
Tests are proof artifacts, not validation examples.

**Synonyms (disallowed or mapped):**  
- Unit Test → TEST  
- Spec Test → TEST  

---

## **Proof**

**Definition:**  
A deterministic verification that a constraint holds under all defined conditions.

**Invariants:**  
CDD_FOUNDATION_PROOF_BOUND_AUTHORITY, CDD_TEST_POSITIVE_PROOF, CDD_TEST_NEGATIVE_PROOF

**Constraints Impacted:**  
All constraints require proof.

**Notes:**  
Proof replaces confidence-based validation.

**Synonyms (disallowed or mapped):**  
- Validation → PROOF  

---

## **Semantic Closure**

**Definition:**  
The condition where a child layer fully and faithfully represents all relevant meaning of its parent layer.

**Invariants:**  
CDD_CLOSURE_PARENT_CHILD_COVERAGE, CDD_CLOSURE_NO_SILENT_LOSS, CDD_CLOSURE_NO_UNAUTHORIZED_ADDITION

**Constraints Impacted:**  
All constraints must exist within closed semantic boundaries.

**Notes:**  
Closure is measured as containment, not similarity.

**Synonyms (disallowed or mapped):**  
- Completeness → SEMANTIC_CLOSURE  

**See:**

- [Semantic Closure](./Semantic-Closure.md)

---

## **Monotonic Lowering**

**Definition:**  
A directional transformation process where each layer refines but does not expand or alter upstream meaning.

**Invariants:**  
CDD_LOWERING_MONOTONIC_CONTAINMENT, CDD_LOWERING_NO_EXPANSION, CDD_LOWERING_REFINEMENT_ONLY

**Constraints Impacted:**  
Constraints must not introduce new semantics.

**Notes:**  
This is what enables measurability.

**Synonyms (disallowed or mapped):**  
- Compilation → MONOTONIC_LOWERING  

---

## **Traceability**

**Definition:**  
The ability to map any artifact back to its originating requirement through all intermediate layers.

**Invariants:**  
CDD_TRACEABILITY_END_TO_END, CDD_TRACEABILITY_NO_ORPHANS

**Constraints Impacted:**  
All constraints must be traceable.

**Notes:**  
Traceability is required for governance and debugging.

**Synonyms (disallowed or mapped):**  
- Lineage → TRACEABILITY  

---

## **Contract**

**Definition:**  
An explicit boundary definition describing interaction semantics between system components.

**Invariants:**  
CDD_CONTRACT_BOUNDARY_EXTERNALIZATION, CDD_CONTRACT_SEMANTIC_CARRIER

**Constraints Impacted:**  
Constraints governing interactions must be reflected in contracts.

**Notes:**  
Contracts define the system boundary before implementation exists.

**Synonyms (disallowed or mapped):**  
- Interface → CONTRACT  

---

## **Test Double**

**Definition:**  
A generated substitute implementation used to simulate contract behavior during testing.

**Invariants:**  
CDD_DOUBLE_CONTRACT_BOUND, CDD_DOUBLE_DETERMINISTIC_BEHAVIOR

**Constraints Impacted:**  
Used to validate constraints at boundaries.

**Notes:**  
Must not introduce new semantics.

**Synonyms (disallowed or mapped):**  
- Mock → TEST_DOUBLE  
- Stub → TEST_DOUBLE  

---

## **Boundary**

**Definition:**  
The interface surface where system components interact.

**Invariants:**  
CDD_CONTRACT_BOUNDARY_EXTERNALIZATION, CDD_ARCH_BOUNDARY_FIRST

**Constraints Impacted:**  
Boundary constraints define interaction correctness.

**Notes:**  
Most failures occur at boundaries.

**Synonyms (disallowed or mapped):**  
- Integration Point → BOUNDARY  

---

## **Coverage**

**Definition:**  
The degree to which constraints are proven through tests.

**Invariants:**  
CDD_COVERAGE_CONSTRAINT_COMPLETE, CDD_COVERAGE_SEMANTIC

**Constraints Impacted:**  
All constraints must be covered.

**Notes:**  
Coverage is semantic, not line-based.

**Synonyms (disallowed or mapped):**  
- Test Coverage → COVERAGE  

---

## **Determinism**

**Definition:**  
The property that execution produces the same result given the same inputs.

**Invariants:**  
CDD_DETERMINISM_RUNTIME_PURITY, CDD_TEST_DETERMINISTIC_EXECUTION

**Constraints Impacted:**  
Tests and constraints must be deterministic.

**Notes:**  
Required for proof integrity.

**Synonyms (disallowed or mapped):**  
- Repeatability → DETERMINISM  

---

## **Drift**

**Definition:**  
Loss of semantic alignment between layers.

**Invariants:**  
CDD_CLOSURE_DRIFT_DEFINITION, CDD_CHANGE_DRIFT_DETECTION

**Constraints Impacted:**  
Constraints must be updated to eliminate drift.

**Notes:**  
Drift is a primary failure mode.

**Synonyms (disallowed or mapped):**  
- Misalignment → DRIFT  

---

## **Pressure Exit**

**Definition:**  
A point in the system where semantic, structural, or governance containment can fail.

**Invariants:**  
CDD_META_STATE_SPACE_COLLAPSE, CDD_CLOSURE_NO_SILENT_LOSS

**Constraints Impacted:**  
Constraints must eliminate or govern pressure exits.

**Notes:**  
These are structural failure paths.

**Synonyms (disallowed or mapped):**  
- Leak → PRESSURE_EXIT  

---

## **State Space**

**Definition:**  
The total set of possible system behaviors.

**Invariants:**  
CDD_META_STATE_SPACE_COLLAPSE

**Constraints Impacted:**  
Constraints reduce state space.

**Notes:**  
CDD works by collapsing invalid possibilities.

**Synonyms (disallowed or mapped):**  
- Behavior Space → STATE_SPACE  

---

## **Admissible Behavior**

**Definition:**  
Behavior that satisfies all constraints and proof requirements.

**Invariants:**  
CDD_FOUNDATION_CONFORMANCE_OVER_INVENTION

**Constraints Impacted:**  
Defined entirely by constraints.

**Notes:**  
Anything outside this is invalid.

**Synonyms (disallowed or mapped):**  
- Valid Behavior → ADMISSIBLE_BEHAVIOR  

---

## **Nonfunctional Constraint**

**Definition:**  
A constraint governing system qualities such as performance, reliability, or security.

**Invariants:**  
CDD_CODEGEN_NO_UNPROVEN_BEHAVIOR

**Constraints Impacted:**  
Applies to operational characteristics.

**Notes:**  
Must be included in constraint system.

**Synonyms (disallowed or mapped):**  
- NFR → NONFUNCTIONAL_CONSTRAINT  

---

## **Execution Authority**

**Definition:**  
The right for code or behavior to exist and run within the system.

**Invariants:**  
CDD_FOUNDATION_EXECUTION_AUTHORITY_EMERGENCE

**Constraints Impacted:**  
Granted only through proof.

**Notes:**  
Authority is earned, not assumed.

**Synonyms (disallowed or mapped):**  
- Permission to Run → EXECUTION_AUTHORITY  

---

## **Residual Code**

**Definition:**  
Code that exists solely as a result of satisfying constraints and passing proof.

**Invariants:**  
CDD_FOUNDATION_CODE_AS_RESIDUE

**Constraints Impacted:**  
All code must be residual.

**Notes:**  
Code is not authored, it is derived.

**Synonyms (disallowed or mapped):**  
- Implementation → RESIDUAL_CODE  

---

## **Semantic Mass**

**Definition:**  
The density and completeness of structured meaning available to guide generation and enforcement.

**Invariants:**  
CDD_LLM_STRUCTURE_BOUND_USAGE

**Constraints Impacted:**  
Higher semantic mass improves constraint quality.

**Notes:**  
Directly impacts codegen cleanliness.

**Synonyms (disallowed or mapped):**  
- Signal Density → SEMANTIC_MASS  

---

## **Legitimacy**

**Definition:**  
The condition where behavior is fully derived, constrained, proven, and traceable.

**Invariants:**  
CDD_META_CONSTRAINT_DRIVEN_REALITY

**Constraints Impacted:**  
All constraints define legitimacy boundaries.

**Notes:**  
Legitimacy replaces correctness as the governing concept.

**Synonyms (disallowed or mapped):**  
- Correctness → LEGITIMACY  

---

## **Recompilation**

**Definition:**  
The process of regenerating downstream artifacts after upstream change.

**Invariants:**  
CDD_LOWERING_RECOMPILATION_OVER_PATCHING, CDD_CHANGE_DOWNSTREAM_RECOMPILATION

**Constraints Impacted:**  
Constraints must be regenerated after change.

**Notes:**  
Replaces patch-based updates.

**Synonyms (disallowed or mapped):**  
- Rebuild → RECOMPILATION  

---

## **Orphan Artifact**

**Definition:**  
An artifact with no traceable lineage to upstream intent.

**Invariants:**  
CDD_TRACEABILITY_NO_ORPHANS

**Constraints Impacted:**  
Such artifacts are invalid.

**Notes:**  
Indicates structural failure.

**Synonyms (disallowed or mapped):**  
- Untracked Logic → ORPHAN_ARTIFACT  

---

## **Final Compression**

**Definition:**  
The state where semantic closure, constraints, and proof reduce the system to a minimal admissible implementation.

**Invariants:**  
CDD_META_STATE_SPACE_COLLAPSE

**Constraints Impacted:**  
All constraints contribute to final compression.

**Notes:**  
This is where code becomes inevitable.

**Synonyms (disallowed or mapped):**  
- Convergence → FINAL_COMPRESSION  

---
