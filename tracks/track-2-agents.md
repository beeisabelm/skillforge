# Track 2 — Building Agents (Copilot Studio, Agent Builder, Azure AI Foundry)

> **The "can my team build something?" track.** Low-code → connector-driven → enterprise orchestration.

## What this track covers

The progression from no-code agents that anyone can build to multi-step orchestrated agents with governance, trust scoring, and human-in-the-loop frameworks.

---

## Level 100 — Foundational

**Audience:** PMs, ops, business managers building their first agent.

**Hands-on focus:** 
No-code agents in Microsoft 365 Copilot Agent Builder, grounded in SharePoint or Teams content. Build something useful in under an hour — onboarding helper, FAQ assistant, document summarizer.

**Outcome:** 
Participant ships one working agent grounded in a real internal data source, demos it to peers, and identifies the next two improvements they'd make.

**Microsoft Learn:**
- [Analyze and visualize data using Microsoft 365 Copilot](https://learn.microsoft.com/en-us/training/modules/analyze-visualize-data-copilot/)
- [Analyze requirements for AI-powered business solutions](https://learn.microsoft.com/en-us/training/modules/analyze-requirements-ai-powered-business-solutions/)
- [Get started with Microsoft Copilot Studio](https://learn.microsoft.com/en-us/training/modules/power-virtual-agents-bots/)

**Live session structure (60 min):**
- 10 min: The "agent" concept — what makes it different from a chatbot or a script.
- 40 min: Hands-on — build one agent from scratch, end to end.
- 5 min: Demo round — show your agent to a peer.
- 5 min: RAI checkpoint — what data does it see? Who can use it?

**Reality check for facilitators:** L100 takes about 90 minutes for someone who's never built a bot. If you only have 60, pre-build the SharePoint grounding and have participants do just the agent assembly. Don't promise "everyone ships an agent" — promise "everyone sees how an agent gets built."

---

## Level 200 — Applied

**Audience:** PMs, engineers, TPMs building production-track agents with custom logic.

**Hands-on focus:** 
Custom agents in Copilot Studio with actions, connectors, and plugins. Versioning, environments (dev/test/prod), and governance for agents that touch real data and trigger real actions.

**Outcome:** 
Participant builds an agent with at least one custom action that calls an external system, configures a non-prod environment, and articulates the promotion path from dev to prod.

**Microsoft Learn:**
- [Use Copilot in Power BI](https://learn.microsoft.com/en-us/training/modules/power-bi-copilot/)
- [Power Platform Business Value Toolkit](https://learn.microsoft.com/en-us/training/modules/get-started-center-excellence) *(Center of Excellence guidance)*
- [Design and build integrated AI agent solutions in Copilot Studio](https://learn.microsoft.com/en-us/training/courses/ab-620t00) *(course AB-620T00 — available May 2026)*

**Live session structure (60 min):**
- 10 min: Agent components — actions, connectors, knowledge sources, prompts.
- 35 min: Hands-on — add one custom action to an existing agent, test it in dev.
- 10 min: Promotion discussion — what changes between dev, test, and prod?
- 5 min: RAI checkpoint.

---

## Level 300 — Production

**Audience:** Engineers, TPMs, ops leads building enterprise-grade orchestrated agents.

**Hands-on focus:** 
Multi-step orchestrated agents with MCP integration, manifest-driven deployment, trust scoring, and human-in-the-loop frameworks for high-stakes scenarios.

**Outcome:** 
Participant can design a multi-agent workflow with explicit human approval gates, deploy via manifest, and instrument trust signals (confidence scores, source attribution) into the agent's responses.

**Microsoft Learn:**
- [Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) *(learning path)*
- [Operationalize AI with Azure AI Foundry](https://learn.microsoft.com/en-us/training/paths/operationalize-ai-responsibly/) *(learning path)*

**Open-source tools:**
- **Microsoft Responsible AI Toolbox** — <https://github.com/microsoft/responsible-ai-toolbox>

**Live session structure (60 min):**
- 10 min: From "agent" to "agent system" — when do you need orchestration?
- 35 min: Hands-on — design a 2-agent workflow with one human approval gate.
- 10 min: Trust signals — what does the user need to see to trust the output?
- 5 min: RAI checkpoint — adversarial test the workflow against one common attack pattern.

---

## Common pitfalls

1. **Promising "everyone ships an agent" at L100.** See the reality check above. Promise discovery, not delivery.
2. **Skipping the dev/test/prod conversation at L200.** Agents that touch production data need promotion discipline. Teach it before they need it.
3. **Building L300 multi-agent workflows without trust signals.** Users won't act on agent output they can't verify. Trust signals aren't optional at production scale.
4. **Forgetting the human approval gate.** A multi-step agent that takes irreversible actions without a checkpoint is a future incident. Always have at least one human gate at L300.

---

## Customer workshop variant

For customer-facing sessions, the most effective format is:

- **Pre-work:** customer brings one real internal use case
- **Live (90 min, not 60):** facilitator builds the L100 version live with the customer's data
- **Outcome:** customer leaves with a working prototype, not a generic demo

See [adaptations/for-customer-workshops.md](../adaptations/for-customer-workshops.md) for the full format.

---

## What success looks like

- 30-day metric: % of participants who improved or rebuilt their agent after the session
- 90-day metric: at least one agent deployed beyond the original builder (someone else uses it)
- Long-term: an internal catalog of working agents, with named owners and adoption metrics

---

*Microsoft Learn module titles and URLs occasionally change. If a link 404s, search the module title at [learn.microsoft.com](https://learn.microsoft.com) and open an issue. The canonical link list with last-verified dates lives in [`_module-index.md`](./_module-index.md).*
