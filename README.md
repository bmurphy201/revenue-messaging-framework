# Revenue Messaging Framework (RMF)

**An open methodology and Claude Code skill for auditing and rewriting B2B website copy: messaging, positioning, and value proposition.**

[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](LICENSE)
[![Built by Colony Spark](https://img.shields.io/badge/built%20by-Colony%20Spark-ff5a1f.svg)](https://colonyspark.com)

The Revenue Messaging Framework (RMF) is a repeatable way to evaluate a B2B company's website
messaging and rewrite it to convert. Point it at a homepage. It researches the company, scores the
messaging out of 100, tears it down section by section, and hands back rewritten copy: the headline,
the value props, the CTAs, and a full three-layer narrative. You end up knowing exactly what to change
on your own site.

Colony Spark built it and uses it on real go-to-market engagements. We published all of it, including
the spec, the grading scale and the six-expert copywriting panel that gates every rewrite, so you can
see exactly how a score gets made and argue with any part of it.

## Contents

- [What it does](#what-it-does)
- [Example](#example)
- [How the framework works](#how-the-framework-works)
- [Use it](#use-it)
- [Why it's different](#why-its-different)
- [Who it's for](#who-its-for)
- [What changed in October 2026](#what-changed-in-october-2026)
- [Contributing](#contributing)
- [Credit](#credit)

## What it does

Give it a company name and a URL (or pasted homepage copy). You get one analysis back:

- A messaging **score out of 100** and a letter grade, justified section by section.
- A section-by-section teardown. Every visible block (hero, value props, social proof, CTAs, pricing,
  about) gets quoted, analyzed for what works and what doesn't, and rewritten in full.
- The three-layer Revenue Messaging Framework: Role, Function, and Market narratives that move a buyer
  from the old way to the new way.
- A market transformation story, plus a 7 / 30 / 90 / 365-day implementation roadmap.
- Competitive positioning: your real differentiators, and the one positioning trap to escape.
- A prioritized place to start, so you know which quick wins to ship this week.

Every rewritten line goes through a plain-English check first, which turns dramatic, mannered phrasing
into plain statements. Then it gets scored against six expert frameworks: Dunford (positioning), Ogilvy
(copy craft), Cialdini (buyer psychology), Schwartz (awareness stages), Laja (differentiation), and
Moesta (Jobs to Be Done). A line ships once it clears the threshold and further rewrites stop raising
its score.

## Example

Here's the kind of rewrite the RMF produces, based on the worked example in the
[output template](templates/audit-template.md). The company is BuildFlow, a fictional
construction-ERP vendor that scored 58/100, grade C.

> **Current hero:** "The Complete ERP Solution for Modern Businesses"
>
> **Why it fails:** It could describe hundreds of ERP systems. It puts the company head to head with
> SAP, Oracle NetSuite, and Microsoft Dynamics, companies with far bigger brands and budgets, and it
> buries a real differentiator (purpose-built for commercial construction) under language meant to
> appeal to everyone.
>
> **Recommended revision:**
>
> **"See Every Job's Margin Before the AIA Pay App Goes Out"**
>
> *BuildFlow runs job costing, AIA billing, and job-level profitability in one ERP built for
> commercial construction. It has served more than 200 construction companies over 15 years, and one
> 140-person commercial GC cut pay-app prep from five days to one.*
>
> **The positioning trap it escapes:** "Complete ERP Solution for Modern Businesses" competes with
> every ERP on the market. Leading with commercial construction means buyers judge BuildFlow on
> construction fit, where its 15 years, 200+ construction clients and native AIA billing are real
> advantages.

The [worked example](templates/audit-template.md) at the bottom of the template is a condensed
analysis. It shows the bottom line, what the score means, the hero rewrite and the first layer of
the messaging framework.

## How the framework works

| Piece | File |
|---|---|
| The full analysis spec: 10-section structure, grading scale, the rules | [`methodology/revenue-messaging-framework.md`](methodology/revenue-messaging-framework.md) |
| The plain-English check and the six-expert copywriting panel that gate every rewrite | [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md) |
| The fill-in output skeleton and worked example | [`templates/audit-template.md`](templates/audit-template.md) |
| The Claude Code skill that drives it | [`SKILL.md`](SKILL.md) |

## Use it

**Quickstart: run it on your own site.**
1. Grab your homepage copy (or just the URL).
2. Give any capable model the two files in `methodology/` and the template in `templates/` as its
   instructions, or use the Claude Code skill setup below.
3. Ask: *"Run an RMF on [Company] ([url]). Here's our homepage copy: ..."*

You get back a scored, section-by-section teardown and the rewritten copy.

**As a Claude Code skill.** Drop `SKILL.md` (and the `methodology/` and `templates/` files it
references) into your project's `.claude/skills/rmf-audit/` directory, then ask Claude to
"run an RMF on [company]."

**Any capable model works too.** The methodology is plain markdown. Paste
`methodology/revenue-messaging-framework.md` as a system prompt along with
`methodology/copywriting-panel.md` and `templates/audit-template.md`, give the model the company's
homepage copy, and ask for the analysis.

## Why it's different

- **Every analysis ends in a grade you can check.** Each one produces a 0-100 score and a letter
  grade, and the section-by-section analysis has to justify the number.
- **Every rewrite has to earn its place.** Each recommended line passes the plain-English check, then
  has to clear six expert frameworks (positioning, copy craft, buyer psychology, awareness stage,
  differentiation, and Jobs to Be Done) at a 7.5+ composite with no single framework below 6. Lines
  that clear keep getting rewritten until the score stops rising. The full gate, scoring rubrics
  included, is in [`methodology/copywriting-panel.md`](methodology/copywriting-panel.md).
- **It never invents data.** If a claim isn't verifiable on the site, the framework flags it and tells
  you how to prove it or replace it. It won't make up statistics, client names or outcomes to fill a gap.
- **The whole spec is published.** The grading scale, the section-by-section rules, the never-do and
  always-do lists and the panel rubrics are all in this repo.

## Who it's for

It's for any team selling a considered-purchase B2B product or service, including founders, GTM leads,
product marketers, and the consultants who advise them. If you need to know where your messaging is
leaking and what to say instead, start here. Whatever you call the work (positioning, messaging, value
proposition, conversion copywriting, or fixing your website copy), the RMF finds what's weak and
rewrites it.

Colony Spark built it for industrial vendors, and it works in any industry where buyers make a
considered decision. Pure e-commerce and B2C impulse purchases are a weaker fit, because there's no
real evaluation to analyze.

## What changed in October 2026

- **A plain-English check before scoring.** Recommended copy gets rewritten to drop the dramatic
  shapes that make a line read as machine-written, such as manufactured reversals, payoff colons and
  wise-sounding closers, before the panel sees it.
- **The panel keeps pushing.** 7.5 is the minimum to ship. Lines that clear get rewritten from new
  angles and re-scored until the score stops rising.
- **Stricter readability.** Short beats, every labeled field on its own line, and real lists, so a
  busy site owner can scan the analysis.
- **A cleaner worked example.** The BuildFlow example now models copy that clears the plain-English
  check and the panel, with no unsupported claims.
- Section 3 is renamed "Section-by-Section Messaging Analysis."

## Contributing

Found a sharper rule, a better scoring boundary, or a failure mode the framework misses? Open an
issue or a PR against `methodology/` (see [`CONTRIBUTING.md`](CONTRIBUTING.md)). Ran it on a site
and got a great (or a bad) result? Examples are welcome. They help calibrate the framework.

## Credit

Built and maintained by **[Colony Spark](https://colonyspark.com)**, a GTM systems architect for
industrial vendors. If this is useful, a star helps, and a link back to https://colonyspark.com is
appreciated. If you build on it or share an audit it generated, please keep the attribution.

We publish two related packages the same way.
[Target List Build](https://github.com/bmurphy201/target-list-build) builds the named-account list
and finds the buying committee inside each account.
[AI Marketing Operator](https://github.com/bmurphy201/ai-marketing-operator) is a set of agent skills
for running a marketing week, and its `message-check` is a compact form of this framework.

## License

[MIT](LICENSE) © Colony Spark. Use it, fork it, build on it.
