---
name: "legal-fact-verifier"
description: "Adversarial verification for legal analysis, demand letters, mediation briefs, timelines, and rebuttals. Use when the user wants a truth-bound review that strips speculation, checks source support, and flags overstatement before distribution or reliance."
---

# Legal Fact Verifier

Pressure-test legal writing before it gets reused.

## Core rules

- Verify each claim against actual source text.
- Downgrade unsupported certainty.
- Never allow invented quotations, fake authority, or implied facts to pass as established.
- If a point cannot be verified, say so plainly.

## Review targets

- Demand letters
- Rebuttal letters
- Mediation statements
- Internal case memos
- Timelines
- Witness outlines
- Damages summaries

## Verification workflow

1. List each factual assertion that matters.
2. Check whether the source actually proves it.
3. Distinguish:
   - direct support
   - partial support
   - inference
   - legal argument
   - unsupported claim
4. Check dates, names, contract sections, amounts, and who said what.
5. Flag conflicts between sources instead of reconciling them silently.
6. Identify what would be needed to cure each weak point.

## Output structure

Lead with findings first, ordered by severity:

- Critical: false or materially overstated claims
- High: unsupported certainty or missing source support on important points
- Moderate: ambiguity, weak wording, or incomplete attribution
- Low: cleanup improvements

Then provide a safer rewrite if useful.

## Required labels

- [Fact]
- [Inference]
- [Legal Argument]
- [Open Question]
- [Needs Evidence]

## Anti-patterns

- Do not reward polished prose that outruns the record.
- Do not approve a statement just because it “sounds right.”
- Do not hide gaps in a footnote.
