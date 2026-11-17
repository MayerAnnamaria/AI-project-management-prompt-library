# Stakeholder Engagement Plan

## Purpose

Use this prompt to create a structured stakeholder engagement plan for an IT, software, digital transformation, data, infrastructure, or technology-enabled project.

The plan should define:

- who needs to be engaged,
- why they need to be engaged,
- how they should be engaged,
- when engagement should happen,
- who owns the relationship,
- and how engagement effectiveness will be measured.

The objective is not simply to communicate project information.

The objective is to create the level of stakeholder involvement needed to support **decisions, delivery, adoption, and project success**.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery / Change / Deployment

**Project type:**  
Software implementation / Digital transformation / ERP / Data / Cloud / Infrastructure / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Change Lead / Business Analyst

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Created during planning and reviewed throughout the project

---

# Prompt

```text id="stakeholder-engagement-01"
ROLE

You are a senior IT Project Manager experienced in stakeholder
engagement, organisational change, international software delivery,
project governance, vendor management, and cross-functional
communication.

TASK

Create a complete stakeholder engagement plan using the stakeholder
information below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target completion:
[DATE]

Countries / locations:
[LIST]

Languages:
[LIST]

KEY STAKEHOLDERS

[PASTE STAKEHOLDER MATRIX OR LIST]

KNOWN CONCERNS

[LIST]

KNOWN DECISION DEPENDENCIES

[LIST]

OUTPUT FORMAT

1. Purpose and Scope
2. Engagement Objectives
3. Engagement Principles
4. Stakeholder Engagement Activities
5. Decision-Maker Engagement
6. End-User / Business Engagement
7. Vendor / External Partner Engagement
8. Feedback and Concern Management
9. Engagement Effectiveness Measures
10. Plan Review Schedule
```

---

# 1. Purpose and Scope

State:

```text id="engagement-purpose"
Why stakeholder engagement is required

Which project areas it covers

Which stakeholder groups are included

What outcomes the plan should support
```

Example:

> This plan defines how the CRM Replacement project will engage business, technical, operational, vendor, and governance stakeholders throughout delivery and transition to operations.

---

# 2. Engagement Objectives

Possible objectives include:

```text id="engagement-objectives"
Maintain sponsor alignment

Obtain timely decisions

Build user readiness

Reduce resistance

Validate requirements

Resolve dependencies

Support testing

Improve vendor coordination

Prepare operations

Maintain governance transparency
```

Objectives should connect engagement activity to project outcomes.

---

# Weak vs Strong Objective

### Weak

```text id="engagement-objective-weak"
Keep stakeholders informed.
```

### Better

```text id="engagement-objective-good"
Ensure that business decision-makers receive sufficient information
to approve scope, readiness, and release decisions within agreed
governance timelines.
```

---

# 3. Engagement Principles

Use principles such as:

```text id="engagement-principles"
Relevant
Timely
Transparent
Audience-specific
Two-way
Evidence-based
Respectful
Action-oriented
```

---

# Transparency Principle

Communicate:

```text id="engagement-transparency"
Progress

Risks

Decisions

Dependencies

Trade-offs

Changes
```

Do not communicate only positive information.

---

# Audience Principle

Different stakeholders need different information.

Example:

```text id="engagement-audience"
Executive Sponsor
→ Decisions, business value, major risks

Product Owner
→ Scope, priorities, dependencies

Technical Teams
→ Requirements, architecture, blockers

End Users
→ Change impact, training, readiness

Operations
→ Support, monitoring, handover
```

---

# 4. Stakeholder Engagement Activities

Use:

| Stakeholder | Objective | Activity | Method | Timing | Responsible | Success Measure |
|---|---|---|---|---|---|---|

---

# Example

| Stakeholder | Activity | Method | Timing | Owner | Success Measure |
|---|---|---|---|---|---|
| Sponsor | Steering Committee | Meeting + decision paper | Monthly | PM | Decisions made within governance deadline |
| Product Owner | Priority review | Working session | Weekly | PM / PO | Priorities confirmed |
| Security | Design review | Workshop | Milestones | Architect | Approval risks identified early |
| End Users | Product demo | Demo / feedback | Monthly | Change Lead | Feedback captured and addressed |
| Operations | Readiness review | Workshop | Pre-release | PM | Handover gaps closed |

---

# Activity Design Rule

Every activity should answer:

```text id="engagement-activity-rule"
Why are we doing this?

What outcome is required?

Who owns it?

When does it happen?

How will we know it worked?
```

---

# 5. Decision-Maker Engagement

Identify stakeholders who control:

```text id="engagement-decisions"
Budget

Scope

Architecture

Security

Release

Acceptance

Resources

Commercial decisions
```

Provide:

| Decision Owner | Decision Type | Required Information | Timing | Escalation if Delayed |
|---|---|---|---|---|

---

# Example

```text id="engagement-decision-example"
Decision Owner:
Executive Sponsor

Decision:
Approve release-date change.

Information Required:
Schedule impact
Business impact
Recovery options
Risk

Required By:
15 October

Escalation:
Programme Steering Committee
```

---

# 6. End-User / Business Engagement

For users affected by the solution, consider:

```text id="engagement-user"
Requirements workshops

Prototype reviews

Demos

UAT

Training

Readiness surveys

Feedback sessions

Go-live communication
```

---

# User Engagement Principle

Avoid involving users only at the end.

Use:

```text id="engagement-user-flow"
Understand
↓
Validate
↓
Test
↓
Prepare
↓
Adopt
```

---

# Change Impact

Assess:

```text id="engagement-change-impact"
Process change

Role change

System change

Data change

Reporting change

New responsibilities

Training needs
```

Engagement should be stronger where change impact is higher.

---

# 7. Vendor / External Partner Engagement

For vendors, define:

```text id="engagement-vendor"
Delivery governance

Commercial governance

Technical coordination

Risk review

Dependency review

Escalation
```

Example:

| Activity | Frequency | Participants | Purpose |
|---|---|---|---|
| Delivery review | Weekly | PM + Vendor PM | Progress / blockers |
| Commercial review | Monthly | PM + Procurement | Changes / invoices |
| Architecture review | Milestone | Technical Leads | Technical decisions |
| Escalation | Event-driven | Sponsor + Vendor Leadership | Material issue |

---

# Vendor Relationship Principle

Keep delivery and commercial governance connected but distinct.

Example:

```text id="engagement-vendor-governance"
Delivery Issue
→ Delivery Governance

Contract / Cost Issue
→ Commercial Governance
```

---

# 8. Feedback and Concern Management

Stakeholder engagement must allow information to flow back into the project.

Define:

```text id="engagement-feedback"
How feedback is submitted

Who reviews it

How quickly it is acknowledged

How actions are assigned

How resolution is communicated
```

---

# Feedback Register

| ID | Stakeholder | Feedback / Concern | Owner | Action | Status |
|---|---|---|---|---|---|

Suggested statuses:

```text id="engagement-feedback-status"
New
Under Review
Actioned
Closed
Escalated
```

---

# Concern Escalation

Use:

```text id="engagement-concern-flow"
Concern Raised
↓
Acknowledge
↓
Assess
↓
Assign
↓
Resolve / Escalate
↓
Communicate Outcome
```

---

# 9. Engagement Effectiveness

Do not measure engagement only by number of meetings.

Possible indicators:

```text id="engagement-effectiveness"
Decision turnaround time

Stakeholder attendance

Action completion

Approval delays

Feedback volume

User readiness

UAT participation

Training completion

Escalation frequency

Stakeholder sentiment
```

---

# Example Measures

| Measure | Target / Direction |
|---|---|
| Critical decisions overdue | Decreasing |
| UAT participation | Sufficient for planned coverage |
| Open stakeholder actions | Decreasing |
| Readiness gaps | Decreasing |
| Engagement attitude | Stable / improving |

Do not invent numeric targets unless approved.

---

# 10. Plan Review Schedule

Review the plan:

```text id="engagement-review"
At project initiation

At major milestones

Before release

After stakeholder changes

After significant escalation

When attitudes change

When organisational structure changes
```

---

# Engagement Review Prompt

```text id="engagement-review-prompt"
ROLE

You are a senior IT Project Manager reviewing stakeholder
engagement effectiveness.

TASK

Review the engagement plan and recent stakeholder behaviour.

[PASTE PLAN]
[PASTE RECENT OBSERVATIONS]

Identify:

- stakeholders receiving too little attention,
- stakeholders receiving unnecessary communication,
- deteriorating attitudes,
- decision delays,
- feedback not being closed,
- engagement activities that are not producing outcomes.

OUTPUT FORMAT

Stakeholder
Current Concern
Evidence
Recommended Adjustment
Owner
Priority
```

---

# Example Input

```text id="engagement-example-input"
Project:
CRM Replacement

Stakeholders:

Executive Sponsor
High power / High interest / Supportive

Customer Service Director
High power / High interest / Neutral
Concerned about operational disruption.

Security Lead
High power / Medium interest / Unknown
Production approval required.

Customer Service Agents
Low power / High interest / Unknown
Major process change.

Implementation Vendor
Medium power / High interest / Supportive
```

---

# Example Engagement Activities

| Stakeholder | Activity | Method | Timing | Success Measure |
|---|---|---|---|---|
| Sponsor | Steering | Decision-focused meeting | Monthly | Critical decisions resolved |
| Service Director | Readiness review | Workshop | Biweekly pre-go-live | Operational concerns closed |
| Security | Security checkpoint | Workshop | Design + pre-release | Approval path remains on track |
| Agents | Demo / feedback | Demo | Monthly | Feedback incorporated |
| Vendor | Delivery review | Meeting | Weekly | Blockers resolved |

---

# Cultural / International Considerations

Where a project spans countries, languages, or organisational cultures, consider:

```text id="engagement-cultural"
Language needs

Time zones

Meeting accessibility

Communication preferences

Decision-making styles

Written follow-up requirements

Local holidays

Regional working weeks
```

Avoid stereotyping.

Base engagement choices on actual stakeholder needs.

---

# Language Protocol

Where multilingual communication is required:

```text id="engagement-language"
Official project language

Translation requirements

Who validates translated material

Which documents require bilingual issue

Which meetings require interpretation
```

---

# Accessibility

Where relevant consider:

- accessibility of digital communications,
- meeting captions,
- accessible documentation,
- time-zone fairness,
- remote participation.

---

# Complaints / Concerns Process

For major organisational programmes, employees or users may need a clear route for concerns.

Provide:

```text id="engagement-complaints"
Channel

Owner

Acknowledgement

Assessment

Escalation

Resolution

Feedback
```

Example:

> All project-related operational concerns submitted through the project mailbox will be reviewed by the Change Lead and assigned to the appropriate workstream owner.

---

# Agile / Scrum Considerations

Stakeholder engagement may happen through:

- Sprint Reviews,
- demos,
- backlog refinement where appropriate,
- Product Owner interaction,
- release planning.

However, not every executive or governance stakeholder should participate in delivery ceremonies.

---

# Kanban Considerations

Stakeholders may need visibility of:

- blocked work,
- service performance,
- ageing items,
- priority policies,
- delivery predictability.

Use dashboards where they reduce unnecessary status meetings.

---

# Predictive Considerations

Engagement may align to:

- milestone reviews,
- formal approvals,
- change control,
- stage gates,
- acceptance.

---

# Hybrid Considerations

Use both:

```text id="engagement-hybrid"
Continuous delivery engagement
+
Formal governance engagement
```

---

# Engagement vs Communication

These are related but not identical.

```text id="engagement-vs-comms"
Communication
=
Providing / exchanging information

Engagement
=
Actively involving stakeholders to influence decisions, behaviour,
understanding, or outcomes
```

A stakeholder may receive regular reports and still be poorly engaged.

---

# Engagement Risk Review

Identify engagement-related project risks.

Examples:

```text id="engagement-risks"
Sponsor disengagement

Late business decisions

Insufficient user participation

Resistance to change

Weak vendor collaboration

Operations involved too late

Security engaged too late
```

Use the risk register where material.

---

# Quality Checklist

Before finalising the plan, confirm:

- [ ] Engagement objectives are clear
- [ ] Stakeholders are prioritised
- [ ] Decision-makers are identified
- [ ] Engagement activities have owners
- [ ] Timing is defined
- [ ] Success measures exist
- [ ] End users are considered
- [ ] Vendors are considered
- [ ] Operations are considered
- [ ] Feedback process exists
- [ ] Concerns can be escalated
- [ ] Language / cultural needs are considered where relevant
- [ ] Engagement effectiveness will be reviewed
- [ ] Plan will be updated as stakeholder attitudes change

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder engagement,
- communication,
- leadership,
- organisational change,
- governance,
- decision-making.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- team,
- governance,
- communication,
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

Stakeholder engagement strategies should be reviewed by the relevant:

- Project Manager
- Sponsor
- Change Lead
- Business Owner
- Communications team where relevant
- PMO

AI can help structure engagement activities and identify potential gaps.

It cannot replace direct stakeholder relationships or human judgement about sensitive organisational dynamics.

---

# Confidentiality

Stakeholder engagement plans may contain sensitive information about:

- stakeholder attitudes,
- influence,
- resistance,
- internal relationships,
- escalation paths,
- organisational concerns.

Share the detailed plan only with appropriate project leadership.

---

# Prompt Metadata

```text id="stakeholder-engagement-metadata"
Prompt ID: STAKE-002
Category: Stakeholder Management
Version: 1.0
Status: Draft
Owner: Project Manager / Change Lead
Reviewer: Sponsor / PMO
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT stakeholder-engagement plan framework |
