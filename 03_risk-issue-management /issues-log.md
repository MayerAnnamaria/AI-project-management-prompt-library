# Project Issues Log

## Purpose

Use this prompt to convert an active project problem into a structured issue record and define the actions required to resolve it.

A **risk** is an uncertain future event.

An **issue** is a problem that has already occurred and now requires active management.

The objective is to ensure that significant problems are:

- documented,
- assessed,
- owned,
- resolved,
- escalated where necessary,
- and tracked until closure.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment / Hypercare

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Issue Owner

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Continuously during delivery, with formal review during project reporting

---

# Prompt 1 — Convert a Materialised Risk Into an Issue

```text id="issue-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, issue management, stakeholder coordination,
project governance, and escalation.

TASK

Convert the materialised project risk below into a formal project
issue entry.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target milestone:
[MILESTONE / DATE]

RELATED RISK

Risk ID:
[RISK ID]

Original risk:
[RISK DESCRIPTION]

Current risk rating:
[RATING]

WHAT HAS NOW OCCURRED

[DESCRIBE THE EVENT THAT HAS MATERIALISED]

KNOWN IMPACT

Schedule:
[DETAILS]

Cost:
[DETAILS]

Scope:
[DETAILS]

Quality:
[DETAILS]

Security / Compliance:
[DETAILS]

Operations:
[DETAILS]

Stakeholders:
[DETAILS]

OUTPUT FORMAT

Create a formal issue entry with:

Issue ID
Related Risk ID
Date Raised
Issue Category
Issue Description
Root Cause
Current Impact
Schedule Impact
Cost Impact
Scope Impact
Quality / Technical Impact
Priority
Resolution Actions
Issue Owner
Action Owners
Target Resolution Date
Escalation Required?
Decision Required
Decision Owner
Current Status
Closure Criteria
```

---

# Risk-to-Issue Conversion

When a risk materialises:

```text id="risk-to-issue"
Risk
↓
Event occurs
↓
Issue created
↓
Immediate containment
↓
Root cause analysis
↓
Resolution actions
↓
Decision / escalation
↓
Closure
```

Do not leave an event recorded only as a future risk after it has already occurred.

The related risk should normally be:

- closed as materialised,
- linked to the new issue,
- or updated according to the organisation's risk-management process.

---

# Issue Statement

A strong issue statement should explain:

```text id="issue-structure"
What happened
+
Why it matters
+
Current project impact
```

### Weak

```text id="issue-weak"
API problem.
```

### Better

```text id="issue-better"
The external identity provider missed the agreed API certification
date by 10 working days.

Integration testing cannot complete against the production-equivalent
service until certification is available, creating a potential delay
to the planned UAT start.
```

---

# Issue Categories

Possible categories include:

```text id="issue-categories"
Schedule
Scope
Budget
Resources
Technical
Architecture
Integration
Data
Security
Quality
Testing
Vendor
Procurement
Compliance
Operations
Stakeholder
Governance
Change
```

Use only categories relevant to the project.

---

# Issue Priority

Use an agreed organisational priority model where available.

Example:

```text id="issue-priority"
Critical
Immediate management or governance action required.

High
Material project impact requiring active resolution.

Medium
Manageable impact requiring tracked action.

Low
Limited impact; monitor until closure.
```

Priority should reflect actual project impact and urgency.

---

# Immediate Containment vs Resolution

Separate short-term containment from permanent resolution.

## Containment

Limits immediate project impact.

Example:

> Use the approved mock service so eligible integration testing can continue.

## Resolution

Removes the underlying issue.

Example:

> Complete external API certification and validate the production-equivalent integration.

Both may be required.

---

# Resolution Action Structure

For every significant issue provide:

| Action | Purpose | Owner | Due Date | Status |
|---|---|---|---|---|

Avoid generic actions such as:

```text id="issue-bad-action"
Follow up with vendor.
Monitor progress.
Discuss with team.
```

Prefer:

```text id="issue-good-action"
Vendor Delivery Lead to submit a dated recovery plan by Thursday,
including revised certification milestones and additional capacity
options.
```

---

# Root Cause Review

For material issues, distinguish:

```text id="issue-root-cause"
Symptom
Immediate Cause
Underlying Cause
Systemic Cause
```

Example:

```text id="issue-root-example"
Symptom:
UAT start is at risk.

Immediate Cause:
API certification is late.

Underlying Cause:
Vendor resource allocation was lower than planned.

Systemic Cause:
The dependency had no agreed escalation threshold or recovery plan.
```

This prevents the project team from treating symptoms as root causes.

---

# Impact Assessment

Assess the issue across relevant dimensions:

```text id="issue-impact"
Schedule
Budget
Scope
Quality
Security
Compliance
Operations
Customer
Stakeholders
Business Value
```

Do not automatically mark every dimension as affected.

---

# Example Input

```text id="issue-example-input"
Project:
Customer Portal

Current Phase:
Integration Testing

Related Risk:
R-01 — External identity-provider certification may miss
the planned integration date.

What Has Occurred:
The identity provider has missed the certification milestone
by 10 working days.

Known Impact:
Production-equivalent authentication cannot currently be tested.

Potential Schedule Impact:
UAT start may slip by one week.

Current Action:
Integration team is using a mock authentication service
for eligible tests.

Vendor has not yet submitted a formal recovery plan.
```

---

# Example Issue Entry

| Field | Value |
|---|---|
| Issue ID | I-01 |
| Related Risk | R-01 |
| Category | Vendor / Integration |
| Priority | High |
| Issue | Identity-provider certification is 10 working days late |
| Schedule Impact | UAT start potentially delayed by one week |
| Immediate Containment | Continue eligible integration tests using approved mock service |
| Resolution Action | Obtain vendor recovery plan and revised certification date |
| Issue Owner | Project Manager |
| Action Owner | Vendor Delivery Lead |
| Escalation | Required if revised certification misses UAT dependency date |
| Status | Open |

---

# Prompt 2 — Issue Resolution Analysis

```text id="issue-resolution"
ROLE

You are a senior IT Project Manager reviewing an active project issue.

TASK

Assess the issue below and recommend a structured resolution approach.

ISSUE

[PASTE ISSUE ENTRY]

Analyse:

1. Root cause
2. Immediate containment
3. Permanent resolution
4. Dependencies
5. Decision required
6. Escalation requirement
7. Recovery impact
8. Closure criteria

OUTPUT FORMAT

Root Cause
Immediate Action
Resolution Action
Owner
Deadline
Dependency
Decision Required
Escalation Trigger
Closure Criteria
```

---

# Decision Required

Some issues cannot be solved only through delivery actions.

Examples:

```text id="issue-decisions"
Approve additional budget
Defer scope
Move release date
Accept temporary workaround
Approve production exception
Change vendor
Add resources
Re-sequence delivery
Accept residual operational impact
```

Where a decision is required, make it explicit.

Use:

```text id="issue-decision-format"
Decision Required:
[DECISION]

Decision Owner:
[OWNER]

Decision Deadline:
[DATE]

Impact if Decision Is Late:
[IMPACT]
```

---

# Escalation Criteria

Escalate an issue when:

```text id="issue-escalation"
Critical milestone is threatened.

Impact exceeds project tolerance.

Resolution requires authority outside the project team.

Additional budget is required.

Security or compliance risk exists.

A critical vendor repeatedly misses commitments.

Multiple workstreams are affected.

The accountable decision-maker is not responding within
the required timeframe.
```

---

# Prompt 3 — Management Status Update

Use the issue log to create a concise reporting update.

```text id="issue-reporting"
ROLE

You are a senior IT Project Manager preparing a concise status
update for project governance.

TASK

Write a 3–4 sentence management update for the issue below.

ISSUE

[PASTE ISSUE ENTRY]

Include:

- what has occurred,
- current impact,
- action being taken,
- decision or escalation required,
- expected next update.

Use professional, factual, non-emotional language.
```

---

# Example Status Update

> The external identity provider has missed the agreed API certification milestone by 10 working days, creating a potential one-week impact to the planned UAT start. Eligible integration testing is continuing using the approved mock service while a vendor recovery plan is being requested. The issue will be escalated if the revised certification date does not protect the UAT dependency. A confirmed recovery forecast is required before the next project status review.

---

# Open Issue Reporting

An issue should remain visible in formal reporting until:

```text id="issue-reporting-cycle"
Resolved
Closed
Accepted
Transferred to operational ownership
Superseded by an approved decision
```

Do not remove unresolved issues from reports simply because there has been no change.

Where appropriate, state:

```text id="issue-no-change"
Status unchanged — resolution actions remain in progress.
```

---

# Issue Age

For long-running issues, track:

```text id="issue-age"
Date Raised
Current Age
Target Resolution Date
Days Overdue
```

Ageing issues can signal:

- ineffective resolution actions,
- insufficient authority,
- dependency failure,
- or weak escalation.

---

# Issue Trend Review

During each review, ask:

```text id="issue-review"
Is impact increasing?

Is the resolution date still realistic?

Are actions overdue?

Is the root cause understood?

Has the issue created new risks?

Is the workaround creating technical debt?

Does the issue require governance escalation?

Can the issue be closed?
```

---

# Agile / Scrum Considerations

Issues may surface through:

- Sprint delivery,
- blocked backlog items,
- defects,
- dependency failures,
- release readiness,
- Product Owner decisions.

Where the issue is operational and team-level, resolve it within normal delivery mechanisms where possible.

Escalate only when project-level authority or governance is required.

---

# Kanban Considerations

Issue signals may include:

- blocked work,
- ageing items,
- repeated WIP-limit breaches,
- bottlenecks,
- SLE breaches.

Example:

```text id="issue-kanban"
Signal:
Critical integration work has been blocked for eight days.

Issue:
External approval has not been provided.

Action:
Escalate approval dependency and prevent additional work
from entering the blocked workflow stage.
```

---

# Predictive Considerations

Issue analysis may include:

- schedule variance,
- milestone impact,
- critical-path impact,
- budget impact,
- change control,
- recovery planning.

---

# Hybrid Considerations

Separate delivery handling from project governance.

Example:

```text id="issue-hybrid"
Delivery workaround
↓
Project impact assessment
↓
Formal issue
↓
Governance decision if tolerance exceeded
```

---

# Issue Closure Criteria

Do not close an issue because discussion has stopped.

Define measurable closure criteria.

Examples:

```text id="issue-closure"
Vendor certification completed.

Critical defect fixed and retested.

Security approval formally received.

Required decision documented.

Data reconciliation passes agreed threshold.

Operational workaround removed.
```

Before closure confirm:

```text id="issue-close-check"
Resolution completed
Impact addressed
Evidence available
Required stakeholders informed
Related risks updated
Lessons captured if material
```

---

# Issues Log Format

Recommended register:

| ID | Date Raised | Category | Description | Priority | Impact | Owner | Target Date | Status |
|---|---|---|---|---|---|---|---|---|

For complex projects, additionally include:

```text id="issue-extra-fields"
Related Risk
Root Cause
Decision Required
Escalation Level
Current Workaround
Resolution Action
Action Owner
Closure Criteria
```

---

# Quality Checklist

Before accepting an issue entry, confirm:

- [ ] The event has actually occurred
- [ ] The issue is clearly described
- [ ] Current impact is explicit
- [ ] Root cause is assessed where appropriate
- [ ] Immediate containment is defined
- [ ] Resolution actions are specific
- [ ] Owner is assigned
- [ ] Target resolution date exists
- [ ] Escalation criteria are visible
- [ ] Decisions are explicit
- [ ] Closure criteria are measurable
- [ ] Related risks are updated
- [ ] Issue remains visible until formally closed

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- issue management,
- risk monitoring,
- problem solving,
- stakeholder communication,
- escalation,
- governance,
- decision-making.

## PMBOK Relevance

This prompt supports:

- delivery,
- risk,
- governance,
- measurement,
- stakeholders.

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

Material issues should be reviewed by:

- Issue Owner
- Project Manager
- relevant technical or business leads
- vendor leads where applicable
- Sponsor / Steering Committee where escalation is required

AI can structure issue analysis and identify missing information.

It cannot approve exceptions, accept impacts, or close material issues on behalf of accountable stakeholders.

---

# Confidentiality

Issue logs may contain sensitive information.

Protect:

- security incidents,
- vendor-performance concerns,
- personal performance information,
- customer data,
- commercial disputes,
- confidential financial impact,
- regulatory matters.

Use anonymised information where required.

---

# Prompt Metadata

```text id="issue-metadata"
Prompt ID: RISK-005
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Issue Owner / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT issues-log and risk-to-issue workflow |
