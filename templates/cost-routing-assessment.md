# Kimi + GPT-5.5 Cost Routing Assessment

## Customer

- Customer:
- Product/team:
- Current monthly model spend:
- Current models:
- Main use cases:
- Assessment date:

## Input Samples

| Sample ID | Task Type | Current Model | Monthly Volume Estimate | Customer-Facing? | Quality Risk |
|---|---|---|---:|---|---|
| S-001 |  |  |  |  |  |
| S-002 |  |  |  |  |  |
| S-003 |  |  |  |  |  |

## Recommended Routing

| Task | Current Model | Recommended Model | Reason | Estimated Savings |
|---|---|---|---|---:|
| Summary/classification | GPT-5.5 | Kimi | Frequent and low-risk | 50%-80% |
| First draft | GPT-5.5 | Kimi | Bulk generation can be reviewed | 40%-70% |
| Final copy | GPT-5.5 | GPT-5.5 | Quality-sensitive | 0% |
| Routine support answer | GPT-5.5 | Kimi | Chinese Q&A | 40%-70% |
| VIP customer reply | GPT-5.5 | GPT-5.5 | High risk | 0% |

## Proposed Routing Rules

```text
IF task_type in [summary, classification, extraction, first_draft]
THEN route to Kimi

IF task_type in [final_copy, executive_report, high_value_customer_reply, complex_reasoning]
THEN route to GPT-5.5

IF Kimi confidence/quality check fails
THEN escalate to GPT-5.5

IF monthly budget usage > 80%
THEN alert operator

IF user exceeds daily quota
THEN throttle or require approval
```

## Pilot Scope

Included:

- Unified API endpoint.
- Kimi/GPT-5.5 routing rules.
- Project-level API key.
- Basic usage report.
- Budget alert.
- Failure retry.
- 7-day technical support.

Not included:

- API credit resale.
- Third-party account sharing.
- Region or payment bypass.
- Unlimited traffic.
- Unsupported provider use cases.

## Quote

| Item | Price |
|---|---:|
| 7-day pilot deployment | RMB  |
| Monthly managed gateway | RMB  /month |
| Optional custom workflow | RMB  |

## Success Criteria

- Routing rules accepted by customer.
- Usage report produced.
- Budget alert configured.
- No critical quality drop on high-value outputs.
- Estimated or measured savings documented.
