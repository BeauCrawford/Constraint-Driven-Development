# Phase 04 - Constraint Derivation Invariants

## Overview

These invariants define the phase-specific truths that must hold for Phase 04 - Constraint Derivation.
They specialize the global CDD constraint, traceability, semantic closure, glossary, determinism, and governance invariants for the transition from invariant truth to executable rule authority.

No test generation may begin until this invariant set is satisfied or an explicit governance exception is recorded.

---

## [Step 01 - Load Validated Invariants](./Steps/Step-01/README.md)

**CDD_P04_VALIDATED_INVARIANT_SOURCE_REQUIRED**
Phase 04 must load only closure-validated invariants as its semantic source.

**CDD_P04_CLOSURE_REPORT_REQUIRED**
The closure report validating the invariant set must be available before derivation begins.

**CDD_P04_INVARIANT_BASELINE_IDENTITY_VISIBLE**
The invariant baseline version, publication identity, or revision state must be visible.

**CDD_P04_INVARIANT_LINEAGE_VISIBLE**
Requirement-to-invariant lineage must remain visible during constraint derivation.

**CDD_P04_INVARIANT_NO_UNVALIDATED_AUTHORITY**
Unvalidated invariant candidates must not grant constraint authority.

**CDD_P04_INVARIANT_INPUT_DEFECT_ESCALATION**
Missing closure evidence, missing lineage, or unresolved invariant defects must be escalated upstream rather than silently repaired in Phase 04.

---

## [Step 02 - Resolve Terminology](./Steps/Step-02/README.md)

**CDD_P04_GLOSSARY_ALIGNMENT_REQUIRED**
Constraint language must align with canonical glossary terms used by the validated invariants.

**CDD_P04_GLOSSARY_MEANING_PRESERVATION**
Constraint wording must preserve invariant meaning and glossary definitions.

**CDD_P04_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms must block constraint publication unless resolved or explicitly excepted.

**CDD_P04_GLOSSARY_NO_TERM_INVENTION**
Constraint derivation must not introduce new domain terminology without glossary grounding.

**CDD_P04_GLOSSARY_EXECUTION_TERM_BOUNDARY**
Executable precision may add operational structure but must not change domain meaning.

**CDD_P04_GLOSSARY_DRIFT_VISIBILITY**
Any term meaning shift between invariants and constraints must be recorded as drift.

---

## [Step 03 - Partition Invariants](./Steps/Step-03/README.md)

**CDD_P04_RULE_UNIT_PARTITION_REQUIRED**
Validated invariants must be partitioned into enforceable rule units before constraint derivation.

**CDD_P04_RULE_UNIT_PARENT_BINDING**
Each rule unit must link to the invariant that authorizes it.

**CDD_P04_RULE_UNIT_ATOMICITY**
Each rule unit must represent a coherent enforceable behavior boundary.

**CDD_P04_RULE_UNIT_NO_SEMANTIC_LOSS**
Partitioning must not drop invariant meaning.

**CDD_P04_RULE_UNIT_NO_SEMANTIC_ADDITION**
Partitioning must not add behavior absent from the validated invariant set.

**CDD_P04_RULE_UNIT_POS_NEG_BOUNDARY_READINESS**
Rule units must be suitable for positive, negative, and boundary case definition.

**CDD_P04_RULE_UNIT_GAP_VISIBILITY**
Invariant meaning that cannot be partitioned cleanly must be recorded as a derivation gap.

---

## [Step 04 - Derive Constraint Candidates](./Steps/Step-04/README.md)

**CDD_P04_CONSTRAINT_DERIVATION_REQUIRED**
Each rule unit must be evaluated for constraint derivation.

**CDD_P04_CONSTRAINT_INVARIANT_AUTHORITY**
Every constraint candidate must derive from one or more validated invariants.

**CDD_P04_CONSTRAINT_EXECUTABLE_PRECISION**
Each constraint candidate must be precise enough to define enforceable behavior.

**CDD_P04_CONSTRAINT_NO_INVENTED_BEHAVIOR**
Constraint candidates must not introduce behavior beyond invariant authority.

**CDD_P04_CONSTRAINT_ALLOWED_FORBIDDEN_BOUNDARY_ORIENTATION**
Constraint candidates must orient toward allowed, forbidden, and boundary behavior.

**CDD_P04_CONSTRAINT_FAILURE_DETECTABILITY**
Constraint candidates must be capable of producing detectable pass or failure semantics downstream.

**CDD_P04_CONSTRAINT_TRACEABILITY**
Each constraint candidate must retain lineage to invariant IDs or statements and parent requirement IDs.

**CDD_P04_CONSTRAINT_REVIEWABILITY**
Constraint candidates must be inspectable before publication.

---

## [Step 05 - Define Positive / Negative / Boundary Cases](./Steps/Step-05/README.md)

**CDD_P04_PNB_CASES_REQUIRED**
Constraints must define positive, negative, and boundary behavior when semantically applicable.

**CDD_P04_POSITIVE_CASE_AUTHORITY**
Positive cases must describe behavior admitted by invariant authority.

**CDD_P04_NEGATIVE_CASE_AUTHORITY**
Negative cases must describe behavior forbidden by invariant authority or negative-space definitions.

**CDD_P04_BOUNDARY_CASE_AUTHORITY**
Boundary cases must describe edge conditions implied by invariant meaning, scope, or glossary definitions.

**CDD_P04_PNB_NO_UNAUTHORIZED_EXPANSION**
Positive, negative, and boundary cases must not expand behavior beyond validated invariants.

**CDD_P04_PNB_COMPLETENESS**
Missing positive, negative, or boundary semantics must be recorded as a derivation gap.

**CDD_P04_PNB_TEST_READINESS**
Positive, negative, and boundary cases must be precise enough to support later proof construction.

---

## [Step 06 - Encode Failure Semantics](./Steps/Step-06/README.md)

**CDD_P04_FAILURE_SEMANTICS_REQUIRED**
Each constraint must define how violation is recognized or represented.

**CDD_P04_FAILURE_CONDITION_EXPLICITNESS**
Failure conditions must be explicit and tied to constraint semantics.

**CDD_P04_FAILURE_NO_IMPLEMENTATION_LOCK_IN**
Failure semantics must not prescribe implementation mechanisms unless required by upstream authority.

**CDD_P04_FAILURE_BOUNDARY_ALIGNMENT**
Failure semantics must align with negative and boundary cases.

**CDD_P04_FAILURE_DETERMINISM**
Failure semantics must be deterministic enough to support reproducible proof.

**CDD_P04_FAILURE_TRACEABILITY**
Failure semantics must remain traceable to the constraints and invariants that authorize them.

---

## [Step 07 - Assign CONSTRAINT_IDs](./Steps/Step-07/README.md)

**CDD_P04_CONSTRAINT_ID_REQUIRED**
Every published constraint must have a stable CONSTRAINT_ID.

**CDD_P04_CONSTRAINT_ID_UNIQUENESS**
No two constraints may share the same CONSTRAINT_ID.

**CDD_P04_CONSTRAINT_ID_STABILITY**
CONSTRAINT_IDs must not change because wording is refined.

**CDD_P04_CONSTRAINT_ID_NON_REUSE**
Retired or rejected CONSTRAINT_IDs must not be reused for different rule authority.

**CDD_P04_CONSTRAINT_ID_TRACE_BINDING**
Each CONSTRAINT_ID must bind constraint text to its authorizing invariant lineage.

**CDD_P04_CONSTRAINT_ID_ADDRESSABILITY**
Each constraint must be directly referable by ID in tests, coverage reports, reviews, gaps, and exceptions.

---

## [Step 08 - Check Non-Contradiction & Satisfiability](./Steps/Step-08/README.md)

**CDD_P04_CONSISTENCY_CHECK_REQUIRED**
The constraint set must be checked for contradiction before publication.

**CDD_P04_CONSTRAINT_NON_CONTRADICTION**
No constraint may make another constraint impossible to satisfy unless the conflict is resolved.

**CDD_P04_SATISFIABILITY_REQUIRED**
The constraint set must admit at least one valid implementation or explicitly identify an upstream contradiction.

**CDD_P04_CONFLICT_LINEAGE**
Constraint conflicts must identify affected constraints, invariants, and requirement lineage.

**CDD_P04_CONFLICT_NO_SILENT_OVERRIDE**
A constraint must not override another constraint without a visible resolution artifact.

**CDD_P04_CONFLICT_UPSTREAM_ESCALATION**
Conflicts caused by invariant or requirement issues must be escalated upstream rather than patched in Phase 04.

**CDD_P04_CONFLICT_BLOCKS_PUBLICATION**
Unresolved constraint contradictions block publication.

---

## [Step 09 - Ensure Completeness vs Invariants](./Steps/Step-09/README.md)

**CDD_P04_COMPLETENESS_CHECK_REQUIRED**
The constraint set must be checked for complete enforcement of validated invariants.

**CDD_P04_INVARIANT_TO_CONSTRAINT_COVERAGE**
Every validated invariant must map to one or more constraints or a governed exception.

**CDD_P04_CONSTRAINT_TO_INVARIANT_COVERAGE**
Every constraint must map back to one or more validated invariants.

**CDD_P04_NEGATIVE_SPACE_ENFORCEMENT**
Negative-space definitions must be enforced by constraints where applicable.

**CDD_P04_COMPLETENESS_NO_ORPHAN_RULES**
No constraint may exist without invariant authority.

**CDD_P04_COMPLETENESS_GAP_VISIBILITY**
Missing constraint coverage must be recorded as a gap with impacted invariants.

**CDD_P04_COMPLETENESS_GATE_BOUND**
Blocking completeness gaps must prevent review approval and publication.

---

## [Step 10 - Review Gate](./Steps/Step-10/README.md)

**CDD_P04_REVIEW_GATE_REQUIRED**
The constraint set must pass a review gate before publication.

**CDD_P04_REVIEW_PRECISION_EVIDENCE**
Review must include evidence that constraints are executable and precise.

**CDD_P04_REVIEW_COVERAGE_EVIDENCE**
Review must include invariant-to-constraint coverage evidence.

**CDD_P04_REVIEW_ID_EVIDENCE**
Review must validate CONSTRAINT_ID uniqueness, stability, and addressability.

**CDD_P04_REVIEW_CONSISTENCY_EVIDENCE**
Review must validate non-contradiction and satisfiability evidence.

**CDD_P04_REVIEW_TRACEABILITY_EVIDENCE**
Review must validate requirement-to-invariant-to-constraint lineage.

**CDD_P04_REVIEW_EXCEPTION_VISIBILITY**
Any exception to Phase 04 invariants must be visible, justified, owned, and reconciliation-bound.

**CDD_P04_REVIEW_NO_CEREMONIAL_APPROVAL**
Review approval without evidence does not grant downstream authority.

---

## [Step 11 - Publish Constraint Set](./Steps/Step-11/README.md)

**CDD_P04_PUBLICATION_REQUIRED**
The authoritative constraint set must be published before test generation begins.

**CDD_P04_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve executable rule authority through the published constraint set.

**CDD_P04_PUBLICATION_CONTENT_COMPLETE**
Publication must include constraint statements, CONSTRAINT_IDs, invariant mappings, positive/negative/boundary cases, failure semantics, consistency report, gaps, and governed exceptions.

**CDD_P04_PUBLICATION_ACCESSIBILITY**
Published constraints must be accessible to downstream actors and tools that perform test generation.

**CDD_P04_PUBLICATION_VERSION_VISIBILITY**
The published constraint set must expose its version, baseline identity, or revision state.

**CDD_P04_PUBLICATION_NO_ORPHAN_CONSTRAINTS**
No published constraint may lack invariant lineage or governance status.

**CDD_P04_PUBLICATION_EXECUTION_AUTHORITY_BOUNDARY**
Published constraints define the first executable authority boundary for downstream tests and implementation.

---

## Cross-Phase Exit Invariants

**CDD_P04_EXIT_ALL_INVARIANTS_ENFORCED**
Every validated invariant exiting Phase 04 must be enforced by one or more constraints or a governed exception.

**CDD_P04_EXIT_CONSTRAINTS_EXECUTABLE_PRECISE**
Every constraint exiting Phase 04 must be precise enough for deterministic proof construction.

**CDD_P04_EXIT_CONSTRAINTS_IDENTITY_STABLE**
Every constraint exiting Phase 04 must have a unique, stable CONSTRAINT_ID.

**CDD_P04_EXIT_PNB_AND_FAILURE_DEFINED**
Positive, negative, boundary, and failure semantics must be defined where applicable.

**CDD_P04_EXIT_NON_CONTRADICTORY_SATISFIABLE**
The constraint set exiting Phase 04 must be non-contradictory and satisfiable.

**CDD_P04_EXIT_TRACEABLE_TO_INVARIANTS**
Every constraint exiting Phase 04 must be traceable to validated invariants and parent requirements.

**CDD_P04_EXIT_READY_FOR_TEST_GENERATION**
The Phase 04 output must be suitable for test generation without adding new semantic authority.

**CDD_P04_EXIT_NO_DOWNSTREAM_AUTHORITY_WITHOUT_GATE**
No downstream artifact may claim authority from Phase 04 unless the Phase 04 gate is passed or explicitly excepted.

---

## Final Compression

Phase 04 requires that closure-validated invariants become precise, addressable, non-contradictory, satisfiable, traceable constraints with explicit positive, negative, boundary, and failure semantics before executable proof is generated.
