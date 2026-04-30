# Scenarios Library

Real-world scenarios are what turn this curriculum from generic training into something that lands. This directory holds the scenario library and the guidance for adding to it.

---

## Why scenarios matter

The Microsoft Learn modules already cover the technical content. What you'll spend most of your facilitation time on is **mapping concepts to your audience's real work.** Without that, the live sessions feel generic — and generic AI training has a measurable adoption ceiling.

This is the biggest, most consistent finding from running this curriculum across multiple cohorts: **the bottleneck is scenarios, not content.**

---

## How to use this library

1. Browse the scenarios in this directory.
2. Find one that's close to your audience's domain. Adapt names, data, and outcomes.
3. If nothing fits — write a new one. Open a PR (see below).

---

## How to write a good scenario

A reusable scenario needs five things. If any are missing, the scenario is too generic to teach with.

### 1. The role
Who's doing the work. Be specific. *"A customer support manager at a 200-person SaaS company"* beats *"a manager."*

### 2. The current workflow (without AI)
3–5 steps. What they actually do today. Time spent. Pain points. This is what the audience compares against.

### 3. The AI-augmented workflow
Same workflow, with AI inserted at specific points. Not "AI does it all" — *where* does AI assist, *where* does the human still own the decision?

### 4. The Responsible AI checkpoint
The 3 questions, applied to *this* scenario:
- What data did the AI see?
- Where does a human review the output?
- What's the worst case if the AI gets it wrong?

### 5. The metric
How do you know it worked? *"Triage time per ticket dropped from 12 min to 4 min, with same or better resolution rate."* If you can't write the metric, the scenario is incomplete.

---

## Scenario template

Copy this into a new file at `scenarios/[track]-[short-name].md`:

```markdown
# Scenario — [Short descriptive name]

**Track / level:** Track X, L100/L200/L300
**Domain:** [industry, function, audience]
**Time to run:** [minutes for live demo]

## The role
[2–3 sentences]

## The current workflow (no AI)
1. ...
2. ...
3. ...
**Time:** ~X minutes/hours per [unit of work]
**Pain points:** [bullets]

## The AI-augmented workflow
1. ... [where AI assists]
2. ... [where AI assists]
3. ... [where the human still decides]
**Expected change:** [what's faster, better, more consistent]

## Responsible AI checkpoint
- **Privacy / fairness:** [answer]
- **Human review:** [answer]
- **Failure mode:** [answer + mitigation]

## Success metric
[Concrete, measurable, with a baseline]

## Facilitator notes
[What to demo, what to assign, common stumbling points]
```

---

## Scenario starter pack

A few scenarios that are close-to-ready and welcome contributions:

| Scenario | Track | Status |
|---|---|---|
| Customer support ticket triage | Track 1 L100 | 🟡 Draft welcome |
| Quarterly business review prep | Track 3 L200 | 🟡 Draft welcome |
| Onboarding FAQ agent | Track 2 L100 | 🟡 Draft welcome |
| Incident post-mortem assist | Track 6 Topic 2 L200 | 🟡 Draft welcome |
| Vendor evaluation workflow | Track 6 Topic 2 L100 | 🟡 Draft welcome |
| Sales-to-CSM handoff summary | Track 1 L200 | 🟡 Draft welcome |

If you've run any of these (or similar) successfully, please open a PR.

---

## What scenarios should not include

- **Customer-identifying details.** Anonymize names, products, dollar amounts, dates.
- **Internal-only data sources** that contributors outside your org can't access.
- **Vendor-loaded examples** that wouldn't work with comparable tools.
- **Speculative outcomes.** If you haven't run it, mark it as `proposed` rather than describing results that didn't happen.

---

## Contribution workflow

1. Open an issue: *"Proposing scenario: [name]"* with a 3-line summary.
2. Maintainer responds with sizing / direction within ~1 week.
3. Submit a PR using the template above.
4. Iterate on review.
5. Merge → live in the library.

See [../CONTRIBUTING.md](../CONTRIBUTING.md) for the general contributor workflow.
