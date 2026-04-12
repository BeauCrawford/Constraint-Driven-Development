# Step 03 - Apply Glossary Grounding

---

## Description

Step 03, Apply Glossary Grounding, anchors requirement language to canonical terms so downstream lowering uses a shared semantic frame. It resolves undefined terms, collapses synonyms, detects terminology drift, and records glossary gaps before requirements proceed.

---

## Invariants

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

## Substeps

### 🟥 Substep 01 - Extract Governed Terms
*Find the vocabulary that carries requirement meaning.*

* **🟥 AI Actions:** Identify domain terms, actor names, state names, behavior names, classifications, and scoped terms in normalized requirements.
* **🟦 Human Actions:** Confirm which terms are governed domain vocabulary versus ordinary language.

**Inputs:** Normalized requirements and canonical glossary.

**Outputs:** Governed term inventory.

**Invariants:** CDD_P01_GLOSSARY_TERM_RESOLUTION, CDD_P01_GLOSSARY_DOMAIN_IMPLEMENTATION_SEPARATION

**Prompts**
- Governed Term Extractor - Identify domain terms in normalized requirements that need glossary resolution.
- Domain vs Implementation Term Review - Separate domain terms from implementation or technology terms.

---

### 🟥 Substep 02 - Resolve Terms
*Map requirement terms to canonical glossary entries.*

* **🟥 AI Actions:** Match governed terms to glossary definitions and flag unresolved terms.
* **🟦 Human Actions:** Approve term mappings and resolve uncertain definitions.

**Inputs:** Governed term inventory and canonical glossary.

**Outputs:** Glossary-resolved requirement terms.

**Invariants:** CDD_P01_GLOSSARY_TERM_RESOLUTION, CDD_P01_GLOSSARY_UNDEFINED_TERM_BLOCK

**Prompts**
- Glossary Resolution Mapper - Map each governed term to its canonical glossary entry.
- Undefined Term Register - List governed terms that lack glossary definitions and explain why they block progression.

---

### 🟥 Substep 03 - Collapse Synonyms
*Replace equivalent terms with stable semantic anchors.*

* **🟥 AI Actions:** Identify synonyms, aliases, and near-equivalent labels, then map them to canonical terms.
* **🟦 Human Actions:** Confirm synonym equivalence or preserve scoped distinctions.

**Inputs:** Glossary-resolved requirement terms and raw intent wording.

**Outputs:** Synonym mapping and canonicalized requirement vocabulary.

**Invariants:** CDD_P01_GLOSSARY_SYNONYM_COLLAPSE, CDD_P01_GLOSSARY_TERM_MEANING_STABILITY

**Prompts**
- Synonym Collapse Mapper - Find equivalent terms and map them to a single glossary anchor.
- Scoped Meaning Review - Identify terms that look synonymous but require separate scoped meanings.

---

### 🟥 Substep 04 - Detect Term Drift
*Ensure terms carry stable meaning across requirements.*

* **🟥 AI Actions:** Compare term usage across requirements and identify ambiguous or competing meanings.
* **🟦 Human Actions:** Decide whether meaning differences require glossary changes or requirement clarification.

**Inputs:** Canonicalized requirement vocabulary and requirement set.

**Outputs:** Term drift findings and impacted requirement list.

**Invariants:** CDD_P01_GLOSSARY_TERM_MEANING_STABILITY, CDD_P01_GLOSSARY_TERM_CHANGE_IMPACT

**Prompts**
- Term Drift Detector - Find terms whose meaning shifts across requirements.
- Glossary Impact Mapper - Identify requirements affected by a new or changed glossary meaning.

---

### 🟥 Substep 05 - Record Glossary Gaps
*Make terminology blockers visible.*

* **🟥 AI Actions:** Record missing entries, ambiguous definitions, competing meanings, and unresolved implementation-language issues.
* **🟦 Human Actions:** Decide which gaps require glossary update, requirement edit, or governed exception.

**Inputs:** Term drift findings and unresolved term list.

**Outputs:** Glossary gap register.

**Invariants:** CDD_P01_GLOSSARY_GAP_VISIBILITY, CDD_P01_GLOSSARY_UNDEFINED_TERM_BLOCK

**Prompts**
- Glossary Gap Register Builder - Convert unresolved terminology issues into explicit glossary gaps.
- Glossary Grounding Exit Review - Assess whether requirement terms are grounded enough to proceed.
