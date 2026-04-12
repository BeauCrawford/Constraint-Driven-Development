# Step 01 - Capture Intent Surface

---

## Description

Step 01, Capture Intent Surface, ensures that raw stakeholder intent is captured visibly, faithfully, and with source attribution before any normalization or interpretation occurs. It preserves the full semantic signal, including goals, constraints, risks, exclusions, and acceptance language, while retaining links to domain or system context and making any missing input or incomplete context explicit as visible gaps.

---

## Invariants

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

## Substeps

### 🟥 Substep 01 - Source Inventory
*Bring every available source of intent into view.*

* **🟥 AI Actions:** Identify and list stakeholder inputs, source documents, existing system references, notes, goals, constraints, and expectation-bearing artifacts.
* **🟦 Human Actions:** Confirm source completeness, add missing sources, and identify which sources are authoritative.

**Inputs:** Stakeholder input, source documents, existing system context, meeting notes, acceptance language, and domain references.

**Outputs:** Source inventory with authority status and capture readiness.

**Invariants:** CDD_P01_INTENT_SOURCE_VISIBILITY, CDD_P01_INTENT_CAPTURE_GAP_VISIBILITY

**Prompts**
- Source Inventory Builder - Identify every source artifact that may contain stakeholder intent and classify its authority.
- Missing Source Detector - Surface missing stakeholder inputs, documents, or context needed before capture can be considered complete.

---

### 🟥 Substep 02 - Source Attribution
*Keep every captured intent item tied to where it came from.*

* **🟥 AI Actions:** Attach each intent item to its source, stakeholder, document, system context, or decision record.
* **🟦 Human Actions:** Resolve unclear authorship, confirm authoritative sources, and correct incorrect attribution.

**Inputs:** Source inventory and raw intent items.

**Outputs:** Attributed raw intent register.

**Invariants:** CDD_P01_INTENT_SOURCE_ATTRIBUTION, CDD_P01_INTENT_SOURCE_VISIBILITY

**Prompts**
- Intent Attribution Mapper - Link each raw intent item to its originating stakeholder, document, or system context.
- Authority Conflict Spotter - Identify cases where multiple sources appear to claim authority over the same intent.

---

### 🟥 Substep 03 - Raw Intent Preservation
*Preserve the original semantic signal before interpretation begins.*

* **🟥 AI Actions:** Capture raw wording, preserve source phrasing, and separate raw intent from later analysis.
* **🟦 Human Actions:** Verify that capture has not normalized, filtered, or rewritten stakeholder meaning too early.

**Inputs:** Attributed source material and stakeholder statements.

**Outputs:** Raw intent capture set with original wording preserved.

**Invariants:** CDD_P01_INTENT_UNTRANSFORMED_CAPTURE, CDD_P01_INTENT_SIGNAL_RETENTION

**Prompts**
- Raw Intent Extractor - Pull intent-bearing language from source material without normalizing or interpreting it.
- Preservation Review - Check whether any captured item has been prematurely rewritten, summarized, or softened.

---

### 🟥 Substep 04 - No-Filter Intake
*Keep ambiguous, conflicting, redundant, or difficult intent visible.*

* **🟥 AI Actions:** Retain questionable intent items and label ambiguity, conflict, redundancy, or implementation difficulty without discarding them.
* **🟦 Human Actions:** Decide whether questionable items remain in capture, require clarification, or become explicit gaps.

**Inputs:** Raw intent capture set and source inventory.

**Outputs:** Filter-safe intent register with questionable items retained and labeled.

**Invariants:** CDD_P01_INTENT_NO_PREMATURE_FILTERING, CDD_P01_INTENT_CAPTURE_GAP_VISIBILITY

**Prompts**
- Premature Filtering Audit - Find intent that may have been discarded or minimized because it was messy, conflicting, or hard to implement.
- Ambiguity Retention Pass - Label ambiguous or conflicting intent while preserving it for later normalization.

---

### 🟥 Substep 05 - Semantic Signal Capture
*Capture the full behavioral signal carried by each source.*

* **🟥 AI Actions:** Identify behavioral expectations, goals, constraints, exclusions, risks, acceptance language, and nonfunctional expectations.
* **🟦 Human Actions:** Confirm that important intent categories are represented and clarify missing signal.

**Inputs:** Raw intent capture set and attributed source material.

**Outputs:** Intent signal map grouped by expectation, goal, constraint, exclusion, risk, and acceptance language.

**Invariants:** CDD_P01_INTENT_SIGNAL_RETENTION, CDD_P01_INTENT_NO_PREMATURE_FILTERING

**Prompts**
- Signal Category Mapper - Classify raw intent into goals, behaviors, constraints, exclusions, risks, and acceptance language.
- Nonfunctional Signal Finder - Identify reliability, performance, security, usability, operational, or governance expectations embedded in raw sources.

---

### 🟥 Substep 06 - Context Linkage
*Keep domain and system context attached to captured intent.*

* **🟥 AI Actions:** Link intent items to relevant domain concepts, existing system behavior, source references, and contextual assumptions.
* **🟦 Human Actions:** Validate context links and add missing domain or system context.

**Inputs:** Raw intent register, source inventory, glossary, and existing system context.

**Outputs:** Context-linked intent register.

**Invariants:** CDD_P01_INTENT_CONTEXT_LINKAGE, CDD_P01_INTENT_SOURCE_ATTRIBUTION

**Prompts**
- Context Linker - Attach raw intent items to relevant domain context, existing system behavior, or source references.
- Context Gap Finder - Identify captured intent that lacks enough surrounding context to support later normalization.

---

### 🟥 Substep 07 - Capture Gap Register
*Make missing input and incomplete context visible before the step exits.*

* **🟥 AI Actions:** Record missing sources, incomplete stakeholder input, unresolved context, and unclear authority as explicit gaps.
* **🟦 Human Actions:** Decide which gaps must be resolved now and which can proceed as governed open items.

**Inputs:** Source inventory, attributed intent register, context-linked intent register, and capture review notes.

**Outputs:** Capture gap register with affected sources, intent items, and required decisions.

**Invariants:** CDD_P01_INTENT_CAPTURE_GAP_VISIBILITY, CDD_P01_INTENT_CONTEXT_LINKAGE

**Prompts**
- Capture Gap Register Builder - Turn missing source, context, and attribution issues into explicit capture gaps.
- Step Exit Readiness Review - Assess whether Capture Intent Surface can exit or must pause for missing input.
