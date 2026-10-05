# Structured Output

## Purpose

Defines the structured format expected from the AI when generating workflows. It explains schema validation, required fields, data types, allowed values, and how structured output reduces ambiguity and makes AI-generated configurations safer to process.

The AI should return a structured workflow rather than free-form text.

Example:

```json
{
  "workflow_name": "Production Server Offline",
  "trigger": {
    "type": "machine_offline"
  },
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
      "parameters": {
        "priority": "high"
      }
    }
  ]
}
