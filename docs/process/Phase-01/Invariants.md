# Phase 01 - Requirement Formation Invariants

## Overview

These invariants define the phase-specific truths that must hold for Phase 01 - Requirement Formation.
They specialize the global CDD requirement, glossary, traceability, closure, and governance invariants for the requirement formation layer.

No downstream invariant extraction may begin until this invariant set is satisfied or an explicit governance exception is recorded.

---

## [Step 01 - Capture Intent Surface](./Steps/Step-01/README.md)

**CDD_P01_INTENT_SOURCE_VISIBILITY**
All raw stakeholder intent used by Phase 01 must be visible as an input artifact.

**CDD_P01_INTENT_SOURCE_ATTRIBUTION**
Every captured intent item must identify its originating source, stakeholder, document, or system context.

**CDD_P01_INTENT_UNTRANSFORMED_CAPTURE**
Initial capture must preserve raw intent before normalization or interpretation.

**CDD_P01_INTENT_NO_PREMATURE_FILTERING**
Raw intent must not be discarded because it appears ambiguous, conflicting, redundant, or difficult to implement.

**CDD_P01_INTENT_SIGNAL_RETENTION**
All behavioral expectations, constraints, goals, exclusions, risks, and acceptance language present in the source must remain available for normalization.

**CDD_P01_INTENT_CONTEXT_LINKAGE**
Captured intent must retain links to relevant domain context, existing system context, or source material when provided.

**CDD_P01_INTENT_CAPTURE_GAP_VISIBILITY**
Missing stakeholder input, missing source documents, or incomplete context must be recorded as visible gaps.

---

## [Step 02 - Normalize Language](./Steps/Step-02/README.md)

**CDD_P01_REQUIREMENT_STATEMENT_STRUCTURE**
Each normalized requirement must be expressed as a structured statement of intended system behavior.

**CDD_P01_REQUIREMENT_SINGLE_INTENT**
Each normalized requirement should contain one coherent intent unit suitable for invariant extraction.

**CDD_P01_REQUIREMENT_AMBIGUITY_REDUCTION**
Ambiguous language must be rewritten or flagged before the requirement can proceed.

**CDD_P01_REQUIREMENT_NARRATIVE_DRIFT_REMOVAL**
Narrative, motivational, or incidental language must not remain in the requirement body unless it carries required domain meaning.

**CDD_P01_REQUIREMENT_IMPLEMENTATION_ABSTINENCE**
Requirements must not prescribe implementation mechanisms unless the mechanism itself is a stakeholder intent or domain constraint.

**CDD_P01_REQUIREMENT_MODALITY_EXPLICITNESS**
Required, forbidden, optional, and conditional behavior must be explicitly distinguished.

**CDD_P01_REQUIREMENT_ACTOR_EXPLICITNESS**
Actors, systems, users, or external parties referenced by a requirement must be explicit or recorded as unresolved.

**CDD_P01_REQUIREMENT_CONDITION_EXPLICITNESS**
Triggering conditions, preconditions, and applicability boundaries must be explicit or recorded as gaps.

**CDD_P01_REQUIREMENT_OUTCOME_EXPLICITNESS**
Expected outcomes and externally observable effects must be explicit or recorded as gaps.

**CDD_P01_REQUIREMENT_RAW_TRACE_RETENTION**
Each normalized requirement must remain traceable to the raw intent it came from.

---

## [Step 03 - Apply Glossary Grounding](./Steps/Step-03/README.md)

**CDD_P01_GLOSSARY_TERM_RESOLUTION**
Every governed domain term in a requirement must resolve to the canonical glossary.

**CDD_P01_GLOSSARY_UNDEFINED_TERM_BLOCK**
Requirements containing undefined governed domain terms must not proceed without definition, replacement, or explicit exception.

**CDD_P01_GLOSSARY_SYNONYM_COLLAPSE**
Synonyms in raw intent must be collapsed to canonical glossary terms during normalization.

**CDD_P01_GLOSSARY_TERM_MEANING_STABILITY**
A term used across multiple requirements must carry the same meaning unless a scoped distinction is explicitly defined.

**CDD_P01_GLOSSARY_DOMAIN_IMPLEMENTATION_SEPARATION**
Glossary grounding must separate domain meaning from implementation detail.

**CDD_P01_GLOSSARY_TERM_CHANGE_IMPACT**
Any new or changed glossary meaning discovered in Phase 01 must identify the impacted requirements.

**CDD_P01_GLOSSARY_GAP_VISIBILITY**
Missing glossary entries, ambiguous definitions, and competing term meanings must be recorded as visible gaps.

---

## [Step 04 - Assign Requirement IDs](./Steps/Step-04/README.md)

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

## [Step 05 - Declare Scope Boundaries](./Steps/Step-05/README.md)

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

## [Step 06 - Surface Assumptions](./Steps/Step-06/README.md)

**CDD_P01_ASSUMPTION_EXPLICITNESS**
Any meaning required to understand a requirement but absent from raw intent must be recorded as an assumption.

**CDD_P01_ASSUMPTION_SOURCE_CLASSIFICATION**
Each assumption must identify whether it came from domain knowledge, existing system context, analyst inference, or stakeholder confirmation.

**CDD_P01_ASSUMPTION_REQUIREMENT_LINKAGE**
Each assumption must link to the requirement IDs it affects.

**CDD_P01_ASSUMPTION_APPROVAL_REQUIRED**
An assumption that affects behavior must be reviewed before the requirement set is stabilized.

**CDD_P01_ASSUMPTION_NO_HIDDEN_AUTHORITY**
Unreviewed assumptions must not grant downstream execution authority.

**CDD_P01_ASSUMPTION_CONFLICT_VISIBILITY**
Assumptions that conflict with raw intent, glossary definitions, or other assumptions must be recorded as conflicts.

**CDD_P01_ASSUMPTION_RETIREMENT_TRACE**
When an assumption is replaced by confirmed intent, the decision must remain traceable.

---

## [Step 07 - Detect Conflicts](./Steps/Step-07/README.md)

**CDD_P01_CONFLICT_DETECTION_REQUIRED**
The requirement set must be checked for contradictions before publication.

**CDD_P01_CONFLICT_RAW_NORMALIZED_PARITY**
Conflicts must be detected across raw intent, normalized requirements, glossary meanings, scope declarations, and assumptions.

**CDD_P01_CONFLICT_REQUIREMENT_LINKAGE**
Each detected conflict must identify the affected requirement IDs or raw intent items.

**CDD_P01_CONFLICT_DECISION_RECORD**
Each resolved conflict must include the resolution decision and authority for that decision.

**CDD_P01_CONFLICT_NO_SILENT_OVERRIDE**
A requirement must not override another requirement without a visible resolution artifact.

**CDD_P01_CONFLICT_BLOCKS_STABILIZATION**
Unresolved behavioral conflicts block requirement stabilization.

**CDD_P01_CONFLICT_RESOLUTION_TRACE_RETENTION**
Rejected alternatives and superseded wording must remain traceable to the conflict record.

---

## [Step 08 - Validate Completeness](./Steps/Step-08/README.md)

**CDD_P01_COMPLETENESS_CHECK_REQUIRED**
The requirement set must be checked for missing or underdefined intent before governance review.

**CDD_P01_COMPLETENESS_BEHAVIORAL_COVERAGE**
Required behavior, forbidden behavior, boundary behavior, and failure expectations must be evaluated for completeness.

**CDD_P01_COMPLETENESS_ACTOR_COVERAGE**
All actors referenced by the requirement set must have their relevant responsibilities and interactions defined or flagged.

**CDD_P01_COMPLETENESS_CONDITION_COVERAGE**
Important triggering conditions, preconditions, and termination conditions must be defined or flagged.

**CDD_P01_COMPLETENESS_DATA_MEANING_COVERAGE**
Domain data, states, terms, and classifications needed to understand requirements must be defined or flagged.

**CDD_P01_COMPLETENESS_NEGATIVE_SPACE_VISIBILITY**
Forbidden or excluded states implied by the intent must be captured or flagged for stakeholder decision.

**CDD_P01_COMPLETENESS_GAP_RECORDING**
Each completeness gap must be recorded with affected requirements, impact, and required decision.

**CDD_P01_COMPLETENESS_GAP_BLOCKING_CLASSIFICATION**
Each gap must be classified as blocking, non-blocking, or governed exception.

---

## [Step 09 - Governance Review](./Steps/Step-09/README.md)

**CDD_P01_GOVERNANCE_REVIEW_REQUIRED**
The requirement set must pass a governance review before downstream lowering.

**CDD_P01_GOVERNANCE_EVIDENCE_REQUIRED**
Review must have evidence for explicitness, glossary grounding, IDs, scope, assumptions, conflicts, completeness, and stability.

**CDD_P01_GOVERNANCE_DECISION_AUTHORITY**
Review approval, rejection, and exception decisions must identify the responsible authority.

**CDD_P01_GOVERNANCE_EXCEPTION_VISIBILITY**
Any exception to Phase 01 invariants must be visible, justified, owned, and time-bounded or reconciliation-bound.

**CDD_P01_GOVERNANCE_NO_CEREMONIAL_APPROVAL**
Approval without evidence does not grant downstream authority.

**CDD_P01_GOVERNANCE_REVIEW_TRACEABILITY**
Review findings must link to affected requirement IDs, gaps, assumptions, conflicts, or glossary terms.

---

## [Step 10 - Stabilize Requirements](./Steps/Step-10/README.md)

**CDD_P01_STABILITY_GATE_REQUIRED**
Requirements must pass a stability gate before they can serve as input to invariant extraction.

**CDD_P01_STABILITY_NO_OPEN_BLOCKERS**
No unresolved blocking gaps, conflicts, undefined terms, or unapproved assumptions may remain at stabilization.

**CDD_P01_STABILITY_BASELINE_DECLARATION**
The stabilized requirement set must be identified as a semantic baseline.

**CDD_P01_STABILITY_CHANGE_CONTROL**
Changes after stabilization must occur through governed revision rather than silent editing.

**CDD_P01_STABILITY_TRACE_PRESERVATION**
Stabilization must preserve traceability to raw intent, glossary terms, assumptions, scope decisions, and conflict decisions.

**CDD_P01_STABILITY_DOWNSTREAM_READINESS**
Each stabilized requirement must be fit for invariant extraction without requiring runtime interpretation.

---

## [Step 11 - Publish Requirements](./Steps/Step-11/README.md)

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

## Cross-Phase Exit Invariants

**CDD_P01_EXIT_EXPLICIT_NORMALIZED_GROUNDED**
Every requirement exiting Phase 01 must be explicit, normalized, and glossary-grounded.

**CDD_P01_EXIT_ADDRESSABLE_TRACEABLE_STABLE**
Every requirement exiting Phase 01 must be addressable, traceable, and stable.

**CDD_P01_EXIT_SCOPE_ASSUMPTION_CONFLICT_CLOSED**
Scope, assumptions, and conflicts must be resolved or carried as visible governed exceptions.

**CDD_P01_EXIT_READY_FOR_INVARIANT_EXTRACTION**
The Phase 01 output must be suitable for direct invariant extraction without adding new intent.

**CDD_P01_EXIT_NO_DOWNSTREAM_AUTHORITY_WITHOUT_GATE**
No downstream artifact may claim authority from Phase 01 unless the Phase 01 gate is passed or explicitly excepted.

---

## Final Compression

Phase 01 requires that raw intent become an explicit, glossary-grounded, addressable, scoped, assumption-visible, conflict-resolved, complete, governed, stable, and published semantic baseline before invariant extraction begins.
