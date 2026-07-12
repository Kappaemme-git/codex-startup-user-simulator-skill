---
name: startup-user-simulator
description: Simulate how five plausible customer personas experience a startup, SaaS, app, or landing page and explain why each would convert, hesitate, or leave. Use when Codex needs to test a live URL, localhost app, screenshot, prototype, or landing-page copy for positioning, first-impression clarity, relevance, trust, objections, conversion friction, CTA effectiveness, mobile experience, or prioritized improvements before launch.
---

# Startup User Simulator

Evaluate a real product surface through five evidence-based simulated customers. Make the distinction between simulation and real user research explicit while producing concrete, prioritized fixes.

Read [references/evaluation-framework.md](references/evaluation-framework.md) before scoring or writing the report.

## Workflow

### 1. Establish the test

- Identify the page, product, intended audience, primary conversion action, and test depth.
- Infer missing context from the page when the inference is safe; label it clearly.
- Ask one concise question only when the missing conversion goal or audience would materially change the evaluation.
- Default to five personas and the primary landing-page journey.

Supported inputs:

- public URL or localhost app
- screenshots or design mockups
- pasted landing-page copy
- repository containing a runnable frontend
- two versions for a before/after comparison

### 2. Inspect the actual experience

- Prefer an interactive browser for URLs and localhost apps.
- Inspect desktop and mobile when both are available.
- Review the hero, navigation, social proof, pricing, FAQ, forms, CTA destinations, error states, and important interactions relevant to conversion.
- Record specific page evidence for every important conclusion.
- Do not submit forms, create accounts, make purchases, send messages, or change external state unless the user explicitly requests it.
- If only screenshots or copy are available, evaluate only what is visible and state the limitation.

### 3. Build five plausible personas

Create personas after inspecting the product. Base them on the stated audience, page positioning, price, use case, and buying motion rather than generic demographics.

Ensure the set contains meaningful decision differences, such as:

- strongest-fit user
- skeptical evaluator
- budget-sensitive buyer
- time-constrained buyer
- adjacent or non-technical user

For each persona define the job, context, awareness level, main constraint, decision criteria, and strongest objection. Avoid stereotypes and invented biographical detail.

### 4. Simulate each decision journey

Trace each persona through:

1. first five seconds
2. problem and product comprehension
3. personal relevance
4. trust formation
5. effort, risk, and price evaluation
6. CTA decision

Separate observations from inferences. Tie observations to visible elements or interactions. Score with the bundled framework and label every score:

> Simulated decision score — not a predicted conversion rate.

Never present simulated personas as real customers, interviews, analytics, or statistically valid research.

### 5. Produce the report

Lead with the result, not the methodology. Use this order:

1. **Verdict** — one sentence on who converts and why others leave.
2. **Biggest conversion leak** — the single highest-impact issue with evidence.
3. **Persona scorecard** — persona, job, first impression, trust break, objection, simulated score, and decision.
4. **Five journeys** — concise evidence-backed reasoning for each persona.
5. **Top five fixes** — rank by expected impact and effort; include exact copy or UI changes when useful.
6. **Fastest experiment** — one measurable test the founder can run next.
7. **Limits** — what simulation cannot establish and what requires real users or analytics.

Keep the default report compact and visually scannable. Avoid generic advice such as “improve the design” or “add social proof”; specify the element, reason, persona affected, and proposed change.

## Modes

- **quick**: Inspect the primary page and return the verdict, scorecard, and top five fixes.
- **deep**: Inspect desktop, mobile, important interactions, pricing, and CTA destinations.
- **mobile**: Focus on small-screen comprehension, interaction, and CTA visibility.
- **before-after**: Compare two versions with the same personas and scoring framework.
- **copy**: Focus on positioning, hero copy, objection handling, and CTA language.

Use `quick` by default unless the user requests another mode.

## Quality bar

- Make every major claim traceable to page evidence.
- Prefer five distinct decision models over five cosmetic persona variations.
- Treat scores as structured heuristics, never behavioral forecasts.
- Distinguish product problems from landing-page communication problems.
- Prioritize changes a founder can actually implement.
- End with the strongest next action, not a vague summary.
