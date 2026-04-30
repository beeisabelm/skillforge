# Facilitator Guide

For anyone running a session from this curriculum — sellers, Solution Engineers, partner trainers, internal community leads, or learning facilitators.

---

## The session format

Every session in this curriculum follows the same three-stage structure. Don't deviate without good reason — the structure is doing more work than it looks like.

### Stage 1 — Pre-work (1–2 weeks before)

- Send the participants the relevant Microsoft Learn module links from the track page.
- **Track these completions.** If you can't see who completed pre-work, you can't recover the session in real time.
- Send one **scenario primer** — a 1-paragraph description of the real workflow you'll work through live. Ask one prep question: *"Where in this workflow do you currently spend the most time?"*
- For customer-facing sessions: confirm tooling access (Copilot license, Azure subscription, GitHub Copilot if relevant). Tooling-not-working in the first 10 minutes kills the session.

### Stage 2 — Live session (60 minutes)

| Minute | Activity |
|---|---|
| **0–10** | Recap the pre-work concepts. Ask one question: *"What surprised you?"* |
| **10–55** | Hands-on with the scenario. Facilitator demos one example, then participants try a variant. Encourage live questions. |
| **55–60** | Q&A + the **Responsible AI checkpoint** (see below). |

**Responsible AI checkpoint** — the last 5 minutes are non-negotiable. Ask three questions about whatever was just built:

1. **Privacy / fairness:** What data did the AI see? Could it leak or bias?
2. **Human review:** Where in this workflow does a human still validate the output?
3. **Failure mode:** What's the worst that happens if this gives a wrong answer? Is the consequence proportionate?

This is the single most underused practice in AI training. Don't skip it.

### Stage 3 — Post-work (the next 30–90 days)

- Share the session recording (if recorded) and templates.
- **30-day check-in:** "Did anyone use what we covered?" Light touch — Teams message, email, or office-hours.
- **90-day check-in:** Measurable adoption — usage telemetry, time saved, workflow changed. This is your evidence for the next session pitch.

---

## Session-level checklist

Before every session:

- [ ] Pre-work sent ≥ 7 days in advance
- [ ] Pre-work completion checked 2 days before (chase non-completers)
- [ ] Scenario primer sent
- [ ] Tooling access confirmed (for hands-on sessions)
- [ ] Backup demo recorded (in case live demo fails)
- [ ] Responsible AI checkpoint questions ready
- [ ] 30-day and 90-day follow-up scheduled in your calendar *now*

---

## Audience-specific guidance

### Running for customers (sellers / SEs)

- **Lead with the customer's stated problem**, not with the curriculum structure. "You said your team spends 3 hours a week on X. Today we'll cover the track that addresses that."
- **Don't pitch the product mid-session.** This is enablement, not a demo. Trust builds faster when you focus on their learning.
- **End with a scoped follow-up offer:** "I'd like to come back in 30 days and see what's changed. What metric should we look at?"
- See [adaptations/for-customer-workshops.md](adaptations/for-customer-workshops.md) for the customer workshop format.

### Running for partners

- **Train-the-trainer focus:** the partner needs to be able to run this themselves after one session.
- Provide the facilitator notes, slide source, and scenario library.
- Cover *why* each step exists, not just what to do.
- See [adaptations/for-partner-enablement.md](adaptations/for-partner-enablement.md).

### Running for internal teams

- **Use real internal scenarios.** "How would we use Copilot for our actual quarterly planning doc?" beats any generic example.
- Pair with an internal champion who'll be available between sessions.
- See [adaptations/for-internal-teams.md](adaptations/for-internal-teams.md).

---

## Three things that consistently go wrong

Across many cohorts, these are the recurring failure modes:

1. **No real scenarios.** Generic examples produce generic engagement. Spend 30 minutes before the session surfacing one real workflow from the audience.
2. **Audience level mismatch.** Half the room is at L100, half at L300. Run a 30-second self-assessment at the start (*"raise your hand if you've already built a custom agent"*) and adjust on the fly. Or split the room.
3. **No follow-up.** The session is forgotten in 14 days without a 30-day check-in. Schedule it before the live session, not after.

---

## What to measure

For every session you run, track at least:

- **Completion rate** — pre-work done / pre-work assigned
- **Live attendance** — registered / attended
- **Activation** — did anyone use the skill in the next 30 days? (1 question survey)
- **Adoption** — did the workflow actually change in 90 days? (1 follow-up call or telemetry)

You don't need a dashboard. A spreadsheet with these four columns per session is enough to demonstrate impact and earn the next session.

---

## When to deviate from the format

- **You have 30 minutes, not 60.** Cut to 5 / 20 / 5 — recap, single hands-on, RAI checkpoint. Drop the Q&A; defer to follow-up.
- **You have a half day.** Run two consecutive tracks (e.g., Track 0 L100 + Track 1 L100) with a 15-minute break. Don't run three — fatigue kills retention after 2 hours.
- **The audience is wildly mixed.** Run L100 content but offer "extension challenges" for advanced participants during the hands-on. Keeps everyone engaged.

---

## Templates and runsheets

Copyable templates live in this repo (coming soon — contributions welcome):

- `templates/pre-work-email.md`
- `templates/live-session-runsheet.md`
- `templates/post-work-30-day-checkin.md`
- `templates/post-work-90-day-survey.md`
- `templates/responsible-ai-checkpoint.md`

If you've built a template that worked, please open a PR.
