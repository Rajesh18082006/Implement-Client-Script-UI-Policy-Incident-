# Configuration Reference

## UI Policy
- Name: High Impact Control
- Table: Incident
- Condition: Impact is High
- Reverse if false: Enabled

## UI Policy Action
- Field: Urgency
- Behavior: Read-only when the high-impact condition is met

## onChange Client Script
- Runs when Impact changes
- Handles the Urgency behavior for high-impact incidents

## onSubmit Client Script
- Prevents saving a High Impact Incident when Assigned To is empty

## onCellEdit Client Script
- Prevents direct State changes through list editing

## Testing
- Mandatory enforcement
- Successful save
- Reverse condition test
- List edit blocking
- Form-based State update
