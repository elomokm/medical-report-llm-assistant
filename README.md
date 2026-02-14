# Medical Report LLM Assistant

AI assistant that transforms raw medico-social notes into structured professional observations.

Goal: reduce administrative time while keeping human responsibility.

---

## Problem

Professionals in medico-social structures spend significant time writing daily observations.

Notes are often:
- fast
- heterogeneous
- incomplete

This creates cognitive load and reduces time spent with patients.

---

## Proposed Solution

The system reformulates raw notes into structured neutral reports.

Human validates.
AI never diagnoses.

Workflow:

Raw Notes → Structured Proposal → Human Validation → Record

---

## Example

### Input
Mme Dupont agitée ce matin, refus du petit déjeuner, discussion compliquée avec sa fille, meilleure humeur après promenade, traitement pris avec aide

### Output
Observation:
Patient shows agitation in the morning and refuses breakfast.

Relational event:
Tense interaction with daughter during visit.

Evolution:
Mood improves after accompanied walk.

Treatment:
Medication taken with assistance.

---

## AI Pipeline

User Notes
↓
Segmentation
↓
Semantic classification
↓
Constrained generation (LLM)
↓
Human validation


More details in docs/product_spec.md