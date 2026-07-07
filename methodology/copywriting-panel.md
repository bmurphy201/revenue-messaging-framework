# RMF Copywriting Panel — Recommended-Copy Scoring Gate

Used by the Revenue Messaging Framework analysis. Scores EVERY piece of recommended copy before it
ships in an analysis. **Threshold: 7.5 composite average, AND no single framework below 6.**

## Purpose

Every piece of recommended copy in an RMF analysis is scored against six expert frameworks **before
inclusion**. This is not pass/fail — each framework scores 1–10. Copy below threshold gets rewritten
until it clears. **The copy that ships is always copy that passed.** Scores are internal; the reader
of the analysis never sees them.

---

## The Panel

### 1. Dunford — Positioning
*Does this copy create a defensible market position or clear competitive separation?*

| Score | Meaning |
|---|---|
| 1–3 | Generic category language. Any competitor could use this. No positioning choice made. |
| 4–5 | Some positioning intent, but the frame is common or the category isn't clearly defined. |
| 6–7 | Clear positioning against alternatives. Buyer understands where this company sits vs competition. |
| 8–9 | Creates a "category of one" or reframes the buying criteria in the company's favor. Competitors would need to respond. |
| 10 | Category-defining. Changes how the buyer thinks about the market. Extremely rare on a first analysis. |

### 2. Ogilvy — Copywriting Craft
*Is the headline doing the heavy lifting? Is the copy specific, benefit-driven, filler-free?*

| Score | Meaning |
|---|---|
| 1–3 | Vague, jargon-heavy, feature-first. Headline could be swapped onto any competitor's site. Body is filler. |
| 4–5 | Communicates something real but buries the benefit or relies on clichés. Headline needs the body to make sense. |
| 6–7 | Benefit-driven and specific. Headline carries the core argument. Minor filler or tightening possible. |
| 8–9 | Every word earns its spot. Headline works standalone. Specific enough to fact-check. Reads like a human wrote it with conviction. |
| 10 | Quotable. The kind of line a CEO puts on a slide or repeats in a pitch. Extremely rare. |

### 3. Cialdini — Buyer Psychology
*Does this correctly deploy proof, authority, contrast, scarcity, reciprocity, or commitment/consistency?*

| Score | Meaning |
|---|---|
| 1–3 | No psychological lever present. Claims made without triggering trust or urgency. |
| 4–5 | One lever, weakly applied. Proof is vague ("trusted by many") or authority implied but not specific. |
| 6–7 | One or two levers applied well with specific evidence (named credentials, quantified proof, clear contrast). |
| 8–9 | Multiple levers working together naturally. Proof and authority stack without a hard-sell feel. Trust barrier addressed directly. |
| 10 | Textbook execution across multiple principles, effortless to the reader. |

### 4. Schwartz — Awareness Stages
*Does the copy meet the buyer at the correct awareness stage for where it appears on the site?*

| Score | Meaning |
|---|---|
| 1–3 | Wrong stage entirely. Product-aware copy where problem-aware is needed, or vice versa. |
| 4–5 | Right general stage, but the transition is clunky or the buyer fills in gaps. |
| 6–7 | Correct stage, smooth read. The buyer feels understood and is moved forward. |
| 8–9 | Precisely calibrated. Problem-aware hero, most-aware CTA, proof that bridges solution- to product-aware. |
| 10 | The copy itself creates new awareness — the buyer didn't know they had this problem until they read this. |

### 5. Laja — B2B Differentiation
*Could a competitor put their logo on this copy and have it still make sense?*

| Score | Meaning |
|---|---|
| 1–3 | Completely interchangeable. Template language. Any company in the category could claim this. |
| 4–5 | Some specificity, but the core claim is common in the industry. |
| 6–7 | Differentiated on ≥1 axis (proof, story, structure, credential) most competitors can't replicate. |
| 8–9 | Clearly ownable. Built on verifiable facts, specific credentials, or a structural advantage. A competitor would look foolish copying it. |
| 10 | The copy IS the moat. So specific to this company's DNA that imitating it would expose the imitator. |

### 6. Moesta — Jobs to Be Done
*Does this speak to the job the buyer is hiring for, or describe the product being sold?*

| Score | Meaning |
|---|---|
| 1–3 | Pure product/company description. Talks about what the company does, not what the buyer gets. |
| 4–5 | Hints at the buyer's job but frames it from the company's perspective ("We help you…" vs "You need…"). |
| 6–7 | Clearly speaks to a real buyer job. The buyer recognizes their situation; hiring criteria addressed. |
| 8–9 | Nails the switching trigger. Articulates WHY the buyer is shopping right now and positions the company as the answer. |
| 10 | Surfaces a job the buyer hadn't consciously articulated. "I didn't know that's what I was looking for, but that's exactly it." |

---

## Scoring Rules

- **Per-framework:** each of the 6 scores 1–10 for each piece of copy.
- **Composite:** average of all 6.
- **Threshold: 7.5 composite to ship.**
  - **9.0+** — exceptional; flag as a highlight in the analysis.
  - **7.5–8.9** — ships as written.
  - **6.0–7.4** — rewrite required; fix the frameworks dragging the score; re-score.
  - **Below 6.0** — start over; fundamental positioning/specificity/buyer-alignment problems.
- **Minimum per-framework: 6.** Even if the composite clears 7.5, any single framework below 6
  triggers a targeted rewrite for that dimension. (A great headline — Ogilvy 9 — with no
  differentiation — Laja 4 — still needs work.)

## What It Runs On (and What It Doesn't)

**Runs on:** hero/subhead/supporting-copy revisions · value-prop / pillar rewrites · section-specific
copy recommendations · CTA rewrites · every RMF "Your Message" statement.

**Does NOT run on:** structural/strategic recommendations ("move this section higher") · directional
guidance dependent on the company's data ("add [X] metric here") · the "What Works / What Doesn't
Work" analysis commentary.

## QA Presentation Format (internal only)

When recording the panel as a QA step (kept in an internal appendix, never in the delivered analysis):

```
**[Revision Name]**
Dunford: X/10 | Ogilvy: X/10 | Cialdini: X/10 | Schwartz: X/10 | Laja: X/10 | Moesta: X/10
**Composite: X.X/10**
[Status: SHIPS / REWRITE NEEDED / START OVER]
[If rewrite needed: which frameworks need attention and why]
```

---
**Related:** [`revenue-messaging-framework.md`](revenue-messaging-framework.md) (the spec) ·
[`../templates/audit-template.md`](../templates/audit-template.md) (the output skeleton).

*The Revenue Messaging Framework was built by [Colony Spark](https://colonyspark.com).*
