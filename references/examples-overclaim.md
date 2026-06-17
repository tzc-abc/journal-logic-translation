# Examples: Overclaim Downgrades

Use this file when the Chinese draft sounds stronger than the evidence supplied.

## Common Downgrades

| Risky Chinese claim | Safer English | What evidence would allow stronger wording |
|---|---|---|
| 证明A导致B | supports a possible association between A and B | causal design, perturbation, rescue, temporal evidence |
| 揭示A调控B的机制 | suggests that A may be involved in B-related signaling | direct mechanistic assays, pathway perturbation, rescue |
| 首次发现 | identifies / reports / provides evidence for | systematic literature support showing novelty |
| 具有重要临床应用价值 | may have clinical relevance | clinical validation, decision-impact analysis, prospective evidence |
| 显著提高 | increased / was higher | statistical test and significance threshold |
| 可作为诊断工具 | may warrant evaluation as a diagnostic biomarker | sensitivity, specificity, AUC, cutoff, independent validation |
| 安全有效 | showed preliminary efficacy / was well tolerated in this setting | adequate efficacy and safety endpoints |

## Quick Draft Example

Chinese source:

```text
我们的研究证明A通过激活B通路显著改善了疾病C，为临床治疗提供了新的策略。
```

Usable English draft:

```text
Our findings suggest that A may improve disease C-related outcomes, potentially through changes in B pathway activity. These results provide a basis for further evaluation of A as a therapeutic strategy.
```

Needs author confirmation:

- Was B pathway activation directly tested or inferred from markers?
- What outcome was improved, and at what timepoint?
- Is there statistical support for "significantly"?
- Is there in vivo, clinical, or only in vitro evidence?

Phrases downgraded:

- "证明" to "suggest" because causality/mechanism is not confirmed.
- "通过激活B通路" to "potentially through changes in B pathway activity" unless direct pathway activation is shown.
- "临床治疗提供新的策略" to "basis for further evaluation" unless clinical evidence exists.

## Stop Example

Stop if the user insists on:

```text
A is a safe and effective treatment for disease C.
```

without treatment efficacy and safety data.

Safe wording available now:

```text
A showed preliminary disease-modifying effects in the present model and warrants further evaluation.
```
