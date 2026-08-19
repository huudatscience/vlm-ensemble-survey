# Contributing

Thanks for helping keep this taxonomy current. VLM ensembling moves fast; the survey's corpus was finalized **July 2026**, so newer work is expected and welcome.

## Adding a new work

1. Check the three membership conditions from Section 4.1 of the survey before proposing an entry:
   - **Condition (i) — Multiplicity**: does the method draw on ≥2 distinct capability sources, verified by the elimination test (remove all but one source — does the mechanism become undefined, not just weaker)?
   - **Condition (ii) — VLM-ness**: does the system's final output stage (a) run on an LLM backbone and (b) produce free-form text?
   - **Condition (iii) — Timeframe**: published 2023–2026.
2. Classify it using the three decidable questions:
   - **Mode**: Fate question (Structural: Preserving vs. Consolidating) or Source question (Inference: Single-Origin vs. Multi-Origin).
   - **Category**: Locus question (Structural) or Shape question (Inference).
   - **Sub**: only applies to the four Sub-activated categories (Multi-Pathway Fusion, Mixture-of-Experts, Parameter-Space Merging, Critic & Role Pipelines) — see Table 3 of the survey.
3. Open a PR editing the relevant table in `README.md`, with:
   - Paper title, authors, venue/year, and a working arXiv or DOI link (no placeholder links).
   - A one-line justification for the Pillar → Mode → Category → (Sub) placement.

## Reporting a correction

If an existing entry is misclassified, has a broken link, or misattributes a claim, please open an issue describing:
- Which table/row is affected.
- What the correct citation or classification should be, with a source.

## Flagging a potential gap closure

The survey records the **Consolidating × Computation** cell (distilling a trained Mixture-of-Experts into a dense VLM) as the one open cell in the design space (Section 7.1). If you know of a VLM work that does this, please open an issue tagged `gap-closure` — this is exactly the kind of falsifying evidence the survey's methodology is designed to surface.

## Style

- Keep the citation format consistent with existing rows: `Author et al., Venue Year — [arXiv:ID](link)` (omit the arXiv part if no preprint exists).
- Don't reorganize table structure without discussion — it mirrors Table 2 of the published survey.
