# Revenue Messaging Framework (RMF)

**An open methodology — and Claude Code skill — for auditing and rewriting B2B website messaging.**

[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](LICENSE)
[![Built by Colony Spark](https://img.shields.io/badge/built%20by-Colony%20Spark-ff5a1f.svg)](https://colonyspark.com)

The Revenue Messaging Framework (RMF) is a complete, repeatable way to evaluate a B2B company's
website messaging and rewrite it to convert. Point it at a homepage and it researches the company,
scores the messaging out of 100, tears it down section by section, and hands back rewritten copy —
headline, value props, CTAs, and a full three-layer narrative — so you know exactly what to change
on your own site.

It was built by [Colony Spark](https://colonyspark.com) and used on real go-to-market engagements.
We open-sourced the whole thing — the spec, the grading scale, and the six-expert copywriting panel
that gates every rewrite — because good positioning shouldn't be a black box.

## Contents

- [What it does](#what-it-does)
- [Example](#example)
- [How the framework works](#how-the-framework-works)
- [Use it](#use-it)
- [Why it's different](#why-its-different)
- [Who it's for](#who-its-for)
- [Contributing](#contributing)
- [Credit](#credit)

## What it does

Give it a company name and a URL (or pasted homepage copy) and it produces a single analysis:

- **A messaging score (0–100) and letter grade**, justified section by section.
- **A section-by-section teardown** — every visible block (hero, value props, social proof, CTAs,
  pricing, about) quoted, analyzed for what works and what doesn't, and rewritten in full.
- **A three-layer Revenue Messaging Framework** — Role, Function, and Market narratives that move the
  buyer from "old way" to "new way."
- **A market transformation story** and a 7 / 30 / 90 / 365-day implementation roadmap.
- **Competitive positioning analysis** — the real differentiators and the one positioning trap to escape.
- **A prioritized next-step plan** — the quick wins to ship this week, ahead of the 30 / 90-day roadmap.

Every rewritten line is scored against six expert frameworks — Dunford (positioning), Ogilvy (copy
craft), Cialdini (buyer psychology), Schwartz (awareness stages), Laja (differentiation), Moesta
(Jobs to Be Done) — and only copy that clears the bar ships.

## Example

Here's the kind of rewrite the RMF produces — pulled from the worked example in the
[output template](templates/audit-template.md) (a fictional construction-ERP vendor, scored 58/100,
grade C):

> **Current hero:** "The Complete ERP Solution for Modern Businesses"
>
> **Why it fails:** Generic enough to describe hundreds of ERP systems. It puts the company in
> direct competition with SAP, Oracle NetSuite, and Microsoft Dynamics — a fight it can't win —
> and buries a real differentiator (purpose-built for commercial construction) under language
> trying to appeal to everyone.
>
> **Recommended revision:**
> **"Generic ERPs Don't Understand Construction. We Do."**
> *Subhead: BuildFlow is the only ERP purpose-built for commercial construction. Integrated
> project costing, AIA billing, and job-level profitability in one system. Trusted by 200+
> construction companies for 15 years.*
>
> **The positioning trap it escapes:** "Complete ERP Solution for Modern Businesses" competes
> against every ERP on earth. "The Only ERP Purpose-Built for Commercial Construction" creates a
> category of one. That's the trade the RMF is built to find — on every site it runs on.

The [full worked example](templates/audit-template.md) (near the bottom of the template) shows the
complete teardown: every section, the full three-layer messaging framework, and the grading
breakdown behind the score.

## How the framework works

| Piece | File |
|---|---|
| The full analysis spec — 10-section structure, grading scale, the rules | [`methodology/revenue-messaging-framework.md`](methodology/revenue-messaging-framework.md) |
| The six-expert copywriting panel that gates every rewrite | [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md) |
| The fill-in output skeleton + worked example | [`templates/audit-template.md`](templates/audit-template.md) |
| The Claude Code skill that drives it | [`SKILL.md`](SKILL.md) |

## Use it

**Quickstart — run it on your own site.**
1. Grab your homepage copy (or just the URL).
2. Paste `methodology/revenue-messaging-framework.md` to any capable model as its instructions, or use
   the Claude Code skill setup below.
3. Ask: *"Run an RMF on [Company] — [url] — here's our homepage copy: …"*

You get back a scored, section-by-section teardown and the rewritten copy.

**As a Claude Code skill.** Drop `SKILL.md` (and the `methodology/` and `templates/` files it
references) into your project's `.claude/skills/rmf-audit/` directory, then ask Claude to
"run an RMF on [company]."

**With any capable model.** The methodology is plain markdown. Paste
`methodology/revenue-messaging-framework.md` as a system prompt, give the model the company's
homepage copy, and ask for the analysis. The copywriting panel and template do the rest.

## Why it's different

Most messaging advice is either a vague checklist ("be clear," "know your audience") or a single
copywriting lens applied in isolation. The RMF is neither:

- **It's a graded output, not a vibe check.** Every analysis produces a 0–100 score with a letter
  grade, and the score is justified section by section — not just "this feels weak."
- **Every rewrite has to earn its place.** No recommendation ships until it clears six independent
  expert frameworks — positioning, copy craft, buyer psychology, awareness stage, differentiation,
  and Jobs to Be Done — at a 7.5+ composite with no single framework below 6. That gate lives in
  [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md) in full, scoring rubrics
  included.
- **It never invents data.** No fabricated stats, client names, or outcomes — if a claim isn't
  verifiable on the site, the framework flags it and tells you how to prove or replace it instead.
- **It's the whole spec, not a summary.** The grading scale, the section-by-section rules, the
  never-do / always-do lists, the panel rubrics — all of it is here, not held back.

## Who it's for

Any team selling a considered-purchase B2B product or service — founders, GTM leads, product
marketers, and consultants who need to know exactly where their messaging is leaking and what to say
instead. Colony Spark built it for founder-led vendors selling into the industrial economy, but the
framework is industry-agnostic. It's a weaker fit for pure e-commerce or B2C impulse purchases,
where there's no considered buying decision to evaluate.

## Contributing

Found a sharper rule, a better scoring boundary, or a failure mode the framework misses? Open an
issue or a PR against `methodology/` — see [`CONTRIBUTING.md`](CONTRIBUTING.md). Ran it on a site
and got a great (or a bad) result? Examples are welcome; they help calibrate the framework.

## Credit

Built and maintained by **[Colony Spark](https://colonyspark.com)** — a GTM systems architect for
founder-led vendors selling into the industrial economy. If this is useful, a star helps, and a link
back to https://colonyspark.com is appreciated. If you build on it or share an audit it generated,
please keep the attribution.

## License

[MIT](LICENSE) © Colony Spark. Use it, fork it, build on it.
