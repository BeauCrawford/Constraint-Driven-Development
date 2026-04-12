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

See [Constraint-Driven Development Process](/docs/process/README.md) for the phase-by-phase flow that moves CDD from requirement formation through invariant extraction, semantic closure, constraint derivation, proof, and code generation.

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

## **[The Process](./docs/process/README.md)**

### **Intent Closure**

*Tagline: Make meaning explicit before anything becomes executable.*

#### **1. [Requirement Formation](./docs/process/Phase-01.md)**
- Define glossary-grounded requirements  
- Assign unique IDs  
- Declare scope, assumptions, and conflicts  

#### **2. [Invariant Extraction](./docs/process/Phase-02.md)**
- Convert intent into irreducible truths  
- Remove redundancy and implementation bias  
- Capture forbidden states  

#### **3. [Semantic Closure Validation](./docs/process/Phase-03.md)**
- Ensure invariants fully cover requirements  
- Detect gaps, overlap, drift, or unauthorized additions  
- Record closure evidence  

### **Proof Construction**

*Tagline: Compile closed meaning into rules, contracts, and deterministic proof.*

#### **4. [Constraint Derivation](./docs/process/Phase-04.md)**
- Derive executable rules from invariants  
- Assign **unique CONSTRAINT_IDs**  
- Define positive, negative, boundary, and failure semantics  

#### **5. [Contract & Boundary Definition](./docs/process/Phase-05.md)**
- Define isolated interface and contract packages  
- Align interaction rules with constraints  
- Eliminate side-channel behavior  

#### **6. [Test Generation (Proof Construction)](./docs/process/Phase-06.md)**
- Generate deterministic tests from constraints  
- Map tests to CONSTRAINT_IDs  
- Cover positive, negative, boundary, and failure cases  

### **Admitted Implementation**

*Tagline: Prove the boundary first, then allow code to exist.*

#### **7. [Simulation & Boundary Validation](./docs/process/Phase-07.md)**
- Generate test doubles from contracts  
- Prove boundary behavior in isolation  
- Validate interactions and failure modes  

#### **8. [Code Generation / Implementation](./docs/process/Phase-08.md)**
- Generate or implement code to satisfy tests  
- Bind implementation to contracts  
- Avoid unproven behavior  

### **Continuity Governance**

*Tagline: Preserve lineage, closure, and authority as the system changes.*

#### **9. [Traceability Verification](./docs/process/Phase-09.md)**
- Validate Requirement → Invariant → Constraint → Test → Code lineage  
- Ensure stable IDs  
- Verify reverse navigation  

#### **10. [Coverage & Closure Revalidation](./docs/process/Phase-10.md)**
- Measure semantic coverage  
- Revalidate closure across all layers  
- Detect gaps and drift  

#### **11. [Change & Recompilation](./docs/process/Phase-11.md)**
- Apply changes at the requirement or invariant level  
- Recompute downstream artifacts  
- Regenerate constraints, tests, and code  

#### **12. [Governance & Enforcement](./docs/process/Phase-12.md)**
- Enforce entry and exit gates  
- Require proof for authority  
- Track and reconcile exceptions  

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
