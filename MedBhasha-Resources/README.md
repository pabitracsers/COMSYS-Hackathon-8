# MedBhasha — Resources
### A Clinical NLP Hackathon

This repository contains everything you need to complete **Round 1: Onboarding &
Annotation**, plus reference material used throughout the hackathon. Start
here, then follow the links below in order.

---

## Start here

| Step | File | What it's for |
|---|---|---|
| 1 | [`data_collection_rules.md`](./data_collection_rules.md) | What data you're allowed to collect, and the trust-then-verify process we use to check it. **Read this before you source a single note.** |
| 2 | [`entity_schema.md`](./entity_schema.md) | The 10 entity categories, tagging scheme, file format, and edge-case rulings. |
| 3 | [`annotation_guidelines.pdf`](./annotation_guidelines.pdf) | How to apply the schema consistently — workflow, common mistakes, code-mixed text handling, self-review checklist. |
| 4 | [`worked_example/`](./worked_example) | A real note, correctly annotated end to end, validated with zero errors. Use it as your reference for exactly what a correct submission looks like. |
| 5 | [`validate.py`](./validate.py) | Run this on your corpus before every submission. Produces `validation_report.txt`, which is a mandatory part of your Round 1 and Round 2 zip. |

---

## Quick start

```bash
# 1. Read the rules and the schema first — not optional.

# 2. Annotate your corpus in any tool you like (Label Studio, doccano,
#    INCEpTION, a spreadsheet, or a custom script), exporting to the format
#    described in entity_schema.md §4.

# 3. Validate before you submit:
python validate.py --input your_annotated_data.csv --scheme BIO

# 4. Include validation_report.txt in your submission zip, alongside your
#    annotated corpus, source declaration, and EDA summary.
```

---

## Repository structure

```
MedBhasha-Resources/
├── README.md                     ← you are here
├── data_collection_rules.md      ← approved/banned sources, trust-then-verify process
├── consent_form.pdf 			  
├── entity_schema.md              ← entity categories, tagging scheme, file format
├── annotation_guidelines.pdf     ← how to annotate consistently, common mistakes
├── worked_example/
│   ├── sample_note_raw.txt
│   └── sample_note_annotated.csv ← correctly tagged, validated with zero errors
├── validate.py                   ← format validator — run before every submission
└── CHANGELOG.md                  ← version history for this repository
```

---

## Questions?

If anything is ambiguous — a data source you're not sure is allowed, a note
that doesn't clearly fit the entity schema, a validator error you can't
explain — **open an issue in this repository** rather than asking privately.
Your question and our answer become visible to every team, which keeps the
competition fair. Check existing issues first; it may already be answered.

We'll announce any updates to these materials through the official
competition communication channel and log them in
[`CHANGELOG.md`](./CHANGELOG.md).

---

## Timeline reminder

| Round | Dates | Relevant resources |
|---|---|---|
| Round 1 — Onboarding & Annotation | Oct 12 – Oct 22, 2026 | All files in this repository |
| Round 2 — Modeling: NER, Clustering & RAG | Oct 24 – Nov 5, 2026 | `entity_schema.md` (same schema used for scoring) |
| Round 3 — Finale | Nov 6 – Nov 8, 2026 | Submission format references this repository throughout |

See the full competition description on Unstop for complete rules, judging
criteria, and submission instructions.
