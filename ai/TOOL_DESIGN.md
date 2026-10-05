# AI Tool Design

## Purpose

Defines the controlled tools available to the AI assistant and the principles governing tool access. It demonstrates how AI can interact with platform capabilities through explicit, permission-aware interfaces rather than unrestricted system access.

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
