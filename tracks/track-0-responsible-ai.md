# Track 0 — Responsible AI: Start Here

> **The prerequisite for everything else.** Treat this as a hard dependency, not a suggestion.

## Why this is Track 0

The failure modes that get organizations in trouble — privacy leaks, biased outputs, ungoverned autonomous action — show up the *first time* someone uses an AI tool, not after they've mastered it. Teach the principles before the tools, not after.

This track covers Microsoft's six Responsible AI principles and the practical checkpoints that turn them into daily practice:

1. **Fairness**
2. **Reliability & Safety**
3. **Privacy & Security**
4. **Inclusiveness**
5. **Transparency**
6. **Accountability**

---

## Level 100 — Foundational

**Audience:** Everyone using AI tools, regardless of role.

**Hands-on focus:** 
Apply the six principles to daily AI tool use. Practice human review, transparency in outputs, and recognizing when AI assistance is and isn't appropriate.

**Outcome:** 
Participant can articulate the six principles, run a 3-question RAI checkpoint on any AI-generated output, and identify two scenarios in their own work where the principles change their workflow.

**Microsoft Learn:**
- [Embrace Responsible AI Principles & Practices](https://learn.microsoft.com/en-us/training/modules/embrace-responsible-ai-principles-practices/)
- [AI fluency: Explore responsible AI](https://learn.microsoft.com/en-us/training/paths/ai-fluency/) *(learning path)*

**Live session structure (60 min):**
- 10 min: Recap of the six principles. One real-world failure example per principle.
- 30 min: Hands-on — apply the 3-question checkpoint (privacy, human review, failure mode) to three artifacts the audience brings.
- 15 min: Group debrief — which principle was hardest to apply?
- 5 min: Commit to one workflow change in the next 30 days.

---

## Level 200 — Applied

**Audience:** PMs, engineers, technical leads, and operations partners integrating AI into team workflows.

**Hands-on focus:** 
Configure RAI guardrails, data loss prevention, and compliance review checkpoints in agent workflows. Apply purview labels and classification policies. Build approval gates for sensitive scenarios.

**Outcome:** 
Participant can design an AI-assisted workflow with explicit RAI checkpoints at trigger points, approval gates, and escalation paths. Can articulate compliance review requirements for their org.

**Microsoft Learn / docs:**
- [Govern, secure, and manage AI](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework) *(Cloud Adoption Framework guidance)*
- [Microsoft Purview data security and compliance protections for generative AI apps](https://learn.microsoft.com/en-us/purview/ai-microsoft-purview) *(covers DSPM for AI, sensitivity labels, DLP, audit, eDiscovery for Copilot)*

**Live session structure (60 min):**
- 10 min: From principles to controls — what does "transparency" look like as a system requirement?
- 35 min: Hands-on — design RAI checkpoints for one real workflow from the audience.
- 10 min: Compliance review — walk through one Purview label or DLP policy together.
- 5 min: RAI checkpoint on the workflow you just designed.

---

## Level 300 — Production

**Audience:** Engineers, security leads, data scientists, and architects deploying AI in high-stakes scenarios.

**Hands-on focus:** 
Adversarial testing, red teaming, trust scoring, and governance for high-stakes AI use. Run automated risk identification against your own agents and prompts.

**Outcome:** 
Participant can stand up a basic adversarial testing pipeline for an LLM-based application, interpret PyRIT and Responsible AI Toolbox outputs, and articulate the governance review process for production deployment.

**Microsoft Learn:**
- [Operationalize AI with Azure AI Foundry](https://learn.microsoft.com/en-us/training/paths/operationalize-ai-responsibly/) *(learning path)*

**Open-source tools:**
- **PyRIT** (Python Risk Identification Tool for generative AI) — <https://github.com/Azure/PyRIT>
- **Microsoft Responsible AI Toolbox** — <https://github.com/microsoft/responsible-ai-toolbox>

**Live session structure (60 min):**
- 10 min: From "RAI principles" to "RAI testing" — what changes at production scale?
- 35 min: Hands-on — run PyRIT against a sample agent. Interpret the output. Discuss remediation.
- 10 min: Governance — what does the review board need to see before this ships?
- 5 min: RAI checkpoint on the testing pipeline itself (meta — testing the tester).

---

## Embedded RAI checkpoint pattern

This is the single most important practice in this curriculum. Every session in every other track ends with this 5-minute checkpoint:

> **Three questions about whatever was just built:**
> 1. **Privacy / fairness:** What data did the AI see? Could it leak or bias?
> 2. **Human review:** Where in this workflow does a human still validate the output?
> 3. **Failure mode:** What's the worst that happens if this gives a wrong answer? Is the consequence proportionate?

Drilling this into every session is the difference between RAI as a slide deck and RAI as muscle memory.

---

## Common pitfalls

1. **Treating RAI as a compliance checkbox.** It's a design discipline, not paperwork. The checkpoint must change behavior, or it's theater.
2. **Burying RAI in an "advanced" track.** People hit the principles on day one with their first prompt. Teach them on day one too.
3. **Skipping the L300 testing.** "We don't have time for adversarial testing" is the sentence right before the incident.

---

## What success looks like

- 30-day metric: % of sessions in other tracks that closed with the 3-question checkpoint
- 90-day metric: at least one workflow change per participant attributable to an RAI checkpoint
- Long-term: the team starts asking the three questions unprompted, in design reviews and standups

---

*Microsoft Learn module titles and URLs occasionally change. If a link 404s, search the module title at [learn.microsoft.com](https://learn.microsoft.com) and open an issue. The canonical link list with last-verified dates lives in [`_module-index.md`](./_module-index.md).*
