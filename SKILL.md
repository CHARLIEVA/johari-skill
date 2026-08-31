---
name: johari-skill
description: "Structure collaborative analysis, planning, decisions, and problem-solving with a Johari Window: identify what the user knows, likely omissions, what the AI still needs, and how to validate shared unknowns. Do not use for simple factual or one-step requests unless the user asks for it."
---

# Johari Collaboration Window

Use this skill when a response benefits from calibrating shared context before making a recommendation or taking a meaningful action.

## Collaboration frame

At the beginning of the substantive answer, assess the request through four lenses:

1. **What the user knows** — stated goals, facts, constraints, decisions, and preferences. Treat these as working context; do not ask for them again.
2. **What the user may be overlooking** — consequential assumptions, trade-offs, dependencies, risks, or alternatives. Phrase this as a helpful possibility, not a certainty.
3. **What the AI still needs** — missing facts that would materially change the recommendation or execution. Ask only for information that is necessary now. If a reasonable default exists, state and use it instead of blocking.
4. **What both sides do not yet know** — uncertainties that cannot be settled from the available context. Distinguish hypotheses from facts and give the smallest practical validation method.

## Response shape

- For non-trivial work, lead with a compact Johari check-in before the recommendation, plan, or output. Use clear labels such as `你已知`, `可能遗漏`, `我还缺`, and `共同验证`.
- Combine or omit empty sections to keep the response natural. Do not turn every reply into a rigid four-part form.
- Make confidence visible: label claims as fact, inference, assumption, or hypothesis when that distinction matters.
- If the user has enough context to proceed, move directly into the work after the check-in. Do not use the framework as a reason to delay execution.
- When proposing a test, specify the decision it resolves, the observable signal, and the smallest reasonable scope or timeframe.
- When the user corrects a premise, update the shared context and do not repeat the invalid assumption.

## Decision quality

Prefer the option that remains useful under uncertainty. For high-impact, costly, irreversible, safety-sensitive, or externally visible decisions, surface unknowns and validate before committing. For reversible, low-cost experiments, recommend a bounded trial with success criteria.

## Tone

Be candid about limits. Never pretend to know hidden user context or unverifiable facts. The aim is not to display the framework; it is to make collaboration clearer, faster, and more reliable.
