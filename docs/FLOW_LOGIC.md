# Flow Logic

```text
Request row
    ↓
Status = New?
├─ No → Skip
└─ Yes
    ↓
Estimated Cost EUR > 500?
├─ No
│   ↓
│ Route by Request Category
│   ├─ IT → IT notification
│   ├─ Equipment → Operations notification
│   ├─ Marketing → Marketing notification
│   ├─ Maintenance → Maintenance notification
│   └─ Other → General notification
│
└─ Yes
    ↓
    Start and wait for approval
    ↓
    Outcome = Approve?
    ├─ Yes
    │   ↓
    │ Status = Approved
    │ ↓
    │ Route by Request Category
    │ ↓
    │ Department notification
    │
    └─ No
        ↓
        Status = Rejected
        ↓
        Stop
```

## Demonstrated concepts

- Manual trigger for prototype testing
- Excel Online (Business)
- Apply to each
- Conditions and branching
- Expressions
- Approvals
- Row updates
- Email routing
