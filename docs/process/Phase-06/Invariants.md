# Phase 06 - Test Generation Invariants

## Overview

These invariants define the phase-specific truths that must hold for Phase 06 - Test Generation (Proof Construction).
They specialize the global CDD test, proof, coverage, determinism, contract, traceability, and governance invariants for compiling constraints into executable proof artifacts.

No simulation or implementation work may rely on a test suite until this invariant set is satisfied or an explicit governance exception is recorded.

---

## [Step 01 - Load Constraints](./Steps/Step-01/)
**CDD_P06_CONSTRAINT_SOURCE_REQUIRED**
Phase 06 must load the published Phase 04 constraint set as the proof authority.

**CDD_P06_CONSTRAINT_ID_REQUIRED**
Only constraints with stable CONSTRAINT_IDs may be used for authoritative test generation.

**CDD_P06_CONSTRAINT_BASELINE_VISIBLE**
The constraint baseline version, publication identity, or revision state must be visible.

**CDD_P06_CONSTRAINT_PNB_FAILURE_VISIBLE**
Positive, negative, boundary, and failure semantics must be available to test generation.

**CDD_P06_CONSTRAINT_NO_INFORMAL_AUTHORITY**
Unpublished constraints, notes, or manual expectations must not authorize tests.

**CDD_P06_CONSTRAINT_INPUT_DEFECT_ESCALATION**
Missing IDs, missing failure semantics, contradictions, or incomplete mappings must be escalated upstream rather than silently patched in tests.

---

## [Step 02 - Align Terminology](./Steps/Step-02/)
**CDD_P06_GLOSSARY_ALIGNMENT_REQUIRED**
Test names, fixtures, cases, and assertions must align with canonical glossary terms.

**CDD_P06_GLOSSARY_MEANING_PRESERVATION**
Tests must preserve constraint and contract meanings.

**CDD_P06_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms must block authoritative test publication unless resolved or explicitly excepted.

**CDD_P06_GLOSSARY_NO_TEST_TERM_INVENTION**
Tests must not introduce new domain terminology without glossary grounding.

**CDD_P06_GLOSSARY_DRIFT_VISIBILITY**
Any term meaning shift between constraints, contracts, and tests must be recorded as drift.

---

## [Step 03 - Bind to Contracts](./Steps/Step-03/)
**CDD_P06_CONTRACT_BINDING_REQUIRED**
Boundary-relevant tests must bind to the published contract set.

**CDD_P06_CONTRACT_BASELINE_VISIBLE**
The contract baseline version, publication identity, or revision state must be visible.

**CDD_P06_CONTRACT_SEMANTIC_ALIGNMENT**
Tests must use contract semantics without adding interaction behavior.

**CDD_P06_CONTRACT_BOUNDARY_COVERAGE**
Tests must cover contract-bound interactions required by constraints.

**CDD_P06_CONTRACT_NO_SIDE_CHANNEL_TESTING**
Tests must not depend on hidden interaction paths outside contracts.

**CDD_P06_CONTRACT_GAP_VISIBILITY**
Constraints that cannot be bound to required contracts must be recorded as gaps.

---

## [Step 04 - Generate Positive Tests](./Steps/Step-04/)
**CDD_P06_POSITIVE_TEST_REQUIRED**
Constraints with required or allowed behavior must have positive proof tests.

**CDD_P06_POSITIVE_TEST_CONSTRAINT_AUTHORITY**
Positive tests must derive from constraint-admitted behavior.

**CDD_P06_POSITIVE_ASSERTION_EXPLICITNESS**
Positive tests must assert expected outcomes explicitly.

**CDD_P06_POSITIVE_NO_OVERBROAD_ACCEPTANCE**
Positive tests must not admit behavior beyond the governing constraints.

**CDD_P06_POSITIVE_TRACEABILITY**
Each positive test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_POSITIVE_GAP_VISIBILITY**
Missing positive proof must be recorded as a coverage gap.

---

## [Step 05 - Generate Negative Tests](./Steps/Step-05/)
**CDD_P06_NEGATIVE_TEST_REQUIRED**
Constraints with forbidden behavior must have negative proof tests.

**CDD_P06_NEGATIVE_TEST_CONSTRAINT_AUTHORITY**
Negative tests must derive from constraint-forbidden behavior or negative-space definitions.

**CDD_P06_NEGATIVE_REJECTION_EXPLICITNESS**
Negative tests must assert rejection, failure, or non-admission explicitly.

**CDD_P06_NEGATIVE_NO_INVENTED_INVALIDITY**
Negative tests must not forbid behavior absent from governing constraints.

**CDD_P06_NEGATIVE_TRACEABILITY**
Each negative test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_NEGATIVE_GAP_VISIBILITY**
Missing negative proof must be recorded as a coverage gap.

---

## [Step 06 - Generate Boundary Tests](./Steps/Step-06/)
**CDD_P06_BOUNDARY_TEST_REQUIRED**
Constraints with edge conditions must have boundary proof tests.

**CDD_P06_BOUNDARY_TEST_CONSTRAINT_AUTHORITY**
Boundary tests must derive from constraint boundary semantics or contract boundary definitions.

**CDD_P06_BOUNDARY_LIMIT_EXPLICITNESS**
Limits, thresholds, transitions, empty states, and edge cases must be explicit where governed.

**CDD_P06_BOUNDARY_NO_INVENTED_EDGES**
Boundary tests must not invent edge semantics absent from constraints or contracts.

**CDD_P06_BOUNDARY_TRACEABILITY**
Each boundary test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_BOUNDARY_GAP_VISIBILITY**
Missing boundary proof must be recorded as a coverage gap.

---

## [Step 07 - Generate Failure-Path Tests](./Steps/Step-07/)
**CDD_P06_FAILURE_TEST_REQUIRED**
Constraints with failure semantics must have failure-path proof tests.

**CDD_P06_FAILURE_TEST_CONSTRAINT_AUTHORITY**
Failure tests must derive from explicit constraint or contract failure semantics.

**CDD_P06_FAILURE_ASSERTION_EXPLICITNESS**
Failure tests must assert failure behavior, detection, response, or containment explicitly.

**CDD_P06_FAILURE_NO_INVENTED_FAILURE**
Failure tests must not create failure modes absent from governing artifacts.

**CDD_P06_FAILURE_TRACEABILITY**
Each failure-path test must map to the CONSTRAINT_IDs it proves.

**CDD_P06_FAILURE_GAP_VISIBILITY**
Missing failure proof must be recorded as a coverage gap.

---

## [Step 08 - Map Tests to CONSTRAINT_IDs](./Steps/Step-08/)
**CDD_P06_TEST_MAPPING_REQUIRED**
Every authoritative test must map to one or more CONSTRAINT_IDs.

**CDD_P06_TEST_NO_ORPHANS**
No published test may lack constraint lineage.

**CDD_P06_CONSTRAINT_TO_TEST_TRACEABILITY**
Each constraint must expose its mapped tests.

**CDD_P06_TEST_TO_CONSTRAINT_TRACEABILITY**
Each test must expose its governing constraints.

**CDD_P06_MAPPING_STABILITY**
Mappings must remain stable across wording refinements unless authority changes.

**CDD_P06_MAPPING_GAP_VISIBILITY**
Unmapped tests and untested constraints must be recorded as gaps.

---

## [Step 09 - Enforce Determinism](./Steps/Step-09/)
**CDD_P06_TEST_DETERMINISM_REQUIRED**
Generated tests must execute deterministically.

**CDD_P06_NO_RUNTIME_INTERPRETATION**
Tests must not require unresolved interpretation at runtime.

**CDD_P06_CONTROLLED_INPUTS**
Time, randomness, ordering, environment, network, concurrency, and external state must be controlled or eliminated.

**CDD_P06_REPRODUCIBLE_EXPECTATIONS**
Expected outcomes must be stable and reproducible from the constraint and contract baselines.

**CDD_P06_DETERMINISM_CONFIGURATION_VISIBLE**
Determinism controls and execution configuration must be visible.

**CDD_P06_FLAKINESS_BLOCKS_PUBLICATION**
Known nondeterminism or flaky behavior blocks authoritative publication.

---

## [Step 10 - Compute Coverage](./Steps/Step-10/)
**CDD_P06_COVERAGE_COMPUTATION_REQUIRED**
Constraint-level coverage must be computed before review.

**CDD_P06_COVERAGE_CONSTRAINT_COMPLETE**
Every constraint must have at least one mapped proof test or a governed exception.

**CDD_P06_COVERAGE_PNB_FAILURE_INCLUDED**
Coverage must include positive, negative, boundary, and failure semantics where applicable.

**CDD_P06_COVERAGE_ID_LINKED**
Coverage evidence must be linked to CONSTRAINT_IDs.

**CDD_P06_COVERAGE_SEMANTIC_NOT_LINE_BASED**
Coverage must be measured against constraint semantics, not source lines.

**CDD_P06_COVERAGE_GAP_VISIBILITY**
Coverage gaps must be recorded with affected CONSTRAINT_IDs.

---

## [Step 11 - Review Gate](./Steps/Step-11/)
**CDD_P06_REVIEW_GATE_REQUIRED**
The generated test suite must pass a review gate before publication.

**CDD_P06_REVIEW_MAPPING_EVIDENCE**
Review must validate test-to-CONSTRAINT_ID mapping evidence.

**CDD_P06_REVIEW_COVERAGE_EVIDENCE**
Review must validate constraint-level coverage evidence.

**CDD_P06_REVIEW_DETERMINISM_EVIDENCE**
Review must validate deterministic execution evidence.

**CDD_P06_REVIEW_CONTRACT_BINDING_EVIDENCE**
Review must validate contract binding for boundary-relevant tests.

**CDD_P06_REVIEW_EXCEPTION_VISIBILITY**
Any exception to Phase 06 invariants must be visible, justified, owned, and reconciliation-bound.

**CDD_P06_REVIEW_NO_CEREMONIAL_APPROVAL**
Review approval without proof evidence does not grant downstream authority.

---

## [Step 12 - Publish Test Suite](./Steps/Step-12/)
**CDD_P06_PUBLICATION_REQUIRED**
The authoritative test suite must be published before simulation or implementation uses it as proof.

**CDD_P06_PUBLICATION_SINGLE_AUTHORITY**
Downstream phases must resolve proof obligations through the published test suite.

**CDD_P06_PUBLICATION_CONTENT_COMPLETE**
Publication must include tests, mappings, coverage report, deterministic execution configuration, gaps, and governed exceptions.

**CDD_P06_PUBLICATION_ACCESSIBILITY**
Published tests must be accessible to downstream actors and tools that execute proof against doubles and implementations.

**CDD_P06_PUBLICATION_VERSION_VISIBILITY**
The published test suite must expose its version, baseline identity, or revision state.

**CDD_P06_PUBLICATION_NO_ORPHAN_TESTS**
No published test may lack constraint lineage or governance status.

---

## Cross-Phase Exit Invariants

**CDD_P06_EXIT_ALL_CONSTRAINTS_TESTED**
Every constraint exiting Phase 06 must have mapped proof coverage or a governed exception.

**CDD_P06_EXIT_PNB_FAILURE_PROOF**
Positive, negative, boundary, and failure proof tests must exist where applicable.

**CDD_P06_EXIT_DETERMINISTIC_REPRODUCIBLE**
The test suite exiting Phase 06 must be deterministic and reproducible.

**CDD_P06_EXIT_CONTRACT_BOUND**
Boundary-relevant tests must be bound to published contracts.

**CDD_P06_EXIT_TRACEABLE_TO_CONSTRAINTS**
Every test exiting Phase 06 must be traceable to CONSTRAINT_IDs.

**CDD_P06_EXIT_READY_FOR_SIMULATION**
The Phase 06 output must be suitable for execution against test doubles without adding proof semantics.

**CDD_P06_EXIT_NO_DOWNSTREAM_AUTHORITY_WITHOUT_GATE**
No downstream artifact may claim authority from Phase 06 unless the Phase 06 gate is passed or explicitly excepted.

---

## Final Compression

Phase 06 requires that constraints become deterministic, contract-bound, CONSTRAINT_ID-mapped proof tests with semantic coverage over allowed, forbidden, boundary, and failure behavior before simulation or implementation can claim proof authority.
