# AI Risks

## Purpose

Documents the major risks associated with introducing AI into workflow creation and execution. It covers hallucinations, incorrect workflows, prompt injection, data leakage, unauthorized actions, poor explanations, and model changes, together with proposed mitigations.

| Risk | Impact | Mitigation |
|---|---|---|
| Hallucination | High | Controlled tool catalog |
| Incorrect workflow | High | Validation + human approval |
| Prompt injection | High | Tool isolation + input controls |
| Data leakage | High | Data minimization |
| Unauthorized action | Critical | No direct production execution |
| Poor explanation | Medium | Structured explanations |
| Model drift | Medium | Continuous evaluation |

## Human-in-the-Loop

The user must approve a generated workflow before activation.

This creates an important separation:

AI proposes → System validates → User approves → Platform executes
