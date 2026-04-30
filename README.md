# Skillforge

> *Forge AI fluency from the foundations up.*

A practitioner-tested curriculum for building AI fluency at scale — six tracks, three levels each, mapped to public Microsoft Learn modules and open-source tools.

Built for **enterprise learning leaders, customer-facing sellers and SEs, partner trainers, and internal community pods.** Fork it, adapt it, run it.

---

## Why this exists

Most AI rollouts fail the same way: licenses arrive, a one-hour intro happens, and six months later nobody can prove value. This curriculum was built to fix that — by treating AI capability the way we treat any other professional skill: foundational → applied → production, with Responsible AI baked in from the start.

It's been refined across multiple cohorts and is ready for direct use in:

- **Customer workshops** run by sellers and Solution Engineers
- **Partner enablement** sessions and train-the-trainer programs
- **Internal community pods** and AI Champions programs
- **Self-paced learning paths** for individual contributors

---

## How it's structured

**Six tracks, three levels each:**

| Track | Focus |
|---|---|
| **Track 0 — Responsible AI** | The prerequisite for everything else. Start here. |
| **Track 1 — GitHub Copilot & Copilot CLI** | Foundational tool proficiency for IDE and terminal workflows. |
| **Track 2 — Building Agents** | Copilot Studio, Agent Builder, and Azure AI Foundry. |
| **Track 3 — Prompt Engineering & Context** | The most undervalued track in most curricula. |
| **Track 5 — Memory, Context & Token Economics** | Why agents forget, what context costs, how to design around it. |
| **Track 6 — System-Level Topics** | Decision intelligence, human–AI collaboration, change management, ROI. |

**Three levels per track:**

- **L100 — Foundational** — "Can I use the tool safely?"
- **L200 — Applied** — "Can I integrate it into my team's work?"
- **L300 — Production** — "Can I deploy it at scale with governance?"

**Three stages per session** — pre-work (Microsoft Learn modules), one live hour (scenario-based, hands-on), post-work (templates, recordings, 30/90-day adoption metrics).

---

## Start here

**New to the repo?** Read **[START-HERE.md](START-HERE.md)** — a 5-minute decision tree that points you to the right track and level for your audience.

**Running this for customers, partners, or your team?** Read **[FACILITATOR-GUIDE.md](FACILITATOR-GUIDE.md)** — session formats, runsheets, and what to do before/during/after.

**Want to adapt the format?** See **[adaptations/](adaptations/)**:
- [Customer workshops](adaptations/for-customer-workshops.md) — for sellers and SEs
- [Partner enablement](adaptations/for-partner-enablement.md) — train-the-trainer
- [Internal teams](adaptations/for-internal-teams.md) — community pods, AI Champions

---

## The tracks

| Track | Audience entry point | Link |
|---|---|---|
| **0 — Responsible AI: Start Here** | Everyone — prerequisite | [tracks/track-0-responsible-ai.md](tracks/track-0-responsible-ai.md) |
| **1 — GitHub Copilot & Copilot CLI** | Engineers, PMs, ops new to AI-assisted work | [tracks/track-1-copilot-cli.md](tracks/track-1-copilot-cli.md) |
| **2 — Building Agents** | PMs, business managers, engineers building agents | [tracks/track-2-agents.md](tracks/track-2-agents.md) |
| **3 — Prompt Engineering & Context** | Anyone using AI tools daily | [tracks/track-3-prompt-engineering.md](tracks/track-3-prompt-engineering.md) |
| **5 — Memory, Context & Token Economics** | PMs, engineers, anyone designing AI workflows | [tracks/track-5-memory-tokens.md](tracks/track-5-memory-tokens.md) |
| **6 — System-Level Topics** | Leaders, change agents, finance, ops | [tracks/track-6-system-level.md](tracks/track-6-system-level.md) |

> *Track 4 number is reserved — the Responsible AI content was promoted to Track 0 since it's a prerequisite, not a sequential step.*

---

## Minimum viable version

Don't have a full program? Start with **Track 0 + Track 1 L100** as a single 2-hour pilot.

That's the most common entry point and the smallest credible thing you can run. If it works, you scale. If it doesn't, you've spent two hours and learned what your audience actually needs.

---

## What's included

- **Self-paced pre-work** — links to free Microsoft Learn modules
- **Live session designs** — 60-minute hands-on formats with scenarios
- **Facilitator notes** — what to demo, what to assign, how to time it
- **Templates** — pre-work checklist, live-session runsheet, 30/90-day metrics
- **Adaptations** — customer workshop, partner enablement, internal community variants
- **Scenarios library** — starter set with guidance on adding your own

---

## What's not included (and why)

- **No proprietary tooling** — every tool referenced is publicly available (Microsoft Learn, GitHub, Azure AI Foundry, PyRIT, Responsible AI Toolbox, MCP)
- **No session recordings or presenter slides** — those belong to whoever runs each session
- **No customer-specific scenarios** — the strongest scenarios are *yours*; we provide the structure for adding them ([scenarios/](scenarios/))

---

## Contributing

This is a living curriculum. If you've run a session and learned something, opened a PR is the most useful thing you can do.

- New scenarios → [scenarios/README.md](scenarios/README.md)
- New adaptations (your audience, your format) → [adaptations/](adaptations/)
- Module updates (Microsoft Learn titles drift) → edit the relevant `tracks/*.md`
- Bug reports / missing pieces → open an issue

See [CONTRIBUTING.md](CONTRIBUTING.md) for the workflow.

---

## License & notices

Content in this repository is licensed **CC BY 4.0** — fork, adapt, run your own program, just keep attribution.

See [NOTICE.md](NOTICE.md) for third-party tool attributions and the standard "views are my own" note.

---

## Maintainer

Curated and maintained by the Skillforge community. Issues, PRs, and questions welcome.
