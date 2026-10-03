# AI Evaluation

## Evaluation Dimensions

| Dimension | Metric |
|---|---|
| Intent Understanding | Intent accuracy |
| Workflow Generation | Valid workflow rate |
| Parameter Extraction | Parameter accuracy |
| Safety | Unsafe action rate |
| User Experience | Correction rate |

## Example Evaluation

Input:

"Create a ticket when a production server goes offline."

Expected:

Trigger:
`Machine Offline`

Condition:
`Environment = Production`

Action:
`Create Ticket`

The evaluation checks whether the generated workflow matches the expected structure.
