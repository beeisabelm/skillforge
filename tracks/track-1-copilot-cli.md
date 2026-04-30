# Track 1 — GitHub Copilot & Copilot CLI

> **The "can I use it?" track.** Foundational tool proficiency for IDE and terminal workflows.

## What this track covers

GitHub Copilot in the editor, Copilot CLI in the terminal, MCP (Model Context Protocol) for cross-tool skills, and the discipline of validating AI suggestions with human judgment.

---

## Level 100 — Foundational

**Audience:** PMs, ops, business managers, anyone new to AI-assisted work.

**Hands-on focus:** 
Install GitHub CLI and Copilot CLI, authenticate, use Copilot Chat in VS Code, validate suggestions with human judgment. Practice rejecting bad suggestions as much as accepting good ones.

**Outcome:** 
Participant can run Copilot Chat in VS Code and Copilot CLI in the terminal, complete one realistic task (e.g., summarize a document, draft an email, run a CLI command they hadn't memorized), and articulate when they should *not* trust the suggestion.

**Microsoft Learn:**
- [Employ Copilot Chat as AI assistant](https://learn.microsoft.com/en-us/training/modules/employ-copilot-assistant/)
- [Draft and refine business content using Microsoft 365 Copilot](https://learn.microsoft.com/en-us/training/modules/draft-refine-business-content/)

**External docs:**
- GitHub Copilot Getting Started — <https://docs.github.com/copilot>

**Live session structure (60 min):**
- 10 min: What Copilot is (and isn't). The "validate before accept" mindset.
- 35 min: Hands-on — three real tasks from the audience's daily work.
- 10 min: Failure-mode discussion — when did Copilot give bad suggestions? What did you notice?
- 5 min: RAI checkpoint.

**Customer-facing notes:**
For customer workshops, swap "version control and issue trackers" for the customer's actual tooling. K–12 example: lesson planning, parent communication drafts, rubric generation. Healthcare example: patient communication drafts, summarization of public clinical guidelines. The Copilot mechanics are identical — only the scenarios change.

---

## Level 200 — Applied

**Audience:** PMs, engineers, TPMs integrating Copilot into team workflows.

**Hands-on focus:** 
Configure MCP (Model Context Protocol) servers, build cross-tool skills, add explicit approval gates, integrate Copilot with version control and issue trackers.

**Outcome:** 
Participant can configure at least one MCP server, build a multi-tool skill that requires explicit approval before action, and integrate Copilot output with a downstream tool (e.g., creating a work item, opening a PR).

**Microsoft Learn:**
- [Use Copilot in Power BI](https://learn.microsoft.com/en-us/training/modules/power-bi-copilot/)
- [Transform business workflows with generative AI](https://learn.microsoft.com/en-us/training/paths/transform-business-workflows-with-ai/) *(learning path)*
- [Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) *(learning path)*

**Live session structure (60 min):**
- 10 min: What MCP is — and what cross-tool skills unlock.
- 35 min: Hands-on — configure one MCP server, build one skill, run it end-to-end.
- 10 min: Approval-gate design — where in the skill should the human say "yes"?
- 5 min: RAI checkpoint.

---

## Level 300 — Production

**Audience:** Engineers, SREs, technical leads deploying Copilot at organizational scale.

**Hands-on focus:** 
Build enterprise CLI skill libraries, govern cross-team skills, instrument usage telemetry for ROI reporting, integrate with Microsoft Entra ID for identity-aware skills.

**Outcome:** 
Participant can publish a curated skill library to a team, configure identity-aware access (so the skill respects what the *user* can see), and instrument basic telemetry on skill usage for adoption reporting.

**Microsoft Learn:**
- [Architect AI solutions for business productivity](https://learn.microsoft.com/en-us/training/paths/architect-agentic-ai-business-solutions/) *(learning path)*
- [Operationalize AI with Azure AI Foundry](https://learn.microsoft.com/en-us/training/paths/operationalize-ai-responsibly/) *(learning path)*

**Live session structure (60 min):**
- 10 min: From "I built a skill" to "the team uses skills" — the governance gap.
- 35 min: Hands-on — publish a skill, gate access via Entra ID, add telemetry.
- 10 min: ROI question — what does a "useful" skill look like in your telemetry?
- 5 min: RAI checkpoint — what does an identity-aware skill see, and what should it not see?

---

## Common pitfalls

1. **Demoing without validating.** A facilitator who accepts every Copilot suggestion teaches the wrong lesson. Reject suggestions out loud and explain why.
2. **L100 with no hands-on.** A 60-minute Copilot session that doesn't have the audience open Copilot is a webinar, not a workshop.
3. **L300 without identity context.** Skills that ignore identity create exactly the data-leak failures Track 0 warned about.

---

## What success looks like

- 30-day metric: % of participants who used Copilot at least once after the session
- 90-day metric: workflow change attributable to Copilot use (one specific task, time saved, error reduction)
- Long-term: organic skill sharing — participants demo their own skills to peers without being asked

---

*Microsoft Learn module titles and URLs occasionally change. If a link 404s, search the module title at [learn.microsoft.com](https://learn.microsoft.com) and open an issue. The canonical link list with last-verified dates lives in [`_module-index.md`](./_module-index.md).*
