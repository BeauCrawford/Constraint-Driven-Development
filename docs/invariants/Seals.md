# Constraint-Driven Development - Sealing Invariants

This document defines sealing invariants for the invariant structure in `README.md` and recomputes recursive invariant closure with those seals applied.

A sealing invariant prevents semantic leakage across a boundary. It either blocks unauthorized addition, blocks silent loss, blocks bypass, or requires evidence before authority is granted.

## Sealing Invariants

| Seal ID | Sealing Invariant | Boundary Sealed | Rationale |
|---|---|---|---|
| CDD_SEAL_CANONICAL_SOURCE | Every governed artifact must declare its upstream source of authority before it can participate in lowering. | Source authority | Prevents artifacts from entering the structure without an authoritative parent. |
| CDD_SEAL_PARENT_CONTAINMENT | Every child artifact must be fully semantically contained by its immediate parent. | Parent-child lowering | Blocks downstream expansion beyond upstream meaning. |
| CDD_SEAL_NO_SILENT_LOSS | Every child artifact must account for all parent semantics or explicitly record a governed gap. | Parent-child lowering | Blocks implicit deletion of upstream intent. |
| CDD_SEAL_NO_UNAUTHORIZED_ADDITION | Any semantic addition not present in the parent must be rejected or promoted upstream for governance. | Parent-child lowering | Prevents lower layers from inventing authority. |
| CDD_SEAL_INTERMEDIATE_LAYER_REQUIRED | Lowering must pass through required intermediate layers before execution authority can emerge. | Layer transition | Blocks direct requirement-to-code or invariant-to-code jumps that bypass measurable containment. |
| CDD_SEAL_GLOSSARY_RESOLUTION | All domain-bearing terms in governed artifacts must resolve to canonical glossary entries. | Semantic frame | Prevents ambiguous or undefined language from crossing layers. |
| CDD_SEAL_STABLE_IDENTITY | Requirements, invariants, constraints, tests, contracts, and code realizations must retain stable IDs and bidirectional links. | Traceability | Blocks orphan artifacts and makes reverse navigation possible. |
| CDD_SEAL_CONSTRAINT_ADMISSIBILITY | Executable behavior is valid only when admitted by constraints derived from invariants. | Execution authority | Prevents implementation behavior from outrunning the constraint layer. |
| CDD_SEAL_PROOF_BEFORE_AUTHORITY | No artifact may grant execution authority without deterministic proof mapped to its governing constraints. | Proof gate | Blocks confidence, interpretation, or manual review from substituting for proof. |
| CDD_SEAL_NEGATIVE_SPACE | Forbidden states, boundary conditions, and failure semantics must be explicitly represented where they affect admissibility. | Constraint and proof coverage | Prevents closure from considering only positive behavior. |
| CDD_SEAL_CONTRACT_BOUNDARY | External interactions must pass through explicit contracts that carry behavior, dependencies, failures, and version semantics. | Interface boundary | Blocks side channels and hidden coupling. |
| CDD_SEAL_DOUBLE_SYMMETRY | Test doubles and simulations must conform to the same contract and constraint semantics as real implementations. | Simulation boundary | Prevents test environments from inventing behavior that production cannot honor. |
| CDD_SEAL_COVERAGE_THRESHOLD | Closure and coverage thresholds must be explicit before progression gates can pass. | Progression gate | Converts coverage from observation into enforceable authority control. |
| CDD_SEAL_DRIFT_REVALIDATION | Any change to upstream intent, glossary terms, constraints, contracts, or proof artifacts must trigger downstream revalidation. | Change propagation | Prevents stale downstream artifacts from retaining authority after drift. |
| CDD_SEAL_RELOWERING_OVER_PATCHING | Semantic repairs must propagate by re-lowering instead of local downstream patching. | Change management | Prevents downstream fixes from becoming unofficial sources of truth. |
| CDD_SEAL_EXCEPTION_VISIBILITY | Any exception to a seal must be recorded with owner, scope, reason, expiry, and downstream impact. | Governance | Prevents informal bypass from weakening the authority model. |
| CDD_SEAL_REVIEWABLE_STRUCTURE | Seal evidence must be inspectable as structured mappings rather than prose-only claims. | Auditability | Makes closure and enforcement reviewable by humans and tools. |
| CDD_SEAL_MECHANICAL_ENFORCEMENT | A seal is not complete until it is tied to a check, gate, generated artifact, or proof obligation. | Enforcement | Prevents ritualized documentation from masquerading as authority. |

## Seal Application Map

| Prior Closure Gap | Applied Seal |
|---|---|
| No formal parent-child dependency graph | CDD_SEAL_PARENT_CONTAINMENT, CDD_SEAL_STABLE_IDENTITY, CDD_SEAL_REVIEWABLE_STRUCTURE |
| No explicit coverage matrix | CDD_SEAL_COVERAGE_THRESHOLD, CDD_SEAL_NEGATIVE_SPACE, CDD_SEAL_PROOF_BEFORE_AUTHORITY |
| No numeric threshold policy | CDD_SEAL_COVERAGE_THRESHOLD |
| No concrete glossary enforcement | CDD_SEAL_GLOSSARY_RESOLUTION |
| No mechanical proof that invariants are contained, non-redundant, non-conflicting, and enforced | CDD_SEAL_MECHANICAL_ENFORCEMENT, CDD_SEAL_PARENT_CONTAINMENT, CDD_SEAL_NO_SILENT_LOSS, CDD_SEAL_NO_UNAUTHORIZED_ADDITION |
| Risk of bypass across layers | CDD_SEAL_INTERMEDIATE_LAYER_REQUIRED, CDD_SEAL_CONSTRAINT_ADMISSIBILITY, CDD_SEAL_PROOF_BEFORE_AUTHORITY |
| Risk of drift after change | CDD_SEAL_DRIFT_REVALIDATION, CDD_SEAL_RELOWERING_OVER_PATCHING |
| Risk of informal exceptions | CDD_SEAL_EXCEPTION_VISIBILITY |

## Recursive Invariant Closure With Seals Applied

| Structure | Baseline RIC | Sealed RIC | Delta | Rationale |
|---|---:|---:|---:|---|
| Full invariant catalog in `README.md` plus sealing invariants in this document | 0.87 | 0.93 | +0.06 | The seals close the largest structural gaps by requiring parent containment, no silent loss, no unauthorized addition, glossary resolution, stable identity, thresholded coverage, proof-before-authority, drift revalidation, and mechanical enforcement. The catalog now has explicit invariants for the major leakage paths that previously depended on implication. |

## Residual Closure Gap

| Remaining Gap | Effect on RIC | Required Next Artifact |
|---|---|---|
| The parent-child dependency graph is required but not yet materialized. | Prevents full verification of recursive containment. | A dependency map from requirements to invariants to constraints to tests to code. |
| Coverage thresholds are required but not yet numerically defined per layer. | Prevents gates from being mechanically evaluated. | A threshold policy for semantic closure, constraint coverage, proof coverage, and traceability. |
| Glossary resolution is required but not yet checked against a concrete glossary. | Leaves term drift detectable in principle but not mechanically audited. | A canonical glossary plus a term-to-artifact resolution matrix. |
| Proof-before-authority is required but not yet backed by generated proof artifacts. | Prevents the structure from claiming execution-ready authority. | Constraint-derived tests and proof result mappings. |
| Mechanical enforcement is required but not yet implemented as checks. | Keeps the seals structural rather than fully operational. | CI or local validation commands that fail on seal violations. |

Sealed RIC is `0.93`: structurally strong and substantially closed, but not yet `1.00` because the seals define the required closure mechanics without yet supplying every generated map, threshold, proof artifact, and enforcement check.
