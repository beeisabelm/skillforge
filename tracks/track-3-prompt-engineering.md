# Track 3 — Prompt Engineering & Context Management

> **The "can I get good output?" track — and the highest ROI per learning hour.**

## What this track covers

Why most "AI doesn't work" complaints are actually "my prompt was unclear" complaints. The progression from clear instructions to chain-of-thought, structured outputs, and full RAG architectures.

---

## Level 100 — Foundational

**Audience:** PMs, ops, business managers, anyone using AI tools daily without consistent results.

**Hands-on focus:** 
Clear instructions, role priming, context-setting, iterative refinement. The "edit and re-prompt" loop. Validating outputs against your own expertise before trusting them.

**Outcome:** 
Participant can take a prompt that produces mediocre output and improve it through three rounds of refinement. Can articulate the four core moves: clarity, role, context, examples.

**Microsoft Learn:**
- [Introduction to generative AI and agents](https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/)
- [Draft and refine business content using Microsoft 365 Copilot](https://learn.microsoft.com/en-us/training/modules/draft-refine-business-content/)

**Live session structure (60 min):**
- 10 min: The four core moves of a good prompt.
- 35 min: Hands-on — start with a bad prompt, refine it three times. Compare outputs across the room.
- 10 min: Discussion — which refinement made the biggest difference? Why?
- 5 min: RAI checkpoint.

**Why this is the highest-ROI session in the curriculum:** every participant uses AI tools daily. A 60-minute investment in prompt quality compounds across thousands of future interactions. If you can only run one session, run this one.

---

## Level 200 — Applied

**Audience:** PMs, engineers, TPMs building prompts that go into systems, not just chat windows.

**Hands-on focus:** 
Chain-of-thought prompting, few-shot examples, structured (JSON / schema) outputs. Prompt budgets and token-cost awareness. Designing prompts as reusable components.

**Outcome:** 
Participant can write a prompt that returns structured JSON conforming to a schema, with chain-of-thought reasoning, and at least two few-shot examples. Can estimate the token cost of their prompt.

**Microsoft Learn:**
- [AI fluency: Explore responsible AI](https://learn.microsoft.com/en-us/training/paths/ai-fluency/) *(learning path)*
- [Power Platform Business Value Toolkit](https://learn.microsoft.com/en-us/training/modules/get-started-center-excellence) *(Center of Excellence guidance)*
- [Utilize Azure OpenAI model to create applications](https://learn.microsoft.com/en-us/training/modules/utilize-azure-openai-model-create-app/)

**Live session structure (60 min):**
- 10 min: Why structured output matters — you can't program against prose.
- 35 min: Hands-on — convert a prose-output prompt to a JSON-schema prompt with few-shot examples.
- 10 min: Token cost — estimate the cost per call, multiply by usage volume.
- 5 min: RAI checkpoint.

---

## Level 300 — Production

**Audience:** Engineers, data scientists, architects building RAG and agent systems.

**Hands-on focus:** 
Retrieval-Augmented Generation (RAG) architectures with vector indexing, skill chaining, plan-mode patterns with human approval gates. Prompt evaluation harnesses.

**Outcome:** 
Participant can architect a basic RAG pipeline (vector store + retrieval + generation), instrument prompt evaluation, and design a plan-mode pattern with explicit human approval at decision points.

**Microsoft Learn:**
- [Architect AI solutions for business productivity](https://learn.microsoft.com/en-us/training/paths/architect-agentic-ai-business-solutions/) *(learning path)*
- [Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) *(learning path)*
- [Develop generative AI apps in Azure](https://learn.microsoft.com/en-us/training/paths/develop-generative-ai-apps/) *(learning path — replaces the deprecated "Build a custom copilot with Azure AI Foundry"; 6h 52m, 6 modules covering plan/prepare, model selection, chat-app development, tool use, performance optimization, responsible AI)*

**Live session structure (60 min):**
- 10 min: When you need RAG vs. fine-tuning vs. prompt engineering alone.
- 35 min: Hands-on — stand up a minimal RAG pipeline with one document corpus.
- 10 min: Evaluation harness — how do you know the RAG is working?
- 5 min: RAI checkpoint — what could the retrieval surface that it shouldn't?

---

## Common pitfalls

1. **Skipping L100 because "everyone already prompts."** Most people have never been *taught* to prompt. They've imitated. The four core moves are not obvious until pointed out.
2. **L200 without token cost.** Token-cost awareness is what separates "prompt engineer" from "person who types into a chat window." Don't skip this.
3. **L300 RAG demos with toy data.** Use real domain data, even if it's the audience's public docs. Toy data doesn't surface the retrieval failure modes that make RAG hard.

---

## A facilitator move that always works

Bring three real prompts the audience uses, and refine them live. The audience watches their own work get 3x better in 20 minutes. That's the moment they internalize the lesson.

---

## What success looks like

- 30-day metric: % of participants who report changing how they prompt
- 90-day metric: measurable quality improvement in one specific recurring task (drafting, summarization, analysis)
- Long-term: the team develops a shared prompt library, organically, without being told to

---

*Microsoft Learn module titles and URLs occasionally change. If a link 404s, search the module title at [learn.microsoft.com](https://learn.microsoft.com) and open an issue. The canonical link list with last-verified dates lives in [`_module-index.md`](./_module-index.md).*
