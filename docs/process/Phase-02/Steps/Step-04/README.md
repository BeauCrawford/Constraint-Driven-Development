# Step 04 - Extract Invariants

---

## Description

Step 04, Extract Invariants, transforms semantic units into irreducible, implementation-independent truths. It keeps invariant candidates declarative, necessary, scoped to parent meaning, free of downstream semantics, and traceable to requirements.

---

## Invariants

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

## Substeps

### 🟥 Substep 01 - Convert Units to Candidate Truths
*Turn semantic units into invariant candidates.*

* **🟥 AI Actions:** Rewrite semantic units as declarative invariant candidates.
* **🟦 Human Actions:** Confirm candidates preserve domain intent.

**Inputs:** Semantic unit map and glossary-resolved terms.

**Outputs:** Invariant candidate set.

**Invariants:** CDD_P02_INVARIANT_EXTRACTION_REQUIRED, CDD_P02_INVARIANT_DECLARATIVE_FORM, CDD_P02_INVARIANT_CANDIDATE_TRACEABILITY

**Prompts**
- Invariant Candidate Extractor - Convert semantic units into declarative invariant candidates.
- Candidate Traceability Review - Check that each invariant candidate links to semantic units and requirement IDs.

---

### 🟥 Substep 02 - Check Irreducible Truth
*Ensure candidates state truths that must always hold.*

* **🟥 AI Actions:** Identify incidental, optional, explanatory, or nonessential candidate statements.
* **🟦 Human Actions:** Confirm what is essential domain truth.

**Inputs:** Invariant candidate set.

**Outputs:** Irreducible truth candidate set.

**Invariants:** CDD_P02_INVARIANT_IRREDUCIBLE_TRUTH, CDD_P02_INVARIANT_NECESSITY

**Prompts**
- Irreducible Truth Check - Evaluate whether each invariant candidate states necessary always-holding truth.
- Incidental Candidate Filter - Find candidate statements that are context, rationale, or example rather than invariant truth.

---

### 🟥 Substep 03 - Remove Lower-Layer Semantics
*Keep invariants independent of implementation and proof details.*

* **🟥 AI Actions:** Detect mechanisms, technologies, storage, protocol, test, constraint, contract, and implementation language.
* **🟦 Human Actions:** Decide whether lower-layer wording is unauthorized or true upstream intent.

**Inputs:** Irreducible truth candidate set.

**Outputs:** Implementation-independent invariant candidates.

**Invariants:** CDD_P02_INVARIANT_IMPLEMENTATION_INDEPENDENCE, CDD_P02_INVARIANT_NO_DOWNSTREAM_SEMANTICS

**Prompts**
- Implementation Independence Audit - Find implementation details embedded in invariant candidates.
- Downstream Semantics Detector - Identify constraint, test, contract, or code details that do not belong in invariants.

---

### 🟥 Substep 04 - Verify Parent Fidelity and Scope
*Ensure candidates remain inside parent intent.*

* **🟥 AI Actions:** Compare candidates to parent semantic units and scope boundaries.
* **🟦 Human Actions:** Resolve candidate drift or escalate upstream ambiguity.

**Inputs:** Implementation-independent invariant candidates, semantic units, and scope records.

**Outputs:** Parent-faithful invariant candidate set.

**Invariants:** CDD_P02_INVARIANT_PARENT_FIDELITY, CDD_P02_INVARIANT_SCOPE_ALIGNMENT

**Prompts**
- Invariant Parent Fidelity Check - Verify invariant candidates preserve parent semantic unit meaning.
- Invariant Scope Alignment Review - Detect invariant candidates that exceed or shrink parent scope.
