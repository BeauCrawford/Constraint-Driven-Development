# **Semantic Closure**

Semantic Closure is the CDD rule that every layer must fully preserve the meaning of the layer above it before the next layer can gain authority.

See [Constraint-Driven Development Invariants](../../invariants/README.md) for the canonical invariant catalog this page summarizes.

See [Constraint-Driven Development Glossary](README.md) for the vocabulary used by the closure model.

---

## **Purpose**

Semantic Closure prevents behavior from being inferred, invented, or silently lost as intent moves through the CDD stack.

Each transformation must prove semantic containment:

Requirements -> Invariants -> Constraints -> Tests -> Code

The child layer may refine the parent layer, but it may not expand it, contradict it, skip it, or weaken it.

---

## **Core Rule**

Every governed artifact must answer two questions before it can be treated as authoritative:

- Does it preserve all relevant meaning from its parent?
- Does it avoid adding meaning that the parent did not authorize?

If either answer is no, closure has failed and downstream artifacts must not be trusted.

---

## **Recursive Loop**

Closure is recursive because the same containment rule applies at every boundary:

- Requirements close into invariants.
- Invariants close into constraints.
- Constraints close into tests.
- Tests close into code.
- Changes reopen closure and require downstream revalidation.

This makes closure a structural property of the whole system, not a one-time review step.

---

## **What Closure Enforces**

- Parent meaning is not silently dropped.
- Lower layers do not introduce unauthorized semantics.
- Constraint authority comes only from closed upstream intent.
- Tests prove constrained behavior rather than sample likely behavior.
- Code remains a residual artifact of proof, not an independent source of truth.
- Drift is treated as closure loss and must be surfaced.

---

## **Related Invariant Groups**

- [Semantic Closure Invariants](../../invariants/README.md) define closure as measurable containment.
- [Monotonic Lowering Invariants](../../invariants/README.md) define the one-way flow from upstream intent to downstream artifacts.
- [Traceability Invariants](../../invariants/README.md) ensure each artifact can be mapped back to its source.
- [Change Management Invariants](../../invariants/README.md) require revalidation when upstream meaning changes.
- [Meta Invariants](../../invariants/README.md) define the larger constraint-driven reality model.

---

## **Failure Signals**

Closure is broken when:

- A constraint cannot be traced back to an invariant.
- A test proves behavior not required by a constraint.
- Code implements behavior that no test or constraint admits.
- A requirement term is used without a glossary anchor.
- A downstream artifact survives after its upstream source changes.
- A layer describes similar intent but cannot prove containment.

---

## **Operational Summary**

Semantic Closure is the discipline that keeps CDD from becoming a loose chain of documents and generated artifacts.

It requires every layer to preserve upstream meaning, reject unauthorized additions, expose drift, and revalidate after change. The result is a system where implementation authority emerges only after intent has been closed, constrained, proven, and traced.
