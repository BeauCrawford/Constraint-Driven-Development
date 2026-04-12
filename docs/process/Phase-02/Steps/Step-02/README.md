# Step 02 - Resolve Terminology

---

## Description

Step 02, Resolve Terminology, ensures invariant extraction uses the same canonical glossary meanings as the parent requirements. It prevents undefined terms, synonym drift, new term invention, and semantic shifts from entering the invariant layer.

---

## Invariants

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

## Substeps

### 🟥 Substep 01 - Map Requirement Terms
*Carry parent vocabulary into invariant extraction.*

* **🟥 AI Actions:** Extract governed requirement terms and map them to glossary definitions.
* **🟦 Human Actions:** Confirm mappings and resolve domain terminology disputes.

**Inputs:** Requirement baseline and canonical glossary.

**Outputs:** Requirement term glossary map.

**Invariants:** CDD_P02_GLOSSARY_RESOLUTION_REQUIRED, CDD_P02_GLOSSARY_REQUIREMENT_TERM_COVERAGE

**Prompts**
- Phase 02 Term Mapper - Map requirement terms to canonical glossary entries for invariant extraction.
- Requirement Term Coverage Check - Find behavior-bearing requirement terms missing from the extraction record.

---

### 🟥 Substep 02 - Normalize Synonyms
*Collapse equivalent language to stable glossary anchors.*

* **🟥 AI Actions:** Identify synonyms and aliases in requirement wording and extraction notes.
* **🟦 Human Actions:** Approve synonym collapse or preserve scoped distinctions.

**Inputs:** Requirement term glossary map.

**Outputs:** Synonym-normalized extraction vocabulary.

**Invariants:** CDD_P02_GLOSSARY_SYNONYM_NORMALIZATION, CDD_P02_GLOSSARY_MEANING_PRESERVATION

**Prompts**
- Invariant Synonym Normalizer - Collapse equivalent terms to canonical glossary anchors.
- Scoped Term Review - Identify terms that look equivalent but require distinct meanings.

---

### 🟥 Substep 03 - Block Undefined or Invented Terms
*Prevent ungrounded vocabulary from entering invariants.*

* **🟥 AI Actions:** Detect undefined terms and new domain terms introduced during extraction.
* **🟦 Human Actions:** Decide whether to update glossary, revise wording, or record an exception.

**Inputs:** Synonym-normalized extraction vocabulary and candidate invariant wording.

**Outputs:** Undefined and invented term register.

**Invariants:** CDD_P02_GLOSSARY_UNDEFINED_TERM_BLOCK, CDD_P02_GLOSSARY_NO_TERM_INVENTION

**Prompts**
- Undefined Extraction Term Detector - Find terms used in extraction that lack glossary grounding.
- Term Invention Audit - Identify new domain language introduced by invariant extraction.

---

### 🟥 Substep 04 - Detect Terminology Drift
*Keep requirement and invariant meanings aligned.*

* **🟥 AI Actions:** Compare requirement term usage with invariant wording and flag meaning shifts.
* **🟦 Human Actions:** Resolve drift or escalate upstream glossary issues.

**Inputs:** Requirement term glossary map and candidate invariant wording.

**Outputs:** Terminology drift findings.

**Invariants:** CDD_P02_GLOSSARY_DRIFT_DETECTION, CDD_P02_GLOSSARY_MEANING_PRESERVATION

**Prompts**
- Requirement-to-Invariant Term Drift Detector - Find glossary meaning shifts between requirements and invariants.
- Terminology Drift Resolution Brief - Summarize drift cases and options for correction.
