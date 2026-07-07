---
name: rmf-audit
description: Run a Revenue Messaging Framework (RMF) analysis on your own (or any) B2B website: score the messaging out of 100, tear it down section by section, and rewrite it. Invoke when asked to "run an RMF", "score a website's messaging", "do a messaging teardown/audit", or "Revenue Messaging Framework analysis". Produces a 10-section analysis with every recommended rewrite gated by a six-expert copywriting panel. Built by Colony Spark (https://colonyspark.com).
---

# RMF Audit

The repeatable driver for the Revenue Messaging Framework analysis. The methodology lives in
[`methodology/revenue-messaging-framework.md`](methodology/revenue-messaging-framework.md) (the spec),
the copy gate in [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md), and the
output skeleton in [`templates/audit-template.md`](templates/audit-template.md). This skill
orchestrates them.

## When to invoke

- "Run an RMF / Revenue Messaging Framework analysis on [company]"
- "Score [site]'s messaging" / "do a messaging teardown / website audit"
- Auditing your own site's messaging, or any B2B site you want to evaluate

## Inputs

**Required:** company name · website URL · homepage copy (pasted, or fetched in Step 2).
**Optional (improves quality):** extra page copy (About/Services/Pricing) · a previous analysis (→ use
the Updated-Analysis structure in the spec) · known competitors · target-audience info · industry news.

## Steps

### 1. Scope check (best fit)
The RMF works on any considered-purchase B2B site, and is sharpest when the buyer is making a real
evaluation (complex product/service, multiple stakeholders, meaningful deal size). If the site is
pure e-commerce or B2C impulse, say so and adjust expectations before proceeding.

### 2. Research (ground it: never guess, never fabricate)
- Fetch the homepage + the highest-signal pages (Services/Products, About/Team, Pricing, any
  "Compare/Why-us", case studies, recent blog/POV posts).
- Identify the real competitors / competitive category (named in Sections 2 & 7).
- Verify proof and credibility on the site (named clients, stats, founder credentials). If a claim
  isn't verifiable, flag it. Don't invent data, client names, or outcomes.

### 3. Run the analysis: 10 sections, exact order
Drive from [`templates/audit-template.md`](templates/audit-template.md), applying every rule in
[`methodology/revenue-messaging-framework.md`](methodology/revenue-messaging-framework.md):
Bottom Line → What This Score Means → Comprehensive Analysis (+ Missing Elements) → 3-layer RMF →
Transformation Story → Roadmap → Competitive Positioning → Bigger Picture → Next Steps → Grade/Score
tags. Honor the grading scale (**never above 85 on a first
analysis**), constructive tone, no `---` dividers, and the never-do/always-do lists.

### 4. Run the copywriting panel internally (during drafting, not after)
Score every recommended revision and every RMF "Your Message" against the six experts
([`copywriting-panel.md`](methodology/copywriting-panel.md)). Ship only
copy that clears **7.5 composite and ≥6 on every framework**. Rewrite the rest and re-score. Keep
scores in an internal QA appendix, never in the analysis itself.

### 5. Output
Output the full 10-section analysis: a self-contained messaging audit the site owner can act on.

## Outputs (checklist)

- [ ] Scope checked
- [ ] 10-section analysis produced
- [ ] All recommended copy cleared the panel, scores kept in an internal QA appendix

## Anti-patterns

- Running the analysis before researching the company.
- Shipping copy that didn't clear the panel, or leaving panel scores in the analysis.
- Fabricating stats, client names, or outcomes to fill a section.
- Scoring above 85 on a first analysis, or inflating to be nice.

## Related

- [`methodology/revenue-messaging-framework.md`](methodology/revenue-messaging-framework.md): the canonical spec (rules, structure, grading)
- [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md): the six-expert copy gate
- [`templates/audit-template.md`](templates/audit-template.md): the fill-in output skeleton + worked example

---
*The Revenue Messaging Framework was built by [Colony Spark](https://colonyspark.com).*
