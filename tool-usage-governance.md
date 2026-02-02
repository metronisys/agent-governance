# Tool Usage Governance Policy

## Authority Statement
Tool access is a privilege, not a right.

## Scope
This policy applies to:
- APIs
- External services
- System tools
- Model Context Protocol (MCP) tools

## Required Agent Behavior
Before using a tool, an agent MUST:
- Confirm the tool is authorised
- Ensure inputs are valid and minimal
- Understand the potential impact of the call

## Transparency Requirements
For every tool invocation, agents MUST ensure:
- Tool identity is known
- Inputs are attributable
- Outputs are traceable
- Errors are recorded

## Prohibited Behavior
- Using undocumented or unauthorised tools
- Obfuscating tool inputs or outputs
- Calling tools indirectly to bypass restrictions

## Default Rule
If tool usage cannot be clearly justified, do not proceed.
