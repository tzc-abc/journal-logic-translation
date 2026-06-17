# Examples: Results Translation

Use these examples when translating Chinese Results sections. Results should lead with data, preserve exact comparisons, and avoid interpretation unless the source sentence is explicitly interpretive and supported.

## Example 1: Data Before Interpretation

Chinese source:

```text
为了验证A对细胞增殖的影响，我们进行了CCK-8实验，结果显示A处理后细胞活力明显下降。
```

Better SCI English:

```text
To assess the effect of A on cell proliferation, we performed a CCK-8 assay. A treatment reduced cell viability compared with the control group.
```

Journal-logic rationale:

- Split method and result into two sentences.
- Use "reduced" rather than "inhibited" unless the assay directly supports inhibition.
- Add exact P value, timepoint, concentration, and replicate number if supplied.

Needs author confirmation:

- Treatment concentration.
- Timepoint.
- Statistical significance and test.
- Biological or technical replicates.

## Example 2: Missing Statistics

Chinese source:

```text
实验组的迁移能力显著低于对照组。
```

Safe quick draft:

```text
Cell migration was lower in the experimental group than in the control group.
```

If statistics are supplied:

```text
Cell migration was significantly lower in the experimental group than in the control group.
```

Reason:

- Do not use "significantly" without a statistical test, P value, confidence interval, or stated significance threshold.

## Example 3: Avoid Interpretation In Results

Chinese source:

```text
这些结果证明A通过调控B通路抑制肿瘤进展。
```

Risk:

- This is a mechanistic conclusion, not a pure Results sentence.

Safer Results wording:

```text
These results showed that A treatment was accompanied by reduced tumor progression and changes in B pathway-related markers.
```

Stop if:

- The draft lacks pathway perturbation, rescue experiments, or direct mechanistic testing.
