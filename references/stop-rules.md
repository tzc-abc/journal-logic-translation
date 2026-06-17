# Stop Rules

Use these levels to decide whether to stop, partially translate, or continue with a visible risk note.

## Level 1: Must Stop

Stop before translating the unsafe claim, but offer a safe path forward, when:

- Strict journal alignment is requested but the target journal or article type is unknown.
- The translation would require inventing data, statistics, methods, citations, ethics approval, consent, accession numbers, funding, conflicts, or data availability.
- The draft makes a causal, mechanistic, clinical, diagnostic, prognostic, safety, or superiority claim without matching evidence.
- Journal instructions conflict with the requested output structure.
- Required reporting details are missing for a structured clinical, animal, systematic review, diagnostic, or prognostic study.

Use this response:

```text
Issue:
Why it matters for [journal/article type]:
What is needed:
Safe translation possible now:
```

If a safer version is possible, provide it after the stop response under `Safe wording available now`. Do not make the unsafe claim sound acceptable.

## Level 2: Partial Translation Only

Translate safe parts and bracket risky parts when:

- Most text is descriptive but one claim is unsupported.
- Results are available but some statistics, timepoints, units, or group labels are missing.
- The journal profile is mostly clear but one required element is uncertain.
- The Chinese source contains ambiguous wording that affects interpretation.

Use bracketed author queries:

```text
[Author query: Please confirm sample size/timepoint/statistical test before using this sentence.]
```

## Level 3: Continue With Risk Note

Continue when the issue does not change the factual claim:

- The passage needs stylistic tightening only.
- The journal requirement affects format, not scientific content.
- The original claim is supportable but needs hedging.
- A stronger phrase can be replaced by a cautious one without changing meaning.

Record the risk under `Journal-logic notes` or `Evidence/risk note`.

## Claim Downgrade Examples

- Replace "demonstrates that X causes Y" with "supports an association between X and Y" when causality is not tested.
- Replace "a novel therapeutic strategy" with "a potential therapeutic strategy" when validation is preliminary.
- Replace "significantly improved" with "increased" or "was higher" when statistics are absent.
- Replace "clinically useful" with "may have clinical relevance" when clinical utility has not been validated.
