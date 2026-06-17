# Journal Logic Translation

A Codex skill for translating Chinese academic manuscript drafts into SCI-style English while preserving target-journal logic, evidence boundaries, and author intent.

This skill is designed for researchers who need more than sentence-level translation. It helps convert Chinese manuscript drafts into journal-aligned English, while actively preventing unsupported claims, inflated novelty, invented statistics, or overextended mechanistic and clinical conclusions.

## What It Does

- Translates Chinese academic drafts into clear SCI-style English.
- Aligns wording with the target journal, article type, and section logic.
- Flags claims that exceed the supplied data or methods.
- Supports quick draft translation, strict pre-submission review, abstract preparation, and author-written English review.
- Preserves strong author wording instead of rewriting unnecessarily.
- Provides calibration guidance using anonymized real manuscript passages.

## Core Principle

Translate only what the manuscript, data, methods, and stated results can support.

If target-journal logic would require information the draft does not contain, the skill should stop, ask for clarification, or provide a safer wording instead of inventing a stronger claim.

## Operating Modes

- `Quick draft mode`: for early drafts and routine paragraph translation.
- `Strict review mode`: for abstracts, conclusions, novelty claims, clinical claims, mechanistic claims, and pre-submission checks.
- `Fast submission mode`: for relatively complete manuscripts with methods, results, statistics, and target-journal instructions.
- `Abstract-first mode`: for building a target-journal-aligned abstract before the whole manuscript is ready.
- `Parallel revision mode`: for side-by-side Chinese source, English translation, and revision rationale.
- `Author English Review mode`: for checking and lightly polishing an English version already written by the author.

## Example Use

```text
Use $journal-logic-translation.

Target journal: Results in Engineering
Article type: Full research paper
Section: Results and Discussion
Chinese paragraph:
[paste paragraph]

Known data to preserve:
[sample size, model, metrics, P values, units, figure numbers, or "not available"]
```

For a lighter quick test:

```text
Use $journal-logic-translation.

Target journal: Results in Engineering
Section: Discussion
Chinese paragraph:
[paste paragraph]
```

For reviewing your own English translation:

```text
Use $journal-logic-translation in Author English Review mode.

Target journal: Results in Engineering
Section: Results and Discussion
My English draft:
[paste English draft]
```

## Typical Output

For quick drafts, the skill usually returns:

```text
Usable English draft
[polished English]

Needs author confirmation
- [missing data or details that affect accuracy]

Phrases I downgraded
- [source phrase, safer English, reason]
```

For author-written English, it usually returns:

```text
Verdict
[ready to use / usable with light edits / needs revision]

Lightly polished version
[edited English]

Why these edits
- [concise explanation]

Consistency checks
- [terminology, units, fold-change style, article use, hyphenation]
```

## Repository Structure

```text
journal-logic-translation/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── author-english-review.md
│   ├── calibration-protocol.md
│   ├── examples-abstract.md
│   ├── examples-discussion.md
│   ├── examples-overclaim.md
│   ├── examples-results.md
│   ├── input-template.md
│   ├── journal-logic-audit.md
│   ├── journal-profile-template.md
│   ├── output-patterns.md
│   └── stop-rules.md
├── LICENSE
└── README.md
```

## Installation

Copy or clone this folder into your Codex skills directory:

```text
~/.codex/skills/journal-logic-translation
```

Then invoke it in Codex with:

```text
Use $journal-logic-translation to translate this Chinese manuscript paragraph for [target journal].
```

## Calibration

To make the skill fit your field and writing style, test it with 2-3 anonymized manuscript passages:

- one low-risk Introduction or Methods paragraph;
- one Results paragraph with numerical data;
- one high-risk Discussion, Abstract, Conclusion, novelty, clinical, or mechanistic paragraph.

Use `references/calibration-protocol.md` to score output accuracy, journal logic, evidence restraint, readability, output length, and graduate-student usefulness.

Do not add real manuscript text to the skill unless it has been anonymized and you explicitly want it included as an example.

## What This Skill Will Not Do

- It will not invent data, statistics, citations, methods, ethics statements, or validation results.
- It will not turn correlation into causation.
- It will not convert preliminary evidence into clinical utility.
- It will not over-polish technical writing into vague promotional language.
- It will not store user manuscript text as examples without explicit approval.

## License

MIT License. See `LICENSE`.
