# Phase 02 - Invariant Extraction Invariants

## Overview

These invariants define the phase-specific truths that must hold for Phase 02 - Invariant Extraction.
They specialize the global CDD invariant, glossary, traceability, semantic closure, monotonic lowering, and governance invariants for the invariant extraction layer.

No constraint derivation may begin until this invariant set is satisfied or an explicit governance exception is recorded.

---

## Step 01 - Load Requirements

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

## Step 02 - Resolve Terminology

**CDD_P02_GLOSSARY_RESOLUTION_REQUIRED**
All terms used for invariant extraction must resolve through the canonical glossary.

**CDD_P02_GLOSSARY_MEANING_PRESERVATION**
Invariant wording must preserve the glossary meaning used by the parent requirements.

**CDD_P02_GLOSSARY_UNDEFINED_TERM_BLOCK**
Undefined governed terms must block invariant finalization unless resolved or explicitly excepted.

**CDD_P02_GLOSSARY_SYNONYM_NORMALIZATION**
Synonyms encountered during extraction must collapse to canonical glossary terms.

**CDD_P02_GLOSSARY_NO_TERM_INVENTION**
Invariant extraction must not introduce new domain terms without glossary grounding.

**CDD_P02_GLOSSARY_REQUIREMENT_TERM_COVERAGE**
Every governed term in the parent requirement set that affects behavior must be represented or explicitly excluded in the invariant extraction record.

**CDD_P02_GLOSSARY_DRIFT_DETECTION**
Any change in term meaning between requirement wording and invariant wording must be detected as semantic drift.

---

## Step 03 - Decompose Requirements

**CDD_P02_SEMANTIC_UNIT_DECOMPOSITION_REQUIRED**
Requirements must be decomposed into semantic units before invariant extraction.

**CDD_P02_SEMANTIC_UNIT_PARENT_BINDING**
Each semantic unit must link to its parent requirement ID.

**CDD_P02_SEMANTIC_UNIT_ATOMICITY**
Each semantic unit must represent the smallest meaningful intent segment suitable for invariant extraction.

**CDD_P02_SEMANTIC_UNIT_NO_LOSS**
Decomposition must not drop parent requirement meaning.

**CDD_P02_SEMANTIC_UNIT_NO_ADDITION**
Decomposition must not add meaning not present in the parent requirement or governed glossary.

**CDD_P02_SEMANTIC_UNIT_CONDITION_RETENTION**
Conditions, triggers, actors, outcomes, and scope boundaries from parent requirements must remain visible in semantic units.

**CDD_P02_SEMANTIC_UNIT_MODALITY_RETENTION**
Required, forbidden, optional, and conditional modalities must remain distinguishable after decomposition.

**CDD_P02_SEMANTIC_UNIT_GAP_VISIBILITY**
Semantic units that cannot be extracted cleanly must be recorded as gaps or upstream clarification needs.

---

## Step 04 - Extract Invariants

**CDD_P02_INVARIANT_EXTRACTION_REQUIRED**
Every semantic unit must be evaluated for invariant extraction.

**CDD_P02_INVARIANT_IRREDUCIBLE_TRUTH**
Each invariant must state a truth that must always hold for the governed system.

**CDD_P02_INVARIANT_IMPLEMENTATION_INDEPENDENCE**
Invariants must not encode implementation mechanisms, technologies, storage choices, protocols, or test procedures.

**CDD_P02_INVARIANT_PARENT_FIDELITY**
Invariant statements must preserve the meaning of their parent requirements and semantic units.

**CDD_P02_INVARIANT_NECESSITY**
Each invariant must represent necessary system truth rather than incidental description.

**CDD_P02_INVARIANT_DECLARATIVE_FORM**
Invariants must be stated as declarative truths, not executable procedures.

**CDD_P02_INVARIANT_SCOPE_ALIGNMENT**
Invariants must remain within the scope boundaries established by their parent requirements.

**CDD_P02_INVARIANT_NO_DOWNSTREAM_SEMANTICS**
Invariants must not include constraint IDs, test cases, implementation decisions, or contract design.

**CDD_P02_INVARIANT_CANDIDATE_TRACEABILITY**
Each invariant candidate must retain lineage to source requirement IDs and semantic units.

---

## Step 05 - Remove Redundancy

**CDD_P02_REDUNDANCY_ANALYSIS_REQUIRED**
The invariant candidate set must be checked for duplicate and overlapping truths.

**CDD_P02_DUPLICATE_INVARIANT_ELIMINATION**
Duplicate invariant candidates must be merged or removed without semantic loss.

**CDD_P02_OVERLAP_RESOLUTION**
Overlapping invariant candidates must be separated, merged, or clarified so each remaining invariant has a distinct semantic role.

**CDD_P02_REDUNDANCY_TRACE_RETENTION**
Merged or removed invariant candidates must retain traceability to the requirements they covered.

**CDD_P02_REDUNDANCY_NO_COVERAGE_LOSS**
Removing redundancy must not remove coverage of parent requirement intent.

**CDD_P02_REDUNDANCY_DECISION_VISIBILITY**
Redundancy decisions that affect wording, merging, or removal must be visible for review.

---

## Step 06 - Validate Minimality

**CDD_P02_MINIMALITY_VALIDATION_REQUIRED**
Each invariant must be evaluated for minimality before finalization.

**CDD_P02_INVARIANT_MINIMAL_FORM**
Each invariant must be no broader than required to preserve its parent meaning.

**CDD_P02_INVARIANT_SUFFICIENCY**
The invariant set must be sufficient to preserve all parent requirement intent needed for downstream constraint derivation.

**CDD_P02_INVARIANT_NON_INCIDENTALITY**
Incidental explanation, examples, rationale, and narrative context must not remain in invariant statements.

**CDD_P02_INVARIANT_SPLIT_WHEN_COMPOSITE**
Composite invariants must be split when they contain multiple independently governed truths.

**CDD_P02_INVARIANT_MERGE_WHEN_INSEPARABLE**
Candidate invariants must be merged when separating them would distort a single irreducible truth.

**CDD_P02_MINIMALITY_REVIEWABILITY**
Minimality decisions must be inspectable by reviewers.

---

## Step 07 - Define Negative Space

**CDD_P02_NEGATIVE_SPACE_REQUIRED**
Forbidden states implied by requirements must be represented as invariants or explicit negative-space records.

**CDD_P02_NEGATIVE_SPACE_PARENT_DERIVATION**
Negative-space definitions must derive from parent requirements, glossary meaning, scope exclusions, or approved assumptions.

**CDD_P02_NEGATIVE_SPACE_NO_INVENTION**
Phase 02 must not invent forbidden states beyond upstream intent.

**CDD_P02_NEGATIVE_SPACE_BOUNDARY_VISIBILITY**
Invalid, excluded, and out-of-scope states must be distinguishable.

**CDD_P02_NEGATIVE_SPACE_TRACEABILITY**
Each negative-space definition must link to the requirement IDs and semantic units that justify it.

**CDD_P02_NEGATIVE_SPACE_CONSTRAINT_READINESS**
Negative-space definitions must be precise enough to support later forbidden-state constraint derivation.

**CDD_P02_NEGATIVE_SPACE_GAP_VISIBILITY**
Missing or unclear forbidden states must be recorded as gaps rather than inferred silently.

---

## Step 08 - Resolve Conflicts

**CDD_P02_INVARIANT_CONFLICT_DETECTION_REQUIRED**
The invariant set must be checked for contradictions before review.

**CDD_P02_INVARIANT_CONFLICT_PARENT_TRACE**
Each detected invariant conflict must identify the affected invariants, semantic units, and parent requirement IDs.

**CDD_P02_INVARIANT_CONFLICT_NO_SILENT_OVERRIDE**
One invariant must not override another without a visible resolution artifact.

**CDD_P02_INVARIANT_CONFLICT_UPSTREAM_ESCALATION**
Conflicts caused by parent requirement ambiguity or contradiction must be escalated upstream rather than patched in Phase 02.

**CDD_P02_INVARIANT_CONFLICT_RESOLUTION_AUTHORITY**
Each conflict resolution must identify the authority or decision source that resolved it.

**CDD_P02_INVARIANT_CONFLICT_BLOCKS_FINALIZATION**
Unresolved invariant conflicts block invariant finalization.

**CDD_P02_INVARIANT_CONSISTENCY_WITH_NEGATIVE_SPACE**
Positive invariant truths and negative-space definitions must not contradict each other.

---

## Step 09 - Review Gate

**CDD_P02_REVIEW_GATE_REQUIRED**
The invariant set must pass a review gate before finalization.

**CDD_P02_REVIEW_COVERAGE_EVIDENCE**
Review must include evidence that invariants cover parent requirement intent.

**CDD_P02_REVIEW_IMPLEMENTATION_INDEPENDENCE_EVIDENCE**
Review must include evidence that invariants remain implementation-independent.

**CDD_P02_REVIEW_MINIMALITY_EVIDENCE**
Review must include evidence that invariants are necessary, minimal, and non-redundant.

**CDD_P02_REVIEW_NEGATIVE_SPACE_EVIDENCE**
Review must include evidence that forbidden states were captured or explicitly marked as gaps.

**CDD_P02_REVIEW_TRACEABILITY_EVIDENCE**
Review must include requirement-to-invariant lineage evidence.

**CDD_P02_REVIEW_EXCEPTION_VISIBILITY**
Any exception to Phase 02 invariants must be visible, justified, owned, and reconciliation-bound.

**CDD_P02_REVIEW_NO_CEREMONIAL_APPROVAL**
Review approval without evidence does not grant downstream authority.

---

## Step 10 - Finalize Invariants

**CDD_P02_FINALIZATION_GATE_REQUIRED**
Invariants must pass a finalization gate before publication.

**CDD_P02_FINALIZATION_NO_OPEN_BLOCKERS**
No unresolved blocking conflicts, glossary gaps, coverage gaps, or upstream baseline defects may remain at finalization.

**CDD_P02_FINALIZATION_SEMANTIC_BASELINE**
The finalized invariant set must be identified as the semantic truth baseline for constraint derivation.

**CDD_P02_FINALIZATION_CHANGE_CONTROL**
Changes after finalization must occur through governed revision and revalidation.

**CDD_P02_FINALIZATION_TRACE_PRESERVATION**
Finalization must preserve lineage from requirements through semantic units to invariants and negative-space records.

**CDD_P02_FINALIZATION_DOWNSTREAM_READINESS**
Each finalized invariant must be suitable for constraint derivation without adding new intent.

**CDD_P02_FINALIZATION_NO_UNAUTHORIZED_ADDITION**
Finalized invariants must not contain semantics absent from the Phase 01 baseline or governed glossary.

---

## Step 11 - Publish Invariants

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

## Cross-Phase Exit Invariants

**CDD_P02_EXIT_IRREDUCIBLE_IMPLEMENTATION_INDEPENDENT**
Every invariant exiting Phase 02 must be irreducible and implementation-independent.

**CDD_P02_EXIT_MINIMAL_NON_REDUNDANT_COMPLETE**
The invariant set exiting Phase 02 must be minimal, non-redundant, and complete relative to parent requirement intent.

**CDD_P02_EXIT_TRACEABLE_TO_REQUIREMENTS**
Every invariant exiting Phase 02 must be traceable to one or more Phase 01 requirement IDs.

**CDD_P02_EXIT_NEGATIVE_SPACE_DEFINED**
Forbidden states implied by parent intent must be defined or carried as visible governed gaps.

**CDD_P02_EXIT_CONFLICT_FREE**
No unresolved invariant conflicts may proceed downstream.

**CDD_P02_EXIT_READY_FOR_CLOSURE_VALIDATION**
The Phase 02 output must be suitable for semantic closure validation without adding new intent.

**CDD_P02_EXIT_NO_DOWNSTREAM_AUTHORITY_WITHOUT_GATE**
No downstream artifact may claim authority from Phase 02 unless the Phase 02 gate is passed or explicitly excepted.

---

## Final Compression

Phase 02 requires that stabilized requirements become glossary-grounded, traceable, irreducible, implementation-independent, minimal, non-redundant, conflict-free invariant truth with explicit negative space before downstream closure validation and constraint derivation begin.
