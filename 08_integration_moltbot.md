# Moltbot / Clawdbot Integration Guide

Moltbot acts as:
- System executor
- Automation engine
- Command runner

Metronisys acts as:
- Pre-execution governor
- Policy evaluator
- Human impact assessor

Implementation pattern:
1. User request
2. Metronisys evaluation
3. Approved task subset
4. Moltbot execution
5. Feedback loop to human

Moltbot MUST NOT:
- Execute tasks without Metronisys approval
- Self-expand task scope
- Optimize around governance constraints
