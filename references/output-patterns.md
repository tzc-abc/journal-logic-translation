# Output Patterns

Use the pattern that best matches the user's requested deliverable.

## Quick Draft Mode

Use this as the default for early drafts, short paragraphs, and routine translation requests.

```text
Usable English draft
[Polished English paragraph]

Needs author confirmation
- [Only facts needed to make the wording fully safe, such as sample size, P value, cohort, comparator, or journal format.]

Phrases I downgraded
- Chinese: "[source phrase]"
  English used: "[safer phrase]"
  Reason: [evidence boundary]
```

Keep this mode light. Do not require a full pre-translation audit unless the paragraph contains high-risk causal, mechanistic, clinical, safety, novelty, or superiority claims.

Length limits:

- Keep `Usable English draft` to the translated passage only.
- Keep `Needs author confirmation` to no more than 3 bullets unless accuracy is unsafe.
- Keep `Phrases I downgraded` to no more than 3 bullets.
- Omit empty sections; write `None` only when the absence of risk is useful to the user.

## Author English Review Mode

Use this when the user provides their own English translation and asks whether it is good.

```text
Verdict
[One sentence: ready to use / usable with light edits / needs revision.]

Lightly polished version
[Edited English, preserving the user's structure and strong wording when possible.]

Why these edits
- [Up to 4 concise reasons.]

Consistency checks
- [Terminology, units, hyphenation, fold-change style, article use, or journal-specific concerns.]
```

Length limits:

- Do not rewrite from scratch when the user's version is already strong.
- Keep `Why these edits` to no more than 4 bullets.
- Do not include a full risk audit unless the draft contains unsupported claims.

## Short Passage

```text
Translation
[English text]

Journal-logic notes
- [Why the structure, tense, hedging, or terminology fits the target journal.]

Unsupported or risky claims
- [None / specific issue and required confirmation.]
```

## Full Section

```text
Pre-translation audit
- Target journal logic:
- Article/section logic:
- Main supported claim:
- Claims requiring caution:

Translated English
[English section]

Journal alignment changes
- [Sentence order, hedging, section flow, terminology, or structure changes.]

Claims held back or flagged
- [Claims not translated strongly, with reason.]

Questions for the author
- [Only questions needed to make the section accurate.]
```

## Side-By-Side Revision

```text
| Chinese source | English translation | Journal-logic rationale | Evidence/risk note |
|---|---|---|---|
| ... | ... | ... | ... |
```

Use this for teaching, careful revision, or when the user wants to see exactly why the English changed. Keep each Chinese source cell short enough to preserve readability. Split long Chinese sentences into logical units before translating.

Length limits:

- Use 3-6 rows for a typical paragraph.
- Keep rationale to one short clause per row.
- Move broader comments below the table only if they affect multiple rows.

## Abstract-First Mode

```text
Target-journal abstract logic
- Required format:
- Main evidence chain:
- Risk limits:

Abstract translation
[English abstract]

Line-by-line audit
- Background:
- Objective:
- Methods:
- Results:
- Conclusion:

Author queries
- [Missing information that affects compliance or accuracy.]
```

## Stop Response

```text
Issue:
Why it matters for [journal/article type]:
What is needed:
Safe translation possible now:
```

Keep stop responses concise and concrete. Do not bury the stop decision after a polished translation.

## Final Risk Snapshot

Use this after full sections, abstracts, and strict review outputs:

```text
Submission risk: Low / Medium / High

Main risks
- [Up to 3 highest-impact risks.]

Priority fixes
1. [Most important author action.]
2. [Second action, if needed.]
3. [Third action, if needed.]
```

Do not add this snapshot for simple quick-draft translations unless the user asks or the passage has high-risk claims.
