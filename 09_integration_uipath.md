# UiPath Agent Integration Guide

Use Metronisys as:
- Agent policy layer
- Decision Orchestrator
- Human-in-the-loop controller

Recommended UiPath patterns:
- Action approval queues
- Human confirmation checkpoints
- Task throttling based on workload
- Priority decay over time

UiPath agents should:
- Log decisions with human rationale
- Pause flows when ambiguity increases
- Escalate ethically sensitive actions
