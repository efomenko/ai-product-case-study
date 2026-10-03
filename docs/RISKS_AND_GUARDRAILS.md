# AI Risks & Guardrails

## Hallucination

### Risk

AI may suggest a trigger or action that does not exist.

### Mitigation

Use a controlled catalog of available workflow components.

---

## Unauthorized Actions

### Risk

AI could generate an unsafe automation.

### Mitigation

AI generates a proposal only.

User approval is required before activation.

---

## Prompt Injection

### Risk

User-provided content could attempt to manipulate the AI.

### Mitigation

- Separate system instructions from user content
- Validate tool parameters
- Restrict available tools
- Log AI decisions
- Apply authorization checks

---

## Incorrect Workflow Logic

### Risk

AI may misunderstand the user's intention.

### Mitigation

Show the generated workflow visually and require confirmation.
