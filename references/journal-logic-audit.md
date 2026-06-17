# Journal Logic Audit

Use this reference before translating a substantive Chinese manuscript draft into target-journal-aligned SCI English.

## 1. Target Journal Map

Build a compact map before translation:

- Journal name, article type, and submission category.
- Required section structure and abstract type.
- Word limits for title, abstract, main text, and highlights if applicable.
- Required reporting guideline: CONSORT, PRISMA, STROBE, ARRIVE, CARE, CHEERS, TRIPOD, MDAR, or field-specific equivalent.
- Journal stance on novelty, mechanistic claims, clinical claims, translational claims, limitations, and data availability.
- Whether the journal prefers declarative titles, cautious titles, structured abstracts, graphical abstracts, highlights, or significance statements.

If current journal instructions are needed and not supplied, use official journal pages when browsing is available. Treat third-party summaries as secondary.

## 2. Manuscript Claim Chain

Extract this chain in plain language:

1. Field problem.
2. Specific knowledge gap.
3. Study objective or hypothesis.
4. Study design and materials.
5. Primary evidence.
6. Secondary evidence.
7. Interpretation.
8. Boundary conditions and limitations.
9. Final conclusion.

Do not translate into a stronger chain than the draft supports.

## 2A. Pre-Translation Diagnosis Table

For strict review mode, build this table before polished translation:

```text
| Source claim | Evidence in draft | Support level | English handling |
|---|---|---|---|
| [claim] | [data/method/result] | Supported / weak / unsupported / unclear | Translate / hedge / bracket / stop |
```

Use the table to decide whether the English should preserve, hedge, restructure, query, or stop. Do not hide the diagnosis when the user asked for strict realism.

## 3. Evidence Boundary Checks

Flag and hold back claims when the draft lacks support:

- "demonstrates" or "proves" without direct experimental evidence.
- "first", "novel", "unprecedented", or "breakthrough" without field-level support.
- "mechanism" when the work only shows association or phenotype.
- "diagnostic", "prognostic", "therapeutic", or "clinical utility" without appropriate validation.
- "significantly" without statistics.
- "improves survival", "enhances efficacy", or "reduces risk" without endpoint, comparator, and effect size.
- "universal", "broadly applicable", or "generalizable" from narrow samples.
- "safe" or "well tolerated" without safety assessment.
- Any citation-dependent claim when citations are absent or unsuitable.

Use cautious alternatives only when still accurate: "is associated with", "may contribute to", "was consistent with", "suggests", "supports", "provides evidence that".

## 3A. Common Chinese-to-SCI Risk Patterns

Watch for these recurring draft problems:

- Broad background sentences that are true but not connected to the study question.
- Results paragraphs that begin with interpretation instead of data.
- Discussion paragraphs that repeat results without explaining boundaries.
- Claims of mechanism based only on expression, correlation, enrichment, prediction, or phenotype.
- Claims of clinical value based only on retrospective association, database mining, or small exploratory cohorts.
- Claims of novelty based only on the author's impression rather than literature support.
- Overloaded sentences that combine method, result, implication, and speculation.

When these appear, restructure the English logic instead of translating word for word.

## 4. Section Logic

### Title

Make the title reflect the real result and study type. Avoid causal or mechanistic titles unless the design supports them.

### Abstract

Follow the target journal format. Preserve this order unless the journal requires otherwise: background gap, objective, design/methods, key results with concrete details, restrained conclusion.

### Introduction

Do not create a broad literature review. Build a funnel: established context, unresolved gap, why this study addresses it, precise objective. Avoid exaggerating disease burden or field importance beyond the draft.

### Methods

Translate for reproducibility. Preserve materials, cohorts, inclusion criteria, controls, measurements, statistical methods, software, ethics, and approvals. Do not smooth away missing details; flag them.

### Results

Lead with findings, not interpretation. Keep numbers, units, group names, timepoints, P values, confidence intervals, and figure references consistent with the draft. Do not add causal language.

### Discussion

Use this sequence: principal finding, relationship to existing knowledge, plausible interpretation, implications limited by evidence, limitations, future work, conclusion. Keep speculation visibly conditional.

## 5. Translation Decisions

Use sentence restructuring when Chinese order obscures SCI logic, but preserve factual content. Prefer:

- Active voice for study actions: "We assessed...", "This study evaluated...".
- Passive voice for standard methods when actor is irrelevant.
- Past tense for performed work and observed results.
- Present tense for established knowledge and conclusions that remain true.
- Cautious modal verbs for inference: "may", "could", "might", "is likely to".

Avoid empty intensifiers: "remarkably", "extremely", "very", "greatly", "dramatically" unless quantified and justified.

## 6. Stop-and-Ask Template

When the translation cannot proceed safely, respond with:

```text
Issue:
Why it matters for [journal/article type]:
What is needed:
Safe translation possible now:
```

If a partial translation is possible, translate only the safe parts and bracket unresolved items as author queries.

## 7. Deliverable Audit

Before finalizing, check:

- Does every strong English claim have direct support in the Chinese draft or supplied data?
- Did any sentence add a method, result, citation, limitation, or implication not present in the source?
- Does the abstract match the target journal format?
- Are results separated from interpretation?
- Are limitations honest and not performative?
- Are journal-specific elements included only when requested or required?

## 8. Mini Examples

### Unsupported mechanism

Source idea: Gene A regulates tumor invasion because Gene A expression correlates with invasion markers.

Decision: Do not translate as a proven mechanism. Use "Gene A expression was associated with invasion-related markers" unless functional perturbation or mechanistic experiments are supplied.

### Missing statistics

Source idea: The treatment group was significantly better, but no P value, confidence interval, or statistical method is supplied.

Decision: Translate as a descriptive difference or stop for statistics if the word "significantly" is central to the claim.

### Clinical overreach

Source idea: A biomarker predicts patient prognosis based on a single retrospective cohort.

Decision: Avoid "clinically useful" or "ready for clinical application". Use validation-limited wording and ask for independent validation details.
