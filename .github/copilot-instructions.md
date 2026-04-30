# Skillforge — Copilot Instructions

> Repo-level guidance for GitHub Copilot, Copilot Chat, and any AI coding assistant working in this repository.

## What this repo is

**Skillforge** is a practitioner-built curriculum for AI fluency. It's designed to be used by enterprise learning leaders, sellers and Solution Engineers running customer workshops, partner trainers, and internal community pods. The audience for any content generated here is one of those four groups.

## Core writing principles

When generating, editing, or reviewing any markdown content in this repo:

1. **Plain English first.** No internal jargon. No acronyms without expansion on first use. Aim for content a partner trainer or customer-facing SE could hand to a non-technical executive without translation.
2. **Active voice.** "Run the session" not "the session is run."
3. **Vendor-neutral when possible.** Prefer "AI assistant" over naming a specific product unless the product specifically matters to the lesson. When you do name products, name the publicly available ones (GitHub Copilot, Microsoft 365 Copilot, Copilot Studio, Azure AI Foundry, Power BI, Microsoft Entra ID).
4. **Verifiable claims only.** If you write "this works X% of the time" or "studies show," cite the source or remove the claim. Practitioner experience phrased as such ("across multiple cohorts, the most common failure mode was…") is fine.
5. **Short paragraphs.** Three sentences max. Use bullets and tables freely.
6. **Concrete over abstract.** "Triage time per ticket dropped from 12 min to 4 min" beats "improves efficiency."

## Content rules — non-negotiable

These rules exist because this repo is shared externally with customers and partners. Violations have real consequences.

### No personally identifying information
- **No real names** of customers, employees, partners, or session attendees in any file
- **No real email addresses, tenant IDs, subscription IDs, or any GUIDs**
- **No screenshots of internal tools, internal URLs, or internal-only documentation**
- For examples needing identifiers, use obviously-fictional placeholders (`contoso.com`, `aaaaaaaa-bbbb-cccc-dddd-eeeeeeeeeeee`)

### No proprietary or internal-only references
- No internal session series names, internal newsletters, internal deck titles
- No customer names, customer scenarios, or customer-confidential workflows
- No NDA-covered material under any circumstance
- No "this works at \[company\]" — phrase as "across multiple cohorts" or "in practice"

### Microsoft Learn handling
- **Reference modules by title, link to canonical URLs.** Don't paraphrase or republish module content here.
- **Module titles drift.** When in doubt, link to a search query or the Collection landing page rather than a deep link likely to 404.
- See `tracks/_module-index.md` (when present) for verified canonical URLs.

### License and attribution
- Content in this repo is **CC BY 4.0**. Any new content contributed inherits that license. See `NOTICE.md`.
- Open-source tools referenced (PyRIT, Responsible AI Toolbox, Model Context Protocol) keep their own licenses — link to their repos, don't restate license terms.

## Structural rules

### Track files (`tracks/track-*.md`)
Every track file must contain — in this order:
1. Title with track number and one-line framing
2. "What this track covers" — 2–3 sentences
3. **Level 100 — Foundational** with: Audience, Hands-on focus, Outcome, Microsoft Learn modules, Live session structure (60-min table)
4. **Level 200 — Applied** with the same structure
5. **Level 300 — Production** with the same structure
6. Common pitfalls (3–5 bullets)
7. What success looks like (30-day, 90-day, long-term metrics)

Don't add or remove sections without updating `.github/instructions/tracks.instructions.md`.

### Scenario files (`scenarios/*.md`)
Must follow the template in `scenarios/README.md`:
- Role, current workflow, AI-augmented workflow, RAI checkpoint, success metric, facilitator notes
- See `.github/instructions/scenarios.instructions.md` for the enforcement rules

### Adaptation files (`adaptations/*.md`)
Each adaptation targets one audience type (customers, partners, internal teams). Follow the structure of the existing files: when to use, format, pre-work, what to bring, what not to do, success metrics, common pitfalls.

## The Responsible AI checkpoint — embedded everywhere

This is the curriculum's signature practice. **Any session, scenario, or workflow generated for this repo must end with the 3-question checkpoint:**

1. **Privacy / fairness:** What data did the AI see? Could it leak or bias?
2. **Human review:** Where in this workflow does a human still validate the output?
3. **Failure mode:** What's the worst that happens if this gives a wrong answer? Is the consequence proportionate?

If a generated session structure doesn't end with these three questions, the generation is incomplete.

## Tone calibration

- **Confident, not hype-y.** "This is the highest-ROI session" is fine if you can defend it. "Revolutionary AI breakthrough" is not.
- **Honest about limits.** Say what didn't work, what's hard, what consistently fails. The curriculum is more credible when the failures are named.
- **No empty enthusiasm.** No "🚀 Let's go!" No "exciting journey." No "amazing opportunity." This isn't a marketing landing page.
- **Practitioner voice.** Write like someone who has run the session 10 times and is telling a peer what they learned, not like a vendor introducing a product.

## When generating new content

If asked to draft a new track, scenario, adaptation, or template:

1. **Match an existing file's structure.** Don't invent a new format unless explicitly asked.
2. **Prefer extending a file over creating a new one** if the content is similar in scope.
3. **Add a `[needs verification]` tag** next to any specific claim, URL, module title, or metric you can't independently verify. Better to flag than to fabricate.
4. **Run the RAI checkpoint on your own draft.** What could go wrong if a customer or partner reads this and acts on it?

## When fixing content

If editing existing files:
- Don't reformat unrelated sections (keeps PR diffs readable).
- Don't change product names, module titles, or framework references unless explicitly part of the task.
- Preserve the established voice — match the surrounding paragraphs.

## What this repo is *not*

- Not a Microsoft official training product
- Not a sales pitch for any vendor
- Not a personal blog (keep "I" out of curriculum content; use "we" or imperative voice)
- Not a place for internal-only or NDA-covered material under any circumstances

## When in doubt

Open an issue with the question. The maintainer would rather answer a question than review a PR that has to be rolled back.
