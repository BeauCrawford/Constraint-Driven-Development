# Constraint-Driven Development - Invariant Kernel

This kernel condenses the invariant catalog into minimal irreducible form.
Each invariant below must hold for CDD to remain CDD.

---

## Higher-Order Rollup

**CDD_ROLLUP_INTENT_CLOSURE**
Behavior is legitimate only when it remains inside closed upstream intent.

**CDD_ROLLUP_CONSTRAINT_ADMISSIBILITY**
Execution is allowed only when constraints admit it.

**CDD_ROLLUP_DETERMINISTIC_PROOF**
Correctness requires reproducible proof, not interpretation or confidence.

**CDD_ROLLUP_TRACEABLE_REALIZATION**
Implementation is valid only as a traceable realization of proven constraints.

**CDD_ROLLUP_GOVERNED_EVOLUTION**
Change is valid only when closure, proof, and lineage are re-established.

---

## Kernel Invariants

**CDD_KERNEL_INTENT_AUTHORITY**
Upstream intent is the highest source of behavioral authority.

**CDD_KERNEL_CANONICAL_MEANING**
All governed meaning must resolve through explicit, stable, shared vocabulary.

**CDD_KERNEL_SEMANTIC_CLOSURE**
Each downstream layer must fully preserve parent meaning without silent loss or unauthorized addition.

**CDD_KERNEL_MONOTONIC_LOWERING**
Development must proceed only by bounded refinement from requirements to invariants, constraints, tests, and code.

**CDD_KERNEL_INVARIANT_TRUTH**
Invariants must state implementation-independent truths that always hold.

**CDD_KERNEL_CONSTRAINT_AUTHORITY**
Executable behavior is admitted only through constraints derived from invariants.

**CDD_KERNEL_BOUNDARY_EXPLICITNESS**
All externally observable interaction semantics must be expressed through contracts.

**CDD_KERNEL_PROOF_BEFORE_IMPLEMENTATION**
Tests must deterministically prove constraint conformance before implementation gains authority.

**CDD_KERNEL_TRACEABLE_LINEAGE**
Every artifact must retain stable, bidirectional lineage across requirement, invariant, constraint, test, and code layers.

**CDD_KERNEL_DETERMINISTIC_EXECUTION**
Runtime behavior and proof execution must not depend on unresolved interpretation.

**CDD_KERNEL_NO_UNPROVEN_BEHAVIOR**
No implementation, double, contract, or generated artifact may introduce behavior outside the closed constraint system.

**CDD_KERNEL_RECOMPILATION_OVER_PATCHING**
Change must originate upstream and propagate by re-lowering, regeneration, proof, and revalidation.

**CDD_KERNEL_GOVERNED_AUTHORITY**
Progression between layers requires enforceable gates, evidence, and visible exception handling.

---

## Compression

CDD requires that behavior be explicitly intended, semantically closed, monotonically lowered, constraint-bound, deterministically proven, traceably realized, and governed under change.
