# AI Approach

## Purpose

Explains how AI and deterministic system components work together. AI is used for probabilistic tasks such as language understanding and recommendations, while deterministic services handle validation, permissions, authorization, state management, execution, and auditing.

## Product Principle

AI should reduce complexity without removing user control.

The AI should assist with:

- Understanding intent
- Suggesting workflow components
- Explaining configuration
- Identifying missing parameters
- Detecting potential problems

The AI should not independently activate workflows.

## AI vs Deterministic Logic

AI is useful for:

- Natural language understanding
- Recommendations
- Summarization
- Ambiguous user requests

Deterministic logic should remain responsible for:

- Validation
- Authorization
- Workflow execution
- Permissions
- State changes
- Audit logging

## Example

User:

"Create a ticket whenever a production server goes offline."

AI:

```json
{
  "trigger": "machine_offline",
  "conditions": [
    {
      "field": "environment",
      "operator": "equals",
      "value": "production"
    }
  ],
  "actions": [
    {
      "type": "create_ticket",
      "priority": "high"
    }
  ]
}
