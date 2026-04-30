---
applyTo: 'scenarios/**/*.md'
---

# Scenario File Conventions

These rules apply to any markdown file under `scenarios/` (excluding `scenarios/README.md`, which documents the conventions themselves).

## Required structure

Every scenario file must contain these sections, in this order:

1. **Title** — `# Scenario — [Short descriptive name]`
2. **Frontmatter block** in plain text:
   - `**Track / level:**` (e.g., `Track 1, L100`)
   - `**Domain:**` (industry / function / audience)
   - `**Time to run:**` (minutes for live demo)
   - `**Status:**` (one of: `proposed`, `validated`, `archived`)
3. **The role** — 2–3 sentences naming a specific function and context
4. **The current workflow (no AI)** — numbered list of 3–5 steps + time estimate + pain points
5. **The AI-augmented workflow** — same step structure, naming where AI assists and where the human still decides
6. **Responsible AI checkpoint** — three sub-bullets: Privacy/fairness, Human review, Failure mode
7. **Success metric** — concrete, measurable, with a baseline and a target
8. **Facilitator notes** — what to demo, what to assign, common stumbling points

If you're editing a file that's missing one of these sections, **add the section** rather than removing the others.

## Hard rules

- **No real names of people, customers, or partners.** Use placeholders like Contoso, Fabrikam, or generic role descriptions.
- **No real email addresses, tenant IDs, subscription IDs, or GUIDs.** If an identifier is needed for illustration, use obviously-fictional values (`aaaaaaaa-bbbb-cccc-dddd-eeeeeeeeeeee`).
- **No internal-only references** — no internal session names, newsletters, deck titles, or non-public URLs.
- **Status field must be honest.** Mark `proposed` if the scenario hasn't been run live yet. Don't claim outcomes that didn't happen.

## Style

- **Specific over generic.** "A customer support manager at a 200-person SaaS company" beats "a manager."
- **Active voice.** "Run the workflow" not "the workflow is run."
- **Vendor-neutral by default.** Name a specific product only when the lesson requires it (e.g., a Copilot Studio scenario should name Copilot Studio).
- **Plain English.** No internal jargon. Acronyms expanded on first use.
- **Concrete metrics.** "Triage time dropped from 12 min to 4 min" beats "improves efficiency."

## The success metric — quality bar

The success metric is the single most-skipped section. It should answer **all four** of:

- **What is being measured** (time, quality, volume, cost, satisfaction)
- **The baseline** (today's number, even if estimated)
- **The target** (what success looks like)
- **The unit** (minutes, percent, dollars, count)

If any of the four are missing, mark the section `[needs more detail]` rather than leaving it vague.

## The Responsible AI checkpoint — quality bar

Each of the three sub-questions needs a substantive answer (one sentence minimum, not "yes" or "n/a"):

- **Privacy / fairness:** name the data the AI processes; identify a plausible leak or bias risk.
- **Human review:** name *who* reviews and *when* in the workflow — not just "a human reviews it."
- **Failure mode:** name the worst plausible outcome and whether the human review is proportionate to that risk.

Hand-wavy RAI answers undermine the whole scenario and the curriculum's signature practice. Push back on weak answers.

## File naming

Pattern: `scenarios/track[N]-[short-kebab-case-name].md`

Examples:
- `scenarios/track1-customer-support-triage.md`
- `scenarios/track2-onboarding-faq-agent.md`
- `scenarios/track6-incident-post-mortem-assist.md`

For Track 6 sub-topics, optionally include the topic number: `track6t2-vendor-evaluation.md`.

## What not to include

- Customer-identifying details, even anonymized in a way that's still recognizable
- Speculative outcomes presented as facts (use `proposed` status instead)
- Vendor-loaded examples that wouldn't work with comparable tools (unless the lesson is specifically about that vendor's capability)
- Marketing language ("revolutionary," "game-changing," "exciting opportunity")
- Personal opinions presented as universal truths

## When uncertain

Open an issue rather than guessing. See `CONTRIBUTING.md` for the workflow. Better a slow merge than a scenario that has to be rolled back.
