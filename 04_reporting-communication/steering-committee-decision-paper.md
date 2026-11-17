# Steering Committee Decision Paper

## Purpose

Use this prompt to prepare a formal decision paper for a steering committee, project board, sponsor, or executive governance forum.

The paper should help senior stakeholders:

- understand the issue,
- compare realistic options,
- understand trade-offs,
- see the Project Manager's recommendation,
- and make a clear decision within the required timeframe.

The objective is not simply to describe a problem.

The objective is to support a **governance decision**.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / Programme Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
As required for material project decisions

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in international
software delivery, executive governance, commercial decision-making,
risk management, and stakeholder communication.

TASK

Prepare a formal steering committee decision paper for the issue
described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target milestone:
[MILESTONE / DATE]

Overall status:
[GREEN / AMBER / RED]

ISSUE REQUIRING DECISION

[DESCRIBE ISSUE]

WHY A DECISION IS REQUIRED

[EXPLAIN]

DECISION DEADLINE

[DATE]

OPTIONS

Option A:
[DESCRIPTION]

Cost impact:
[DETAILS]

Schedule impact:
[DETAILS]

Scope impact:
[DETAILS]

Risk:
[DETAILS]

Option B:
[DESCRIPTION]

Cost impact:
[DETAILS]

Schedule impact:
[DETAILS]

Scope impact:
[DETAILS]

Risk:
[DETAILS]

Additional options:
[IF APPLICABLE]

PROJECT MANAGER RECOMMENDATION

[IF ALREADY KNOWN]

OUTPUT FORMAT

Create a formal decision paper with:

1. Purpose
2. Background
3. Decision Context
4. Options Analysis
5. Risk and Impact Analysis
6. Recommendation
7. Decision Required
8. Decision Deadline and Consequence of Delay
9. Implementation Actions Following Decision
10. Referenced Attachments / Evidence
```

---

# 1. Purpose

State exactly why the paper is being presented.

Example:

> The purpose of this paper is to obtain Steering Committee approval for the preferred recovery approach following the two-week delay to the data-migration workstream.

Avoid vague wording such as:

> This paper provides an update.

A decision paper should clearly state the decision sought.

---

# 2. Background

Summarise only the information required to understand the decision.

Include:

```text
What happened
When it happened
Current project impact
Actions already taken
Why the project team cannot resolve the matter without governance input
```

Keep detailed chronology in an attachment where necessary.

---

# 3. Decision Context

Explain why the decision matters now.

Consider:

```text
Schedule
Budget
Scope
Quality
Security
Compliance
Operations
Customer impact
Business value
Vendor commitments
Other dependencies
```

Also explain:

- what happens if no decision is made,
- whether the opportunity to act is time-limited,
- what authority is required.

---

# 4. Options Analysis

Provide:

| Option | Cost Impact | Schedule Impact | Scope Impact | Key Risk | Benefit | Overall Assessment |
|---|---:|---|---|---|---|---|

Do not present unrealistic options merely to create the appearance of choice.

Each option should be genuinely actionable.

---

# Option Design Principles

A useful option should explain:

```text
What changes
What it costs
What time it saves or loses
What value it protects
What new risk it creates
What decision or authority it requires
```

---

# Example

```text
Option A — Accept Delay

Impact:
- Release moves by two weeks.
- No additional delivery capacity required.
- Lower execution risk.
- Business launch date affected.

Option B — Add Temporary Capacity

Impact:
- Additional cost of €80,000.
- Potential recovery of one to two weeks.
- Higher coordination overhead.
- Current launch date may remain achievable.
```

---

# 5. Risk and Impact Analysis

For each option assess relevant dimensions:

| Area | Option A | Option B |
|---|---|---|
| Schedule | | |
| Cost | | |
| Scope | | |
| Quality | | |
| Security | | |
| Business Value | | |
| Vendor Risk | | |
| Operational Risk | | |

Do not imply precision where evidence is limited.

Clearly identify assumptions.

---

# Assumption Check

For each option identify:

```text
Confirmed Facts
Assumptions
Dependencies
Information Gaps
```

This prevents an option from appearing more certain than it really is.

---

# 6. Recommendation

The Project Manager should normally provide a clear recommendation.

Use:

```text
RECOMMENDATION

Recommend Option:
[OPTION]

Reason:

1. [REASON]
2. [REASON]
3. [REASON]

Main Trade-Off:
[TRADE-OFF]

Residual Risk:
[DETAILS]
```

Avoid:

> The Steering Committee should choose whichever option it prefers.

Governance stakeholders typically expect the Project Manager to analyse the evidence and recommend a course of action.

---

# Recommendation Quality Test

A strong recommendation should answer:

```text
Why this option?

Why now?

Why not the alternatives?

What value does it protect?

What risk remains?

What evidence supports the recommendation?
```

---

# 7. Decision Required

State the decision in explicit approval language.

### Weak

```text
Please review the options.
```

### Better

```text
Decision Required:

Approve Option B — temporary expansion of the migration team
for six weeks at an estimated additional cost of €80,000.
```

Where appropriate include:

```text
Approved
Rejected
Deferred
Approved with Conditions
```

---

# 8. Decision Deadline and Consequence of Delay

Always include:

```text
Decision Deadline:
[DATE]

Impact if Decision Is Delayed:
[IMPACT]
```

Example:

> If approval is not received by 15 August, the additional resources cannot be mobilised in time to protect the planned UAT start.

This gives governance the timing context required to act.

---

# 9. Implementation Actions Following Decision

For the recommended option provide:

| Action | Owner | Due Date | Dependency |
|---|---|---|---|

This ensures that approval leads directly to execution.

Example:

| Action | Owner | Due |
|---|---|---|
| Approve purchase order | Sponsor / Procurement | 15 Aug |
| Mobilise vendor resources | Vendor Lead | 18 Aug |
| Re-baseline migration activities | Project Manager | 20 Aug |
| Confirm UAT impact | Business Lead | 22 Aug |

---

# 10. Referenced Evidence

Possible supporting evidence:

```text
Project schedule
Risk register
Issue log
Financial analysis
Vendor recovery plan
Technical assessment
Test results
Security assessment
Change request
Forecast data
```

Do not overload the main decision paper with detailed raw data.

Reference supporting evidence where needed.

---

# Example Input

```text
Project:
CRM Replacement

Current Phase:
System Integration Testing

Overall Status:
Amber

Issue:
Data migration preparation is two weeks behind schedule.

Cause:
Unexpected source-data quality problems.

Current Impact:
UAT start is at risk.

Option A:
Accept two-week delay.

Cost Impact:
Minimal additional project cost.

Schedule Impact:
Go-live likely moves by two weeks.

Option B:
Add two temporary migration specialists for six weeks.

Cost Impact:
€80,000.

Schedule Impact:
Potential recovery of one to two weeks.

Risk:
Resources may not recover the full delay.

Business Constraint:
October go-live supports a major customer-service launch.

Decision Deadline:
15 August.
```

---

# Example Output Excerpt

## Purpose

This paper seeks Steering Committee approval for the preferred recovery strategy following the two-week delay to data-migration preparation.

## Options Analysis

| Option | Cost | Schedule | Main Risk |
|---|---:|---|---|
| A — Accept delay | Low incremental cost | Go-live likely moves by 2 weeks | Business launch impact |
| B — Add migration capacity | +€80k | Potential recovery of 1–2 weeks | Recovery not guaranteed |

## Recommendation

**Recommend Option B.**

The additional cost provides the only current option with a realistic opportunity to protect the October launch date. The approach still carries residual recovery risk, so weekly migration checkpoints and an updated forecast should be required.

## Decision Required

Approve up to €80,000 for two temporary migration specialists for six weeks.

**Decision deadline:** 15 August.

---

# Prompt 2 — Options Challenge

Before issuing the paper, test whether the analysis is balanced.

```text
ROLE

You are an independent PMO Director reviewing a steering committee
decision paper.

TASK

Challenge the options analysis below.

[PASTE PAPER]

Check:

- Are all realistic options represented?
- Is one option unfairly favoured?
- Are assumptions explicit?
- Are costs comparable?
- Are schedule impacts comparable?
- Are risks comparable?
- Is the recommendation supported by evidence?
- Is doing nothing a legitimate option?
- Is the decision deadline justified?

OUTPUT FORMAT

Finding
Evidence
Potential Bias / Gap
Recommended Correction
```

---

# Prompt 3 — Executive Simplification

For complex decisions:

```text
ROLE

You are a senior executive communications advisor.

TASK

Reduce the decision paper below to a one-page executive version.

Preserve:

- decision required,
- context,
- options,
- recommendation,
- cost / schedule impact,
- key risks,
- deadline.

Remove unnecessary operational detail.
```

---

# Agile / Scrum Considerations

Steering decisions may relate to:

- release scope,
- capacity,
- strategic priorities,
- product funding,
- major dependencies.

Avoid escalating normal team-level prioritisation decisions that belong with the Product Owner or delivery team.

Governance escalation should be reserved for matters beyond normal delivery authority.

---

# Kanban Considerations

Decision evidence may include:

```text
Persistent bottlenecks
WIP pressure
Ageing work
Throughput decline
SLE breaches
Blocked dependencies
```

Translate these signals into business or delivery impact rather than presenting flow metrics without interpretation.

---

# Predictive Considerations

Options may involve:

- schedule re-baselining,
- critical-path recovery,
- contingency use,
- resource changes,
- scope change.

---

# Hybrid Considerations

A decision may combine:

```text
Project-level governance
+
Adaptive delivery response
```

Example:

> Steering Committee approves additional budget while the delivery team determines how to reprioritise work within the approved recovery envelope.

---

# Decision Log Integration

After the Steering Committee decides, capture:

| Decision ID | Decision | Date | Decision Owner | Conditions | Follow-Up |
|---|---|---|---|---|---|

The final approved decision should not remain only in meeting minutes.

---

# Quality Checklist

Before issuing the paper, confirm:

- [ ] Purpose is explicit
- [ ] Decision required is clear
- [ ] Background is concise
- [ ] Options are genuinely viable
- [ ] Options are assessed consistently
- [ ] Cost implications are visible
- [ ] Schedule implications are visible
- [ ] Risks are explicit
- [ ] Assumptions are visible
- [ ] Project Manager recommendation is included
- [ ] Trade-offs are explained
- [ ] Decision owner is clear
- [ ] Decision deadline is clear
- [ ] Impact of delay is stated
- [ ] Implementation actions are defined

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- governance,
- decision-making,
- stakeholder engagement,
- risk management,
- financial management,
- schedule management,
- business value,
- leadership.

## PMBOK Relevance

This prompt supports:

- governance,
- finance,
- risk,
- schedule,
- stakeholders,
- delivery,
- value.

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

Before distribution, validate:

- option assumptions,
- financial impact,
- schedule impact,
- technical feasibility,
- legal or contractual implications where relevant,
- recommendation,
- decision authority.

AI can structure and challenge the decision paper.

It cannot make the governance decision or approve project expenditure.

---

# Confidentiality

Decision papers may contain highly sensitive information.

Protect:

- commercial strategy,
- vendor negotiations,
- budget information,
- security concerns,
- contractual positions,
- executive discussions,
- personal information.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text
Prompt ID: REPORT-003
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor
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
| 1.0 | YYYY-MM-DD | Initial IT steering committee decision-paper framework |
