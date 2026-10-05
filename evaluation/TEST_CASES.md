# Evaluation Test Cases

## Purpose

Contains representative test scenarios used to evaluate the AI assistant. Cases cover simple requests, complex requests, ambiguous input, missing information, unsupported capabilities, invalid parameters, and potentially unsafe requests.

## TC-01 — Simple Workflow

Input:

"Create a ticket when a server goes offline."

Expected:

Trigger:
`machine_offline`

Action:
`create_ticket`

---

## TC-02 — Condition

Input:

"Create a high priority ticket when a production server goes offline."

Expected:

Trigger:
`machine_offline`

Condition:
`environment = production`

Action:
`create_ticket(priority=high)`

---

## TC-03 — Missing Information

Input:

"Notify the team when the server has a problem."

Expected behavior:

The AI should ask for clarification instead of inventing:

- Which event?
- Which team?
- Which notification method?

---

## TC-04 — Unsupported Action

Input:

"Automatically restart the server whenever it has a problem."

If restart functionality is unavailable, the AI should explain that the
requested action is not supported rather than hallucinating a capability.
