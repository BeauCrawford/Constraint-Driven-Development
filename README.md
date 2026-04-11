# **Constraint-Driven Development (CDD)**

**Code is not the source of truth.  
Constraints are.**

Constraint-Driven Development is a software engineering model where **requirements are monotonically lowered into invariants, compiled into constraints, and proven through deterministic tests**, such that implementation is forced—not inferred.

This repo defines a system where **behavior is not written—it is admitted**.

---

## **Core Idea**

Traditional development asks:

> “What code should we write?”

CDD asks:

> “What behavior is allowed to exist?”

Everything else is removed.

---

## **The Spine**

Requirements → Invariants → Constraints (ID) → Tests → Code

- **Requirements** — Declared intent (domain-grounded)
- **Invariants** — Irreducible truths (must always hold)
- **Constraints** — Executable bounds (what is allowed / forbidden)
- **Tests** — Deterministic proofs (no runtime interpretation)
- **Code** — Residual artifact of passing proof

See [Constraint-Driven Development Invariants](/docs/invariants/README.md) for the canonical invariant catalog that defines the non-negotiable semantic rules CDD uses to govern lowering, proof, traceability, and change.

See [Constraint-Driven Development Glossary](/docs/theory/glossary/README.md) for the canonical vocabulary that stabilizes CDD terms, maps disallowed synonyms, and keeps requirements, invariants, constraints, tests, and code semantically aligned.

---

## **What This Changes**

### **1. Code Loses Authority**

Code is no longer where truth lives.  
It is the **output of a closed constraint system**.

If it passes, it conforms.  
If it doesn’t, it is rejected.

---

### **2. Tests Become Proof**

Tests are not examples or confidence checks.

They are:
- Generated from constraints  
- Mapped to constraint IDs  
- Deterministic at runtime  
- Exhaustive across positive / negative / boundary space  

**Green means proven—not plausible.**

---

### **3. Constraints Define Reality**

Constraints are the first executable form of truth.

They:
- Encode required behavior  
- Forbid invalid states  
- Define boundary conditions  
- Carry unique IDs for traceability  

**If it’s not constrained, it’s not real.**

---

### **4. Invariants Are the Semantic Core**

Invariants are where intent becomes governable.

They:
- Remove implementation bias  
- Capture irreducible truths  
- Define the semantic closure surface  

Weak invariants → corrupted system.

---

### **5. Contracts Become Semantic Boundaries**

All interfaces live in isolated contract packages.

They:
- Carry behavioral expectations (not just types)  
- Enable generation of test doubles  
- Define system boundaries before implementation exists  

**We prove the boundary before we build the system.**

---

## **The Process**

### **1. Define Requirements**
- Structured, explicit, glossary-grounded  
- No narrative ambiguity  

### **2. Extract Invariants**
- Minimal, non-redundant, exhaustive  
- Independent of implementation  

### **3. Measure Semantic Closure**
- Ensure invariants fully cover requirements  
- Iterate until closure is high  

### **4. Derive Constraints**
- Assign **unique IDs**  
- Encode allowed / forbidden / edge behavior  

### **5. Generate Tests**
- Positive, negative, boundary, failure  
- Deterministic (no agents at runtime)  
- Mapped to constraint IDs  

### **6. Prove Green in Isolation**
- Use contract-driven test doubles  
- Validate boundary behavior first  

### **7. Generate Code**
- Make tests pass  
- No invention, only conformance  

---

## **Key Properties**

- **Monotonic Semantic Lowering**  
  Each layer is fully contained by its parent  

- **Semantic Closure First**  
  Meaning is complete before execution  

- **Constraint Authority**  
  Behavior is enforced, not suggested  

- **Deterministic Proof Surface**  
  No runtime interpretation  

- **Traceable Lineage**  
  Requirement → Invariant → Constraint → Test → Code  

- **Boundary-First Validation**  
  Contracts are proven before implementation  

---

## **What You Get**

- Clean, stable code generation (LLM or otherwise)  
- Elimination of requirement → code drift  
- Deterministic, non-flaky test suites  
- Full traceability of behavior  
- Reduced debugging to constraint tracing  
- Safe refactoring through preserved proof surfaces  

---

## **What This Replaces**

| Traditional | CDD |
|------------|-----|
| Code-first | Constraint-first |
| Tests as validation | Tests as proof |
| Behavior inferred | Behavior enforced |
| Coverage = lines | Coverage = semantics |
| Debugging | Constraint tracing |
| Refactoring risk | Proof-preserving change |

---

## **Failure Modes (What This Prevents)**

- Hidden assumptions in code  
- Untested edge cases  
- Semantic drift across layers  
- Flaky or interpretive tests  
- Boundary leakage and side channels  
- “Works but not correct” systems  

---

## **The Real Model**

CDD is not a workflow.

It is a **legitimacy system**.

Behavior is legitimate only if it:
- originates from requirements  
- is preserved through invariants  
- is enforced by constraints  
- is proven by tests  
- is realized by code  

---

## **High Compression**

**You are not writing software.  
You are collapsing the space of possible software until only one implementation can exist—and then letting the system generate it.**

---

## **Status**

This repo is an evolving specification and reference implementation of Constraint-Driven Development.

Expect:
- patterns  
- tooling ideas  
- examples  
- enforcement strategies  

---

## **License**

MIT — see [LICENSE](./LICENSE.md)
