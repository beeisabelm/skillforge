# Microsoft Learn Modules — Verification Worklist

> **For maintainer review.** This is the consolidated list of every Microsoft Learn module referenced across the six track files. Verify each title, capture the canonical URL, and flag any that have been retitled or removed. Once verified, the results feed into `tracks/_module-index.md` and the track files get linked.

**Verification process:**
1. Search the module title at <https://learn.microsoft.com>
2. Open the canonical module/learning-path page
3. Paste the URL in the **URL** column
4. Note the date verified in the **Verified** column
5. If a module has been retitled, note the new title in **Notes**
6. If a module no longer exists, mark `❌ removed` and suggest a replacement

When this table is filled in, send it back and I'll incorporate the URLs into the track files (with the module title as link text) and create `tracks/_module-index.md` as the canonical reference.

---

## Track 0 — Responsible AI

| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 0.1 | Embrace Responsible AI Principles & Practices | https://learn.microsoft.com/en-us/training/modules/embrace-responsible-ai-principles-practices/ | Y | L100 |
| 0.2 | AI fluency: Explore responsible AI | https://learn.microsoft.com/en-us/training/paths/ai-fluency/ | Y | L100 |
| 0.3 | Govern, secure, and manage AI *(part of Cloud Adoption Framework for AI)* | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework | Y | L200 |
| 0.4 | Get started with Microsoft Purview AI Hub | (TBD) | N | L200 |
| 0.5 | Operationalize AI with Azure AI Foundry | https://learn.microsoft.com/en-us/training/paths/operationalize-ai-responsibly/ | Y | L300 (also referenced in T1, T2, T5, T6) |

---

## Track 1 — GitHub Copilot & Copilot CLI

| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 1.1 | Employ Copilot Chat as AI assistant | https://learn.microsoft.com/en-us/training/modules/employ-copilot-assistant/ | Y | L100 (also referenced in T6) |
| 1.2 | Draft and refine business content using Microsoft 365 Copilot | https://learn.microsoft.com/en-us/training/modules/draft-refine-business-content/ | Y | L100 (also referenced in T3) |
| 1.3 | Use Copilot in Power BI | https://learn.microsoft.com/en-us/training/modules/power-bi-copilot/ | Y | L200 (also referenced in T3, T6) |
| 1.4 | Transform business workflows with generative AI | https://learn.microsoft.com/en-us/training/paths/transform-business-workflows-with-ai/ | Y | L200 (also referenced in T6) |
| 1.5 | Develop AI Agents on Azure | https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/ | Y | L200 (also referenced in T2, T3, T5, T6) |
| 1.6 | Architect AI solutions for business productivity | https://learn.microsoft.com/en-us/training/paths/architect-agentic-ai-business-solutions/ | Y | L300 (also referenced in T2, T3, T6) |

External (not on MS Learn but referenced):
- GitHub Copilot Getting Started — <https://docs.github.com/copilot> *(no verification needed; canonical)*

---

## Track 2 — Building Agents

| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 2.1 | Analyze and visualize data using Microsoft 365 Copilot | https://learn.microsoft.com/en-us/training/modules/analyze-visualize-data-copilot/ | Y | L100 (also referenced in T6) |
| 2.2 | Analyze requirements for AI-powered business solutions | https://learn.microsoft.com/en-us/training/modules/analyze-requirements-ai-powered-business-solutions/ | Y | L100 |
| 2.3 | Get started with Microsoft Copilot Studio | https://learn.microsoft.com/en-us/training/modules/power-virtual-agents-bots/ | Y | L100 |
| 2.4 | Power Platform Business Value Toolkit | https://learn.microsoft.com/en-us/training/modules/get-started-center-excellence | Y | L200 (also referenced in T3, T6) |
| 2.5 | Create copilot with Microsoft Copilot Studio | https://learn.microsoft.com/en-us/training/courses/ab-620t00 | Partial, this one needs to update the course name to "Design and build integrated AI agent solutions in Copilot Studio" and available in May 2026 | L200 |

---

## Track 3 — Prompt Engineering & Context

| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 3.1 | Understanding generative AI | https://learn.microsoft.com/en-us/training/modules/responsible-ai-studio/ | Y | L100 (also referenced in T5, T6) |
| 3.2 | Apply prompt engineering with Azure OpenAI Service | https://learn.microsoft.com/en-us/training/modules/utilize-azure-openai-model-create-app/ | Partial, the title needs update to utilize Azure OpenAI model to create applications | L200 |
| 3.3 | Build a custom copilot with Azure AI Foundry | | N | L300 |

---

## Track 5 — Memory, Context & Token Economics

| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 5.1 | (no track-unique modules — uses 1.5, 3.1, T0.5) | n/a | n/a | Track 5 references modules from Tracks 1, 3, 0 |

External / docs (not on MS Learn but referenced):
- Public Copilot CLI / Azure AI Foundry context-management documentation *(needs canonical URL)*
- Public token-management and cost-optimization docs for Copilot CLI and Azure AI Foundry *(needs canonical URL)*
- Microsoft Entra ID identity-flow documentation (OBO / FIC) *(needs canonical URL)*
- Public Microsoft 365 Copilot administration and memory documentation *(needs canonical URL — for the cross-platform sub-track)*

---

## Track 6 — System-Level Topics

### Topic 1 — Decision Intelligence
| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 6.1.1 | Get started with Copilot in Power BI | https://learn.microsoft.com/en-us/training/modules/power-bi-copilot/ | Y | L100 |

*(also references modules from T2 and T1)*

### Topic 2 — Human–AI Collaboration Workflow Design
| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 6.2.1 | Define the role of Microsoft 365 Copilot in business workflow | https://learn.microsoft.com/en-us/training/modules/define-copilot-role-business-workflow/ | Y | L200 |
| 6.2.2 | "Human–AI principles and responsible agent design" guidance | https://microsoft.design/articles/principles-for-responsible-agent-design/ | Partial, yes, it's an article, not learning module. | L200 (may be a doc page rather than a module — flag) |

*(also references 1.1, 3.1, 1.5, T0.5)*

### Topic 3 — Change Management & Organizational Transformation
| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 6.3.1 | Scale AI in your organization | https://learn.microsoft.com/en-us/training/modules/scale-ai/ | Y | L100 |
| 6.3.2 | Transform your business with AI | https://learn.microsoft.com/en-us/training/paths/transform-your-business-with-microsoft-ai/ | Y | L100 |
| 6.3.3 | Plan for AI adoption *(part of Cloud Adoption Framework)* | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai/ | Y | L200 |
| 6.3.4 | Organizational readiness for AI agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/organization-people-readiness-plan | Partial, this is an article, not learning module | L200 |
| 6.3.5 | Define a strategy for adoption and change management | https://learn.microsoft.com/en-us/dynamics365/guidance/implementation-guide/implementation-strategy-define-strategy-adoption-change-management | Partial, this is an article, not learning module | L300 |
| 6.3.6 | AI Readiness Assessment | https://learn.microsoft.com/en-us/assessments/94f1c697-9ba7-4d47-ad83-7c6bd94b1505/ | Partial, this is an interactive assessment tool, not learning module | L300 (may be assessment tool rather than module — flag) |

### Topic 4 — Value Measurement & ROI
| # | Module title (as referenced) | URL | Verified | Notes |
|---|---|---|---|---|
| 6.4.1 | Capture and communicate value with the Business Value Toolkit | https://learn.microsoft.com/en-us/power-platform/guidance/coe/business-value-toolkit | Partial. This is a guide, not a learning module | L200 |

*(also references 2.4, 0.1, 1.6)*

---

## Open-source tools & projects (no verification needed; canonical repos)

| Tool | URL | Notes |
|---|---|---|
| PyRIT (Python Risk Identification Tool for generative AI) | https://github.com/Azure/PyRIT | Track 0 L300, Track 2 L300 |
| Microsoft Responsible AI Toolbox | https://github.com/microsoft/responsible-ai-toolbox | Track 0 L300, Track 2 L300 |
| Model Context Protocol (MCP) | https://modelcontextprotocol.io | Track 1 L200, Track 2 L300 |

---

## Summary by track

| Track | MS Learn modules referenced (unique) | Doc pages / external references |
|---|---|---|
| 0 | 5 | 0 |
| 1 | 6 (1 unique to T1, 5 shared) | 1 (GitHub Copilot docs) |
| 2 | 5 (3 unique to T2, 2 shared) | 0 |
| 3 | 3 (3 unique to T3) | 0 |
| 5 | 0 unique (3 shared) | 4 doc pages |
| 6 | 8 (7 unique to T6, 1 shared) | 0 |
| **Total unique** | **~22 modules** | **~5 doc pages** |

---

## After verification

Send the filled-in URLs back. I'll then:

1. Update each `tracks/track-*.md` file to convert module titles to markdown links
2. Create `tracks/_module-index.md` as the single source of truth (module → URL → last-verified date)
3. Add a footer to each track file: *"Module titles occasionally change on Microsoft Learn — if a link 404s, search the title at learn.microsoft.com and open an issue."*
4. Add a quarterly verification reminder note in `CONTRIBUTING.md`

If any module no longer exists or has been retitled, just note it in the **Notes** column and we'll handle the swap together.
