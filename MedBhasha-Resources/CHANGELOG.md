# Changelog — MedBhasha Resources

All notable changes to the entity schema, annotation guidelines, data
collection rules, worked example, and validator are logged here. If you
started annotating before a change was logged, check whether it affects
your already-tagged notes.

Format: `[version] — date — what changed — who it affects`

---
 
## [1.2] — November 12, 2026
**Round 2 README released.**
- `README.md` now includes the full Round 2 instructions: the three outputs
  (NER spans, clusters and analysis, RAG answers), scoring, and the submission
  contents.
- These repeat the instructions sent by email on Nov 10, 2026. No new requirements
  or format changes.
  
**Affects:** all teams. No action needed if you already followed the Nov 10 email.
 
---
 
## [1.1] — November 10, 2026
**Round 2 release.**
- Added `round2_release/` with the test notes
  (`medbhasha_bengali_clinical_notes(test_data).csv`, unlabeled) and the Bengali
  test queries (`test_queries_bn.csv`).
- The Round 2 instructions (NER spans, clusters and analysis, RAG answers, and the
  submission zip, which also includes `raw_data.csv`, your own sourced data) were
  sent to all teams by email on this date.

**Affects:** all teams, from the start of Round 2. The entity schema, annotation
guidelines and validator are unchanged.

---

## [1.0] — October 12, 2026
**Initial release.** Covers:
- `entity_schema.md` v1.0 — 10 entity categories, BIO/BIOES tagging scheme,
  file format specification, edge-case rulings
- `annotation_guidelines.pdf` v1.0 — annotation workflow, core principles,
  common mistakes, code-mixed text handling
- `data_collection_rules.md` v1.0 — approved sources, trust-then-verify
  process, consequences
- `worked_example/` — one fully annotated sample note, validated with zero
  errors
- `validate.py` — format validator (BIO/BIOES, column structure, tag
  vocabulary, sequence validity)
- `consent_form.pdf` — the mandatory bilingual consent form for any
  information collected directly from a patient.

**Affects:** all teams, from the start of Round 1.

---

<!--
Template for future entries:

## [1.x] — [DATE]
**Summary of the change in one line.**
- What changed, specifically
- Why (if a correction, link the issue that raised it)

**Affects:** [e.g., "Teams who annotated TEST_RESULT spans before this date
should re-check against the clarified definition in §3." or "New teams only
— no action needed if you already annotated under v1.0."]
-->
