# Sales Process

## Sales Funnel

```text
Lead identified
-> lead scored
-> first outreach
-> reply
-> 15-minute discovery
-> sanitized samples collected
-> cost-routing assessment delivered
-> 7-day pilot proposal
-> deployment
-> managed monthly service
-> case study and referrals
```

## First Conversation Goal

Do not try to close the gateway immediately.

The first goal is to obtain:

- Current monthly model API cost range.
- Main AI task categories.
- 10-30 sanitized request samples.
- Whether they use one model for all tasks.
- Whether they track usage by user/project/customer.
- Whether they have experienced cost spikes, key leakage, or abuse.

## Discovery Questions

Ask:

```text
What is your current monthly model API spend?
Which model handles most requests today?
Do different task types use different models?
Do you track token and cost by user, project, or customer?
Have you had any API cost spikes?
Do you have user-level limits or budget alerts?
Do external contractors or frontend systems ever touch primary API keys?
Can you share 10-30 sanitized real request examples?
```

If the customer cannot answer most of these, the pain is real.

## Assessment Input

Ask the customer for:

- 10-30 sanitized prompts or request examples.
- Current model used for those requests.
- Approximate monthly call volume per request type.
- Current monthly model cost range.
- Required quality or risk level.
- Whether final output is customer-facing.

Sanitization requirements:

- Remove personal data.
- Remove customer names.
- Remove internal secrets.
- Replace sensitive fields with placeholders.

## Assessment Output

Produce a one-page report with:

- Task category.
- Current model.
- Recommended model.
- Reasoning.
- Estimated savings.
- Risk notes.
- Pilot deployment plan.

Example:

| Task | Current Model | Recommended Model | Reason | Estimated Savings |
|---|---|---|---|---:|
| Summary/classification | GPT-5.5 | Kimi | Frequent and low-risk | 50%-80% |
| First draft | GPT-5.5 | Kimi | Bulk generation can be reviewed | 40%-70% |
| Final copy | GPT-5.5 | GPT-5.5 | Quality-sensitive | 0% |
| Routine support answer | GPT-5.5 | Kimi | Chinese Q&A | 40%-70% |
| VIP customer reply | GPT-5.5 | GPT-5.5 | High risk | 0% |

## Pilot Offer

Offer a 7-day pilot:

```text
7-day pilot deployment: RMB 5,000-15,000

Included:
- Unified endpoint
- Kimi/GPT-5.5 routing rules
- Project-level key
- Basic usage dashboard or report
- Budget alert
- Failure retry
- 7 days technical support
```

Do not offer unlimited traffic in a pilot.

## Managed Service Offer

After the pilot:

```text
Monthly managed gateway: RMB 2,000-8,000/month

Included:
- Monthly usage report
- Routing optimization
- Budget and anomaly alerts
- Issue support
- Key rotation support
- Basic SLA
```

For larger customers, quote higher:

- RMB 10,000-30,000/month if custom routing, private deployment, stronger support, or multiple projects are included.

## Handling Common Objections

### "We can call Kimi and GPT ourselves."

Response:

> Yes. The value is not the raw API call. The value is routing, user-level cost visibility, key governance, budgets, retry/fallback, and monthly operations.

### "We only care about cheaper API."

Response:

> Then we may not be the right fit. We do not sell cheap credits or third-party keys. We reduce cost by routing work correctly and controlling abuse.

### "We need more models."

Response:

> Current pilot focuses on Kimi + GPT-5.5 because that solves the Chinese bulk-work plus high-quality-output split. Additional providers can be added later, but the first pilot should prove routing value.

### "Can you invoice in China?"

Response:

> We can support Singapore invoice directly for customers with cross-border procurement. If a China VAT invoice is required, we can work through a domestic partner or China entity arrangement with adjusted pricing.

## Closing Criteria

Only propose paid deployment if:

- The customer has real AI usage.
- There is a clear task split between routine work and high-value work.
- Monthly cost or operational pain is meaningful.
- They accept compliance boundaries.
- They can provide samples or usage structure.

Do not close customers who want bypass access, anonymous access, or raw key resale.
