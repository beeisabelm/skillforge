# Track 5 — Memory, Context & Token Economics

> **The "why does my agent forget?" track.** Undervalued by most curricula, overvalued (too deep, too fast) by engineers.

## What this track covers

How agents "remember" within and across sessions, what context costs, and how to design workflows that respect both. Taught at the right altitude per audience — non-engineers don't need token counting; engineers need to internalize cost dashboards.

---

## Level 100 — Foundational

**Audience:** PMs, ops, business managers, learning leads, anyone designing AI workflows without writing code.

**Hands-on focus:** 
How agents "remember" within and across sessions. Token limits and cost implications at a conceptual level. Designing workflows around memory limits and human handoff points.

**Outcome:** 
Participant can articulate why an agent "forgets," design a workflow that compensates (handoffs, summaries, persistent context), and explain to a non-technical colleague why context costs money.

**Microsoft Learn / docs:**
- [Introduction to generative AI and agents](https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/)
- [Concepts for providing context to GitHub Copilot](https://docs.github.com/en/copilot/concepts/context) *(canonical context-plumbing concepts: MCP, Spaces, indexing, content exclusion; CLI-specific guidance lives under the Copilot CLI "Customize Copilot" how-tos)*

**Live session structure (60 min):**
- 10 min: The "context window" concept — without using the word "tokens" in the first 5 minutes.
- 35 min: Hands-on — take one workflow that "should be one prompt" and break it into three with explicit handoffs. Compare outputs.
- 10 min: Cost framing — one analogy, no math.
- 5 min: RAI checkpoint — when memory persists, who else can see it?

**The single sentence that prevents half of "AI is broken" tickets:** 
*"Every time you start a new session, the agent doesn't remember the last one — design your workflow accordingly."*

Drill it. Twice.

---

## Level 200 — Applied

**Audience:** PMs, engineers, TPMs designing agent workflows that go to production.

**Hands-on focus:** 
Inspect and resume sessions. Track token usage. Apply summarization and compaction to reduce cost. Right-size context per task — not every prompt needs the full conversation history.

**Outcome:** 
Participant can inspect the token count of their own prompts, apply at least one compaction technique (summarization, truncation, key-value extraction), and articulate the trade-off between context completeness and cost.

**Microsoft Learn / docs:**
- [Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) *(learning path)*
- [Plan and manage costs for Microsoft Foundry](https://learn.microsoft.com/en-us/azure/foundry/concepts/manage-costs) *(token-based pricing, fine-tune training/hosting/inference billing, budgets, cost analysis)*

**Live session structure (60 min):**
- 10 min: Token counting — what costs what.
- 35 min: Hands-on — take a verbose prompt, compact it three different ways, compare cost and output quality.
- 10 min: When to compact, when not to — the trade-off conversation.
- 5 min: RAI checkpoint — what does compaction throw away that mattered?

---

## Level 300 — Production

**Audience:** Engineers, SREs, TPMs running production agents with cost and identity constraints.

**Hands-on focus:** 
Memory compaction for long-running agents. Configure On-Behalf-Of (OBO) and Federated Identity Credential (FIC) flows with Microsoft Entra ID so agents act with the right identity. Evaluation harnesses. Cost dashboards.

**Outcome:** 
Participant can design a compaction strategy for an agent with a 30-day session lifetime, configure OBO so the agent acts as the user (not as itself), and instrument a cost dashboard with per-user, per-task breakdowns.

**Microsoft Learn / docs:**
- [Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) *(learning path)*
- [Operationalize AI with Azure AI Foundry](https://learn.microsoft.com/en-us/training/paths/operationalize-ai-responsibly/) *(learning path)*
- [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-on-behalf-of-flow) *(OBO)*
- [Workload identity federation concepts](https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation) *(FIC)*

**Live session structure (60 min):**
- 10 min: Long-running agents — the four problems (memory, cost, identity, drift).
- 35 min: Hands-on — configure OBO on a sample agent, run a query, verify it acted with user identity.
- 10 min: Cost dashboard design — what dimensions matter for *your* finance partner?
- 5 min: RAI checkpoint — when an agent acts as the user, who's accountable for the action?

---

## Cross-platform sub-track — Microsoft 365 Copilot memory & personalization

For PMs, ops, and L&D partners specifically supporting Microsoft 365 Copilot rollouts.

**Hands-on focus:** 
How Microsoft 365 Copilot's user memory works, admin controls, retention policies, data residency, and how to communicate this to end users.

**Outcome:** 
Participant can explain to an end user how their Copilot interactions are remembered (or not), where the data lives, and how to opt out. Can configure admin retention policies for their tenant.

**Microsoft Learn / docs:** [Copilot personalization and memory](https://learn.microsoft.com/en-us/microsoft-365/copilot/copilot-personalization-memory) *(tenant admin controls via Microsoft Graph `enhancedPersonalizationSetting`, where memories are stored — Exchange mailbox hidden folder, retention behavior for custom instructions / saved memories / chat history, eDiscovery and DSR handling). Note: feature is in Frontier preview; re-verify next quarterly cadence.*

**Recommended placement:** run as an extension to L100 or L200 for audiences whose primary tool is Microsoft 365 Copilot, not custom agents.

---

## Common pitfalls

1. **Going too deep at L100.** Token diagrams and architecture slides lose non-engineers. Stay at the workflow-and-handoff level for L100.
2. **Skipping L100 because the audience is "technical."** Even technical audiences benefit from the workflow framing. Don't assume engineers have internalized the *workflow* implications of context windows.
3. **L300 without OBO.** Production agents that act as themselves (not as the user) are a security and audit nightmare. Identity flows are non-negotiable at L300.

---

## What success looks like

- 30-day metric: drop in "AI is broken" tickets that were actually context-window issues
- 90-day metric: workflow redesigns that explicitly reference handoffs, summarization, or compaction
- Long-term: cost-per-user and cost-per-task become standard metrics in your AI program reviews

---

*Microsoft Learn module titles and URLs occasionally change. If a link 404s, search the module title at [learn.microsoft.com](https://learn.microsoft.com) and open an issue. The canonical link list with last-verified dates lives in [`_module-index.md`](./_module-index.md).*
