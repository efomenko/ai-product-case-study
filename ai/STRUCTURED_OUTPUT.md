# Structured Output

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
