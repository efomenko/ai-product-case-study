
## `ai/TOOL_DESIGN.md`

```markdown
# AI Tool Design

## Available Tools

The AI assistant may access controlled tools such as:

### get_available_triggers()

Returns available trigger definitions.

### get_available_actions()

Returns available actions.

### get_entity_schema()

Returns available fields and data types.

### validate_workflow()

Validates the generated workflow.

### explain_workflow()

Generates a user-friendly explanation.

## Important Principle

The AI should not receive unrestricted access to production systems.

Tools should expose only the minimum capability required for the task.
