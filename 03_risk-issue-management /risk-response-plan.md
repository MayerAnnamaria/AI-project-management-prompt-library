# Risk Response Plan

## Purpose

Use this prompt to convert prioritised project risks into specific, owned, and time-bound response actions.

The objective is to move from:

> We know this risk exists.

to:

> We know what we will do, who will do it, when action is required, and what happens if the risk materialises.

A strong risk response plan should define:

- response strategy,
- preventive actions,
- trigger points,
- contingency actions,
- ownership,
- deadlines,
- and expected residual exposure.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / Risk Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
After qualitative risk analysis and during formal risk reviews

---

# Prompt

```text id="risk-response-01"
ROLE

You are a senior IT Project Manager and risk-management specialist
experienced in international software delivery, digital transformation,
vendor management, project governance, and technology risk.

TASK

Create a detailed risk response plan for the highest-priority
project risks listed below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target milestone:
[MILESTONE / DATE]

Risk tolerance:
[IF KNOWN]

TOP RISKS

[PASTE PRIORITISED RISKS]

For each risk provide:

Risk ID
Risk Description
Current Rating
Response Strategy
Specific Preventive Actions
Trigger Point
Contingency Plan
Residual Likelihood
Residual Impact
Residual Score
Residual Rating
Risk Owner
Action Owner
Action Deadline
Review Date
Escalation Required?
```

---

# Response Strategies

Use the response strategy that best fits the risk.

Possible strategies include:

```text id="b1r6ik"
Avoid
Mitigate
Transfer / Share
Accept
Escalate
```

Do not assign a strategy only because it sounds appropriate.

Explain why the strategy fits the specific risk.

---

# Avoid

Change the project approach so the threat no longer exists.

Example:

```text id="c2m6p3"
Risk:
Legacy authentication platform may not support the required
security standard.

Avoidance:
Use the organisation's approved identity platform instead of
extending the legacy authentication solution.
```

---

# Mitigate

Reduce either:

- likelihood,
- impact,
- or both.

Example:

```text id="s323hb"
Risk:
External API delivery may miss the integration-testing window.

Mitigation:
1. Agree API specification freeze by 15 May.
2. Complete interface mock by 20 May.
3. Run weekly dependency review with the supplier.
4. Escalate any milestone variance greater than five working days.
```

---

# Transfer / Share

Move or share responsibility for part of the exposure where appropriate.

Examples may include:

- contractual supplier responsibility,
- insurance,
- specialist provider,
- shared delivery ownership.

Transfer does not mean the Project Manager stops monitoring the risk.

---

# Accept

Accept the risk when:

- exposure is within tolerance,
- mitigation would cost more than the expected impact,
- or no practical response exists.

Acceptance should still define:

```text id="v1g8ji"
Reason for acceptance
Risk owner
Trigger
Contingency
Review date
```

---

# Escalate

Escalate when the response requires authority outside the project team's control.

Examples:

```text id="d1k0r7"
Additional budget required
Committed milestone must change
Risk acceptance exceeds PM authority
Strategic vendor intervention required
Security exception required
Scope decision required
Regulatory exposure exists
```

---

# Specific Response Actions

Each significant risk should have concrete actions.

### Weak

```text id="7dq03l"
Monitor vendor closely.
```

### Better

```text id="8hk7is"
Require the vendor to submit a recovery plan by Friday,
including revised milestone dates, additional capacity options,
and named owners for each overdue deliverable.
```

### Weak

```text id="3mgavh"
Track testing.
```

### Better

```text id="8866xr"
Review critical-defect ageing every business day and escalate
any Severity 1 defect remaining unresolved for more than 48 hours.
```

---

# Action Quality Rule

A response action should ideally define:

```text id="rsbts1"
Action
Owner
Deadline
Expected Risk Reduction
Evidence of Completion
```

Example:

| Action | Owner | Deadline | Expected Effect |
|---|---|---|---|
| Complete API compatibility PoC | Integration Lead | 20 May | Reduce likelihood of integration failure |
| Confirm UAT resources | Business Owner | 1 Aug | Reduce likelihood of testing delay |
| Complete security pre-review | Security Lead | 15 Aug | Reduce release approval risk |

---

# Trigger Points

A trigger is an observable condition indicating that the risk is becoming more likely or that contingency action should begin.

Examples:

```text id="30hcd8"
Vendor milestone more than 5 working days late

Critical defect count remains above threshold 10 days before UAT

Business tester availability below agreed minimum

Security evidence not submitted before review deadline

Cycle time exceeds agreed threshold for three consecutive periods

Data reconciliation failure exceeds agreed tolerance
```

Trigger points should be measurable where possible.

---

# Preventive Action vs Trigger vs Contingency

Keep these three concepts separate.

## Preventive Action

Taken now to reduce exposure.

## Trigger

Evidence that the risk is approaching or has crossed a threshold.

## Contingency

Action activated when the trigger occurs or the risk materialises.

Example:

```text id="37xkvj"
Risk:
Identity-provider certification delay.

Preventive Action:
Hold weekly certification checkpoint and complete test evidence early.

Trigger:
Certification milestone slips by more than five working days.

Contingency:
Use approved mock identity service for non-production integration
testing while certification is completed.
```

---

# Residual Risk

After defining the response, estimate remaining exposure.

Use:

| Risk | Initial Rating | Response | Residual Rating | Rationale |
|---|---|---|---|---|

Do not automatically reduce the rating simply because actions exist.

Only reduce exposure when the planned response can reasonably change likelihood or impact.

---

# Example Input

```text id="risk-response-input"
Project:
Customer Portal

Current Phase:
Integration Testing

Target Go-Live:
30 September 2027

R-01
External identity provider may miss API certification.
Rating: High

R-02
Critical integration defects may remain unresolved before UAT.
Rating: High

R-03
Business users may not be available for UAT.
Rating: High

R-04
Security approval may not complete before release.
Rating: High

R-05
Data migration reconciliation may exceed agreed tolerance.
Rating: High
```

---

# Example Output Excerpt

| Risk | Strategy | Preventive Action | Trigger | Contingency | Owner |
|---|---|---|---|---|---|
| API certification delay | Mitigate | Agree recovery plan and develop mock service | >5-day milestone slip | Continue eligible SIT using mock service | Integration Lead |
| UAT resource shortage | Mitigate | Confirm named testers and backups | <80% tester allocation confirmed | Reduce UAT scope to critical processes and escalate capacity | Business Owner |
| Security approval delay | Mitigate | Submit evidence early and conduct pre-review | Evidence incomplete at review start | Escalate release decision and evaluate revised deployment date | Security Lead |

---

# Prompt 2 — Response Quality Audit

After creating the response plan, run a second review.

```text id="5q2ld3"
ROLE

You are a senior project risk manager performing a quality review
of a project risk response plan.

TASK

Review the response plan below and identify weak or generic actions.

[PASTE RESPONSE PLAN]

Flag actions such as:

- monitor closely,
- keep under review,
- communicate regularly,
- track progress,
- follow up with vendor,
- manage proactively,

unless they contain a specific action, owner, threshold, and timeframe.

OUTPUT FORMAT

Risk
Weak Action
Why It Is Insufficient
Replacement Action
Owner
Deadline
Expected Risk Reduction
```

---

# Management Test

For every High or Critical risk, ask:

```text id="c54t2z"
What are we doing now?

Who owns it?

When must it happen?

How will we know whether it worked?

What event triggers escalation?

What will we do if the risk still materialises?
```

If these questions cannot be answered, the response plan is incomplete.

---

# Dependency-Based Response Planning

Some risks cannot be managed independently.

Example:

```text id="nyycgm"
Vendor API delay
↓
Integration delay
↓
SIT delay
↓
UAT compression
↓
Go-live risk
```

In these cases, create coordinated actions across the risk chain rather than isolated responses.

Provide:

| Risk Chain | Preventive Action | Coordination Owner | Escalation Trigger |
|---|---|---|---|

---

# Agile / Scrum Considerations

Risk responses may be implemented through:

- backlog prioritisation,
- technical spikes,
- dependency removal,
- incremental delivery,
- additional testing,
- earlier stakeholder feedback,
- release-scope adjustment.

Do not assume a long formal mitigation plan is always the best response.

Some Agile risks can be reduced by obtaining evidence sooner.

---

# Kanban Considerations

Where flow data identifies emerging risk, responses may include:

- reducing WIP,
- resolving blocked work,
- changing replenishment priorities,
- removing bottlenecks,
- adjusting policies,
- swarming on ageing work.

Example:

```text id="2b7xr7"
Risk Signal:
Work item age is increasing rapidly in integration review.

Response:
Stop starting lower-priority integration work and prioritise
completion of ageing items until WIP returns below the agreed limit.
```

---

# Predictive Considerations

Responses may involve:

- schedule recovery,
- resequencing,
- contingency use,
- procurement intervention,
- resource adjustment,
- formal change request.

---

# Hybrid Considerations

Use the response mechanism that best fits the actual risk.

Example:

```text id="6yy7bi"
Project-level risk:
Managed through formal governance.

Delivery-level mitigation:
Implemented through backlog reprioritisation or flow changes.
```

---

# Escalation Criteria

Escalate when:

```text id="0pjt55"
Residual risk remains above tolerance.

Required response exceeds project authority.

Additional funding is required.

Committed milestone is threatened.

Risk affects multiple workstreams.

Security or compliance exposure is material.

Vendor intervention requires executive authority.

Business decision is overdue.
```

---

# Response Effectiveness Review

At each risk review, ask:

```text id="yho5if"
Has the action been completed?

Did it reduce likelihood?

Did it reduce impact?

Has the trigger been reached?

Has the residual risk changed?

Is contingency still viable?

Does the owner have sufficient authority?

Should the response strategy change?
```

---

# Quality Checklist

Before accepting the response plan, confirm:

- [ ] Every priority risk has a response strategy
- [ ] Actions are specific
- [ ] Actions have owners
- [ ] Actions have deadlines
- [ ] Triggers are defined
- [ ] Contingency actions exist where required
- [ ] Residual exposure is assessed
- [ ] Generic “monitoring” actions have been replaced
- [ ] Dependencies are considered
- [ ] Escalation criteria are explicit
- [ ] Response effectiveness can be measured

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- risk response planning,
- mitigation,
- contingency planning,
- risk ownership,
- monitoring,
- escalation,
- governance.

## PMBOK Relevance

This prompt supports:

- risk,
- planning,
- delivery,
- governance,
- measurement.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

---

# Human Review Required

Review material responses with:

- Risk Owner
- Project Manager
- Technical or business experts
- Vendor leads where relevant
- Sponsor / Steering Committee where escalation is required

AI may help structure response alternatives.

It should not accept residual risk or approve expenditure on behalf of accountable stakeholders.

---

# Confidentiality

Risk responses may reveal sensitive information.

Protect:

- security weaknesses,
- vendor performance concerns,
- contract positions,
- confidential budget exposure,
- personal performance information,
- customer information.

Use anonymised data where required.

---

# Prompt Metadata

```text id="2n9qx5"
Prompt ID: RISK-004
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager / Risk Manager
Reviewer: Risk Owners / PMO / Sponsor
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: High
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT risk-response planning framework |
