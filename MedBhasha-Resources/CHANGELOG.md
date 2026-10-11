# Changelog — MedBhasha Resources

All notable changes to the entity schema, annotation guidelines, data
collection rules, worked example, and validator are logged here. If you
started annotating before a change was logged, check whether it affects
your already-tagged notes.

Format: `[version] — date — what changed — who it affects`

---

## [1.0] — [October 12, 2026]
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
