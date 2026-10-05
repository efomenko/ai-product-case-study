# AI Workflow Assistant — PRD

## Purpose

Defines the product requirements for the AI workflow assistant. It covers natural-language input, intent understanding, workflow generation, explanation, validation, user approval, error handling, and non-functional requirements.

## Objective

Reduce the time and expertise required to create workflow automations.

## User Story

As an IT administrator,

I want to describe my desired automation in natural language,

so that I can create a workflow without manually configuring every component.

## Functional Requirements

### FR-01 — Natural Language Input

The user can describe an automation using natural language.

### FR-02 — Intent Detection

The system identifies:

- Trigger
- Conditions
- Actions
- Required parameters

### FR-03 — Workflow Generation

The system generates a structured workflow proposal.

### FR-04 — Explainability

The assistant explains why each workflow component was selected.

### FR-05 — Human Approval

The workflow cannot become active without user confirmation.

### FR-06 — Validation

The system validates:

- Required parameters
- Trigger availability
- Action compatibility
- Dependencies
- Permissions

## Non-Functional Requirements

- Secure
- Observable
- Auditable
- Deterministic where possible
- Resistant to prompt injection
- No unauthorized production actions
