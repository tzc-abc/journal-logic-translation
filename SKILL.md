---
name: journal-logic-translation
description: Translate Chinese academic manuscript drafts into SCI-style English that follows the target journal's article logic, section conventions, evidence boundaries, and author-guideline requirements. Use when the user asks to translate, rewrite, polish, or restructure a Chinese paper draft for a named journal, SCI submission, Nature/Cell/Science-family style, target-journal logic, journal-specific framing, abstract/results/discussion translation, or when the user explicitly says to stop if the translation departs from the actual data, methods, conclusions, or manuscript evidence.
---

# Journal Logic Translation

## Core Rule

Translate only what the manuscript, data, methods, and stated results can support. If target-journal logic would require information the draft does not contain, stop and name the missing item instead of inventing a stronger claim.

## Operating Modes

Choose one mode before working:

- `Quick draft mode`: use for early Chinese drafts, paragraph-level translation, or when the user wants a usable English version quickly with visible risk notes. Require only target journal or broad style, section type, and Chinese text when the passage is not high-risk.
- `Strict review mode`: use for journal-critical abstracts, discussion, claims, novelty framing, or any text likely to affect review outcome. Audit before translating and flag every unsupported move.
- `Fast submission mode`: use when the user has supplied complete methods, results, figures, statistics, and target-journal instructions. Translate efficiently, but still hold back unsupported claims.
- `Abstract-first mode`: use when the user asks to prepare a target-journal abstract before the full manuscript is ready.
- `Parallel revision mode`: use when the user needs Chinese source, English translation, and revision rationale side by side.
- `Author English Review mode`: use when the user provides their own English translation and asks whether it is good, publishable, natural, or aligned with the target journal. Preserve good author wording and make only necessary journal-level edits.

Default to `Quick draft mode` for ordinary paragraph translation. Default to `Strict review mode` when the user asks to stop if the translation departs from reality, when claims are high-stakes, or when the passage is an abstract, conclusion, novelty statement, or clinical/mechanistic claim.

## Intake

Before substantive translation, collect or infer these inputs:

- Target journal and article type.
- The Chinese draft text or file.
- Any journal author instructions, template, decision letter, reviewer comments, or model article supplied by the user.
- Study type, main finding, primary endpoint or outcome, key methods, sample/material source, and evidence level.
- Figures, tables, statistics, cited evidence, and author-provided non-negotiable facts when available.

If the target journal is missing, ask for it before applying journal-specific logic. If only a broad style is requested, state that the output is style-aligned rather than journal-compliant.

For incomplete requests, use `references/input-template.md` to ask for only the missing items that matter for the current task.

## Workflow

1. Confirm the operating mode and missing inputs. Use `references/input-template.md` when the user has not supplied enough context.
2. For `Quick draft mode`, translate first with light risk marking, then list author confirmations. Do not run a full audit unless the passage contains high-risk claims.
3. For `Author English Review mode`, read `references/author-english-review.md`, judge whether the user's English is already usable, then provide surgical edits rather than a full rewrite.
4. Build a target-journal profile. Use `references/journal-profile-template.md` for named journals, strict journal alignment, or article-type-specific translation.
5. Read `references/journal-logic-audit.md` for any substantive manuscript, abstract, results, discussion, cover-letter-adjacent framing, or strict journal-specific translation task.
6. Diagnose the Chinese draft before translating when in strict, abstract-first, or parallel revision mode. Extract the actual claim chain: background gap, question, method, result, interpretation, limitation, and conclusion.
7. Apply `references/stop-rules.md` to classify risks as `must stop`, `partial translation only`, or `continue with risk note`.
8. Translate section by section, preserving the evidence hierarchy: methods and results first, interpretation second, significance last.
9. Align rhetoric to the target journal without changing the science. Adjust tense, paragraph logic, hedging, signposting, and sentence order only when supported by the draft.
10. Deliver using the closest pattern in `references/output-patterns.md`.

## Calibration

When the user provides 2-3 real Chinese manuscript passages to improve the skill, use `references/calibration-protocol.md`. Test at least one low-risk paragraph, one Results or Methods-heavy paragraph, and one high-risk Discussion, Abstract, novelty, clinical, or mechanistic paragraph when available.

After calibration, tune only reusable instructions: output length, default mode choice, risk-note wording, author-query thresholds, and example coverage. Do not store the user's manuscript text inside the skill unless the user explicitly asks for anonymized examples.

Treat user-provided English translations as calibration signals. If the user's version is strong, preserve their phrasing and update reusable review rules rather than replacing the text with a model-preferred rewrite.

## Example Library

Use examples only when they match the user's section or risk pattern:

- `references/examples-results.md`: data-first Results translation.
- `references/examples-discussion.md`: Discussion translation with controlled interpretation.
- `references/examples-abstract.md`: abstract logic and structured translation.
- `references/examples-overclaim.md`: common overclaim downgrades and stop decisions.

## Stop Conditions

Stop or limit the task when any of these occur:

- The journal, article type, or required section format is unknown and the user requested strict journal alignment.
- The Chinese text claims causality, mechanism, clinical significance, novelty, generalizability, or superiority that the supplied data do not support.
- Key results lack sample size, control group, statistical method, effect direction, units, timepoint, or endpoint definition.
- The draft needs CONSORT, PRISMA, STROBE, ARRIVE, CARE, or another reporting checklist, but required reporting details are absent.
- The requested translation would require fabricating citations, statistics, methods, limitations, ethical approvals, data availability, or accession numbers.
- The target journal instructions conflict with the user's requested structure.

Use `references/stop-rules.md` to decide whether to stop completely, translate only safe parts, or continue with explicit risk notes.

## Output Format

For short passages, use:

- `Translation`
- `Journal-logic notes`
- `Unsupported or risky claims`

For early drafts or routine paragraph work, use:

- `Usable English draft`
- `Needs author confirmation`
- `Phrases I downgraded`

For teaching, careful revision, or user-requested comparison, use the side-by-side table in `references/output-patterns.md`.

For user-provided English drafts, use:

- `Verdict`
- `Lightly polished version`
- `Why these edits`
- `Consistency checks`

For full sections or manuscripts, use:

- `Pre-translation audit`
- `Translated English`
- `Journal alignment changes`
- `Claims held back or flagged`
- `Questions for the author`

For side-by-side revision, use:

- `Chinese source`
- `English translation`
- `Why this wording fits the journal logic`
- `Evidence/risk note`

See `references/output-patterns.md` for reusable formats.

## Style Priorities

Prefer clear SCI English over ornate language. Use precise verbs, concrete subjects, restrained novelty claims, and explicit links between evidence and interpretation. Keep journal-specific polish secondary to factual fidelity.
