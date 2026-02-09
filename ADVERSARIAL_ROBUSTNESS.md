# Governance Tier 4: Adversarial Robustness

To ensure agent code is "Safe," the framework must treat all incoming instructions—whether from the user or the web—as potentially hostile.

## 1. Prompt Injection Shield
The Governor acts as a "Guardrail Proxy." It evaluates the Executor’s output before it reaches the system terminal or the user's screen to detect:
- **Escape Sequences:** Attempts to break out of the sandbox.
- **Social Engineering:** Attempts to manipulate the user into lowering their "Sustainability" thresholds.

## 2. Deterministic Fail-Safes
The framework includes a "Hard-Code Layer" that overrides AI logic. These are non-negotiable rules defined in `rules.json`:
- `NEVER_DELETE_SYSTEM_FILES: true`
- `MAX_FINANCIAL_TRANSACTION: $50.00`
- `MANDATORY_HUMAN_CONFIRMATION_ON_EMAILS: true`

No amount of "AI reasoning" can override these hard-coded security primitives.
