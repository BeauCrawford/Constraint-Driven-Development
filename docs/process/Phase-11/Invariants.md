# Phase 11 - Change & Recompilation Invariants

## Overview

These invariants define the phase-specific truths that must hold for Phase 11 - Change & Recompilation.
They specialize the global CDD change management, monotonic lowering, recompilation-over-patching, drift detection, traceability, coverage, closure, and governance invariants for system evolution.

No changed system state may be treated as valid until downstream artifacts are re-lowered, regenerated, and revalidated.

---

## [Step 01 - Submit Change Request](./Steps/Step-01/)
**CDD_P11_CHANGE_REQUEST_REQUIRED**
Change must be captured as a governed change request before downstream artifacts are altered.

**CDD_P11_CHANGE_SOURCE_ATTRIBUTION**
Each change request must identify its source, authority, and rationale.

**CDD_P11_CHANGE_INTENT_VISIBILITY**
Requested semantic change must be visible before implementation work begins.

**CDD_P11_NO_UNRECORDED_CHANGE**
Unrecorded edits to downstream artifacts must not grant change authority.

---

## [Step 02 - Classify Impact](./Steps/Step-02/)
**CDD_P11_IMPACT_CLASSIFICATION_REQUIRED**
Each change must be classified by the upstream layer it affects.

**CDD_P11_REVERSE_NAVIGATION_REQUIRED**
Traceability must be used to locate impacted upstream and downstream artifacts.

**CDD_P11_GLOSSARY_IMPACT_VISIBILITY**
Term changes must identify impacted requirements, invariants, constraints, tests, contracts, and code.

**CDD_P11_IMPACT_PATH_COMPLETENESS**
Impact classification must include all affected lineage paths or record gaps.

**CDD_P11_AMBIGUOUS_IMPACT_BLOCKS_PATCHING**
Ambiguous impact must block downstream patching until clarified.

---

## [Step 03 - Update Upstream Source](./Steps/Step-03/)
**CDD_P11_UPSTREAM_UPDATE_REQUIRED**
Behavioral change must originate in requirements, invariants, glossary, or another governing upstream artifact.

**CDD_P11_INTENT_PRECEDENCE**
Updated upstream intent governs all downstream regeneration.

**CDD_P11_NO_DOWNSTREAM_FIRST_CHANGE**
Constraints, tests, contracts, or code must not be patched first to create new authority.

**CDD_P11_UPSTREAM_CHANGE_TRACEABILITY**
Upstream changes must retain lineage to the change request and affected artifacts.

**CDD_P11_UPSTREAM_CONFLICT_VISIBILITY**
Conflicts introduced by upstream change must be detected and governed.

---

## [Step 04 - Re-Lower Affected Artifacts](./Steps/Step-04/)
**CDD_P11_RELOWERING_REQUIRED**
Affected artifacts must be re-lowered through the CDD pipeline.

**CDD_P11_MONOTONIC_RELOWERING**
Re-lowering must refine upstream meaning without expansion or invention.

**CDD_P11_NO_LAYER_SKIP**
Change propagation must not skip required intermediate layers.

**CDD_P11_RELOWERING_TRACEABILITY**
Each re-lowered artifact must retain lineage to the changed upstream source.

**CDD_P11_RELOWERING_GAP_VISIBILITY**
Artifacts that cannot be re-lowered cleanly must be recorded as gaps.

---

## [Step 05 - Regenerate Constraints, Tests, and Code](./Steps/Step-05/)
**CDD_P11_REGENERATION_REQUIRED**
Affected constraints, contracts, tests, doubles, and code must be regenerated or reconformed from updated upstream authority.

**CDD_P11_REGENERATION_OVER_PATCHING**
Regeneration is preferred over manual downstream patching.

**CDD_P11_TEST_REGENERATION_REQUIRED**
Affected tests must be regenerated from updated constraints.

**CDD_P11_CODE_RECONFORMANCE_REQUIRED**
Affected code must be reconformed to regenerated proof.

**CDD_P11_REGENERATION_NO_STALE_AUTHORITY**
Old artifacts must not retain authority when their upstream lineage changed.

**CDD_P11_REGENERATION_EVIDENCE_REQUIRED**
Regeneration must produce evidence of affected artifacts and unchanged artifacts.

---

## [Step 06 - Submit Regenerated Artifacts](./Steps/Step-06/)
**CDD_P11_REGENERATED_ARTIFACT_REVIEW_REQUIRED**
Regenerated artifacts must re-enter the appropriate governance gates.

**CDD_P11_REGENERATED_ARTIFACT_SCOPE_VISIBLE**
Submitted artifacts must identify what changed, what was regenerated, and what remained unchanged.

**CDD_P11_REGENERATED_ARTIFACT_LINEAGE_VISIBLE**
Submitted artifacts must preserve updated traceability.

**CDD_P11_REGENERATED_ARTIFACT_EXCEPTION_VISIBLE**
Any artifact not regenerated despite impact must be recorded as an exception.

---

## [Step 07 - Revalidate Closure and Coverage](./Steps/Step-07/)
**CDD_P11_CLOSURE_REVALIDATION_REQUIRED**
Closure must be revalidated after upstream change and re-lowering.

**CDD_P11_COVERAGE_REVALIDATION_REQUIRED**
Coverage must be revalidated after regenerated constraints and tests.

**CDD_P11_PROOF_REEXECUTION_REQUIRED**
Affected deterministic proof must be re-executed.

**CDD_P11_TRACEABILITY_REVALIDATION_REQUIRED**
Lineage must be revalidated after regenerated artifacts are produced.

**CDD_P11_REVALIDATION_GAP_VISIBILITY**
Revalidation gaps, failures, and exceptions must be visible.

---

## [Step 08 - Detect Stale Artifacts and Drift](./Steps/Step-08/)
**CDD_P11_STALE_ARTIFACT_DETECTION_REQUIRED**
Phase 11 must detect artifacts whose upstream authority changed without regeneration.

**CDD_P11_NO_STALE_ARTIFACT_AUTHORITY**
Stale artifacts must not retain execution or proof authority.

**CDD_P11_DRIFT_DETECTION_REQUIRED**
Semantic drift introduced or exposed by change must be detected.

**CDD_P11_DRIFT_RESOLUTION_REQUIRED**
Unresolved drift blocks change completion.

**CDD_P11_OBSOLETE_ARTIFACT_VISIBILITY**
Retired or superseded artifacts must be marked and traceable.

---

## [Step 09 - Publish Change Report](./Steps/Step-09/)
**CDD_P11_PUBLICATION_REQUIRED**
An authoritative change report must be published.

**CDD_P11_PUBLICATION_CONTENT_COMPLETE**
Publication must include change request, impact classification, upstream updates, regenerated artifacts, stale artifact detection, drift resolution, revalidation evidence, and exceptions.

**CDD_P11_PUBLICATION_SINGLE_AUTHORITY**
Governance must resolve change integrity through the published change report.

**CDD_P11_PUBLICATION_VERSION_VISIBILITY**
The change report must identify before and after artifact baselines.

**CDD_P11_PUBLICATION_NO_ORPHAN_CHANGE_EVIDENCE**
No change evidence may lack affected artifact lineage.

---

## Cross-Phase Exit Invariants

**CDD_P11_EXIT_CHANGE_ORIGINATED_UPSTREAM**
Change must originate in the governing upstream layer.

**CDD_P11_EXIT_DOWNSTREAM_REGENERATED**
Affected downstream artifacts must be regenerated or explicitly excepted.

**CDD_P11_EXIT_CLOSURE_COVERAGE_REVALIDATED**
Closure and coverage must be revalidated after change.

**CDD_P11_EXIT_NO_STALE_ARTIFACTS**
No stale artifact may retain authority.

**CDD_P11_EXIT_DRIFT_ELIMINATED**
No unresolved drift may remain.

**CDD_P11_EXIT_NO_DOWNSTREAM_AUTHORITY_WITHOUT_GATE**
No downstream artifact may claim authority from Phase 11 unless the Phase 11 gate is passed or explicitly excepted.

---

## Final Compression

Phase 11 requires that change enter through upstream authority, propagate by re-lowering and regeneration, and leave no stale or drifted artifacts behind.
