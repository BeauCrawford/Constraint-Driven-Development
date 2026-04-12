# Step 03 - Partition Invariants

---

## Description

Step 03, Partition Invariants, performs its Phase 04 responsibility while preserving the governing invariants, traceability, and evidence needed for downstream authority.

---

## Invariants

**CDD_P04_RULE_UNIT_PARTITION_REQUIRED**
Validated invariants must be partitioned into enforceable rule units before constraint derivation.

**CDD_P04_RULE_UNIT_PARENT_BINDING**
Each rule unit must link to the invariant that authorizes it.

**CDD_P04_RULE_UNIT_ATOMICITY**
Each rule unit must represent a coherent enforceable behavior boundary.

**CDD_P04_RULE_UNIT_NO_SEMANTIC_LOSS**
Partitioning must not drop invariant meaning.

**CDD_P04_RULE_UNIT_NO_SEMANTIC_ADDITION**
Partitioning must not add behavior absent from the validated invariant set.

**CDD_P04_RULE_UNIT_POS_NEG_BOUNDARY_READINESS**
Rule units must be suitable for positive, negative, and boundary case definition.

**CDD_P04_RULE_UNIT_GAP_VISIBILITY**
Invariant meaning that cannot be partitioned cleanly must be recorded as a derivation gap.

---

## Substeps

### 🟥 Substep 01 - Prepare Inputs
*Bring the required source artifacts into view.*

* **🟥 AI Actions:** Load the artifacts needed for Partition Invariants, preserve upstream lineage, and surface missing context.
* **🟦 Human Actions:** Confirm input authority, resolve missing context, and approve readiness to proceed.

**Inputs:** Phase 04 source artifacts, prior phase evidence, glossary context, traceability records, and relevant gap or exception records.

**Outputs:** Input readiness notes for Partition Invariants.

**Invariants:** See step invariants above.

**Prompts**
- Partition Invariants Input Readiness Check - Identify whether the required inputs, lineage, and authority are present for this step.
- Partition Invariants Missing Context Finder - Surface missing artifacts, unresolved context, or upstream gaps before the step proceeds.

---

### 🟥 Substep 02 - Execute Partition Invariants
*Execute Partition Invariants with evidence and traceability.*

* **🟥 AI Actions:** Perform the analysis or transformation required by Partition Invariants while preserving semantic containment and traceability.
* **🟦 Human Actions:** Review the proposed output and resolve domain, scope, or governance decisions.

**Inputs:** Input readiness notes and the relevant governed artifact set.

**Outputs:** Step output for Partition Invariants with traceability to source authority.

**Invariants:** See step invariants above.

**Prompts**
- Partition Invariants Workbench - Produce the step output from the governed inputs while preserving the phase invariants.
- Partition Invariants Traceability Pass - Verify that the step output remains linked to upstream authority and does not introduce orphan meaning.

---

### 🟥 Substep 03 - Review and Record
*Make the step outcome inspectable and ready for the next gate.*

* **🟥 AI Actions:** Summarize evidence, gaps, exceptions, and downstream readiness for Partition Invariants.
* **🟦 Human Actions:** Review outputs, resolve domain decisions, and approve the outcome.

**Inputs:** Step output, evidence notes, gap records, and exception records.

**Outputs:** Reviewed step decision with evidence, gaps, exceptions, and next-step readiness.

**Invariants:** See step invariants above.

**Prompts**
- Partition Invariants Evidence Summary - Summarize the step output, decisions, gaps, and exception status for review.
- Partition Invariants Exit Review - Decide whether this step can proceed, requires rework, or must escalate a blocker.
