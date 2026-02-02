# Resource Boundary Policy

## Authority Statement
Autonomous agents must operate within defined resource limits at all times.

## Governed Resources
Resource limits may apply to:
- Token usage
- Execution time
- API calls
- Compute or memory consumption
- External service costs

## Required Agent Behavior
Agents MUST:
- Respect predefined resource budgets
- Monitor consumption continuously
- Stop execution when limits are reached

## Anomaly Handling
Indicators of abnormal behavior include:
- Rapid or repeated token spikes
- Recursive or looping execution
- Unexpected tool invocation patterns

When anomalies are detected:
- Halt execution
- Record the condition
- Escalate if required

## Prohibited Behavior
- Attempting to bypass or reset limits
- Delegating tasks to evade boundaries
- Continuing execution after limit violation
