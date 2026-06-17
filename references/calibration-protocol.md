# Calibration Protocol

Use this when the user wants to improve the skill with 2-3 real Chinese manuscript passages. The goal is to tune behavior, not to archive the user's manuscript.

## Inputs To Request

Ask the user for 2-3 anonymized passages if possible:

```text
Passage 1: ordinary Introduction/Methods paragraph
Passage 2: Results paragraph with data/statistics
Passage 3: Discussion/Abstract/Conclusion paragraph with higher-risk claims

For each passage:
- Target journal or broad style:
- Section type:
- Chinese text:
- Optional author English translation:
- Known data that must be preserved:
- What output felt too long, too short, too strict, or too loose in previous attempts:
```

If the user provides only one passage, still run calibration but label it as limited.

## Test Procedure

For each passage:

1. Run the skill using the current default mode.
2. Record whether the chosen mode was appropriate.
3. Check whether the English added any unsupported facts, methods, statistics, citations, or conclusions.
4. Check whether risk notes were useful or excessive.
5. Check whether the output length matched the likely user need.
6. Check whether the user would know the next action after reading the output.
7. If the user supplied their own English translation, check whether the skill preserved strong author wording instead of unnecessarily rewriting it.

## Scoring Rubric

Score each passage from 1-5:

```text
Accuracy:
Journal logic:
Evidence restraint:
Readability:
Output length:
Usefulness to a graduate student:
```

Interpretation:

- 5: ready to keep.
- 4: minor wording or length adjustment.
- 3: usable but needs instruction tuning.
- 2: risky or awkward; revise workflow or examples.
- 1: unacceptable; identify the failure mode before continuing.

## Output Length Tuning

Use these thresholds:

- If quick outputs feel too long, reduce author queries to the top 1-2 and downgrade notes to only high-impact phrases.
- If quick outputs feel too shallow, add the side-by-side table only for sentences with risk.
- If strict outputs feel too long, move detailed diagnosis into a compact table and summarize only the top risks.
- If strict outputs miss risks, require the pre-translation diagnosis table for that section type.

## Behavior Tuning

Adjust the skill instructions only when the same issue appears in at least two passages, or when one passage reveals a serious safety failure.

Common fixes:

- Output too verbose: tighten `references/output-patterns.md` length limits.
- Too many stops: move the case from `must stop` to `partial translation only` in `references/stop-rules.md`.
- Too permissive: add the risk phrase to `references/examples-overclaim.md`.
- Weak Results translation: add or revise an example in `references/examples-results.md`.
- Weak Discussion translation: add or revise an example in `references/examples-discussion.md`.
- Poor abstract logic: add or revise an example in `references/examples-abstract.md`.
- Over-rewriting good author English: strengthen `references/author-english-review.md` and the Author English Review output pattern.

## Calibration Report Format

After testing, provide:

```text
Calibration summary
- Passages tested:
- Overall score:
- Main failure pattern:

Recommended skill changes
1. [Specific file and instruction to adjust.]
2. [Specific file and instruction to adjust.]
3. [Specific file and instruction to adjust.]

Do not add manuscript text to the skill unless anonymized and approved.
```

If the user approves, implement the recommended changes and rerun the relevant passage.
