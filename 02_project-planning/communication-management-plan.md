# Communication Management Plan

## Purpose

Use this prompt to create a structured communication management plan for an IT, software, digital transformation, data, or infrastructure project.

The plan should define:

- who needs what information,
- when they need it,
- how it should be communicated,
- who is responsible,
- how escalations work,
- and how project information is controlled.

The objective is not to increase communication volume.

The objective is to ensure that the **right information reaches the right stakeholder at the right time in the right format**.

---

## Best Used For

**Project phase:**  
Planning / Delivery

**Project type:**  
Software implementation / Digital transformation / Data / Infrastructure / ERP / Multi-vendor programme

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Create during planning and review after major stakeholder, team, or governance changes

---

# Prompt

```text id="comm-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, stakeholder management, executive communication,
cross-functional coordination, and distributed-team governance.

TASK

Create a professional communication management plan for the project
described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Project duration:
[DURATION]

Primary project language:
[LANGUAGE]

Other stakeholder languages:
[LIST]

Countries / time zones:
[LIST]

Key stakeholders:
[LIST]

Project team:
[LIST]

External vendors:
[LIST]

Governance bodies:
[LIST]

Known communication challenges:
[LIST]

Existing communication tools:
[TEAMS / SLACK / EMAIL / JIRA / CONFLUENCE / OTHER]

Document repository:
[LOCATION]

OUTPUT FORMAT

Create a communication management plan with:

1. Communication Objectives
2. Stakeholder Communication Matrix
3. Governance Communication
4. Team Communication
5. Language and Time-Zone Protocol
6. Escalation Pathway
7. Meeting Cadence
8. Document Control and Distribution
9. Communication Risks
10. Communication Effectiveness Measures
```

---

# 1. Communication Objectives

Define 3–5 objectives.

Examples:

```text id="comm-objectives"
Ensure stakeholders receive decision-relevant information on time.

Maintain clear visibility of project status, risks, issues,
dependencies, and decisions.

Support effective collaboration across business and technical teams.

Provide consistent executive reporting.

Ensure critical escalations reach the appropriate decision-maker
within the required timeframe.
```

---

# 2. Stakeholder Communication Matrix

Provide:

| Stakeholder | Information Need | Method | Frequency | Owner | Format |
|---|---|---|---|---|---|

Possible communication methods:

```text id="comm-methods"
Status report
Dashboard
Steering committee
Project meeting
Daily coordination
Email
Jira
Confluence
Teams / Slack
Risk review
Vendor review
Release review
Executive briefing
```

Avoid communicating the same level of detail to every stakeholder.

---

# Audience-Based Communication

## Project Team

Focus on:

- current priorities,
- blockers,
- dependencies,
- actions,
- decisions,
- delivery risks.

## Business Stakeholders

Focus on:

- progress,
- business impact,
- scope,
- readiness,
- decisions required.

## Executive Sponsor

Focus on:

- overall status,
- business outcomes,
- material risks,
- budget,
- major decisions,
- escalations.

## Technical Stakeholders

Focus on:

- architecture,
- dependencies,
- environments,
- integration,
- security,
- quality,
- technical risks.

## Vendors

Focus on:

- commitments,
- milestones,
- dependencies,
- acceptance criteria,
- issues,
- commercial obligations where relevant.

---

# 3. Governance Communication

Define how governance information is communicated.

Use:

| Governance Topic | Audience | Cadence | Owner | Evidence |
|---|---|---|---|---|

Possible governance topics:

- project status,
- scope changes,
- budget,
- risk,
- major issues,
- vendor performance,
- release decisions,
- benefits,
- escalation decisions.

---

# 4. Team Communication

Define operational communication separately from governance communication.

Examples:

```text id="comm-team"
Delivery coordination
Technical coordination
Backlog discussion
Dependency review
Risk review
Testing coordination
Release coordination
Incident communication
```

Keep meetings purposeful.

For each meeting or communication:

```text id="comm-purpose"
Purpose
Required Participants
Inputs
Expected Output
Decision Rights
Frequency
```

---

# 5. Language and Time-Zone Protocol

For international teams, define:

```text id="comm-language"
Primary project language
Required translation
Official documentation language
Meeting language
Minutes language
Time-zone reference
Core collaboration hours
Response expectations
```

Example:

```text id="comm-timezone-example"
Primary project time zone:
CET

Core overlap:
14:00–17:00 CET

Teams:
Budapest
London
New York

Rule:
Schedule recurring cross-regional meetings inside the agreed
overlap window whenever possible.
```

Avoid repeatedly placing the inconvenience of time-zone differences on the same regional team.

---

# Written Communication Protocol

For material decisions or commitments:

```text id="comm-written"
Document:

Decision
Owner
Date
Rationale
Actions
Deadline
Affected Scope / Cost / Schedule
```

Verbal agreement should not be the sole record for significant project decisions.

---

# 6. Escalation Pathway

Define escalation levels clearly.

Example:

```text id="comm-escalation"
Level 1
Delivery team resolution

Level 2
Project Manager / Delivery Lead

Level 3
Business Owner / Functional Lead

Level 4
Project Sponsor / Steering Committee
```

For each escalation type define:

| Trigger | Escalation Owner | Recipient | Timeframe | Required Information |
|---|---|---|---|---|

Possible triggers include:

- critical blocker,
- milestone risk,
- unresolved dependency,
- security risk,
- budget tolerance breach,
- scope conflict,
- vendor failure,
- production risk.

---

# Escalation Message Structure

Use:

```text id="comm-escalation-structure"
ISSUE

IMPACT

CURRENT STATUS

OPTIONS

RECOMMENDATION

DECISION REQUIRED

DECISION DEADLINE
```

This avoids escalations that merely describe a problem without explaining what management action is required.

---

# 7. Meeting Cadence

Provide:

| Meeting | Purpose | Frequency | Participants | Owner | Required Output |
|---|---|---|---|---|---|

Possible meetings include:

```text id="comm-meetings"
Project Team Meeting
Delivery Coordination
Scrum Events where applicable
Kanban Replenishment / Delivery Review where applicable
Risk Review
Dependency Review
Vendor Review
Testing / Defect Review
Release Readiness Review
Steering Committee
Executive Review
```

Do not create meetings solely because they are common PM practice.

Every recurring meeting should have a clear purpose.

---

# Agile / Scrum Considerations

Where Scrum is used, avoid duplicating formal Scrum events unnecessarily.

Consider:

- Daily Scrum
- Sprint Planning
- Sprint Review
- Sprint Retrospective
- backlog refinement

The project communication plan should complement these events rather than replace them.

---

# Kanban Considerations

Where Kanban is used, communication may include relevant cadences such as:

- replenishment,
- delivery review,
- risk review,
- operations review.

Flow information may include:

- WIP,
- blocked work,
- work item age,
- cycle time,
- throughput,
- Service Level Expectations.

Use only the cadences relevant to the actual system.

---

# Predictive Considerations

Communication may align strongly with:

- milestone reporting,
- baseline reviews,
- change control,
- schedule reviews,
- formal governance.

---

# Hybrid Considerations

Avoid creating two parallel communication systems.

Where Agile delivery operates inside traditional governance, define how team-level information feeds executive reporting.

Example:

```text id="comm-hybrid-flow"
Delivery data
↓
Project-level interpretation
↓
Risk / dependency assessment
↓
Governance report
↓
Decision / escalation
```

---

# 8. Document Control and Distribution

Define rules for:

```text id="comm-doc-control"
Document owner
Storage location
Version control
Approval status
Distribution
Confidentiality
Retention
Access permissions
```

Possible project records include:

- project charter,
- scope,
- requirements,
- project plan,
- RAID register,
- decision log,
- meeting minutes,
- status reports,
- test evidence,
- release approvals.

Avoid multiple uncontrolled copies of critical project documentation.

---

# Single Source of Truth

Where possible, identify the authoritative source for each type of information.

Example:

| Information | Authoritative Source |
|---|---|
| Delivery tasks | Jira |
| Project documentation | Confluence |
| Approved budget | Finance system |
| Risks | RAID register |
| Decisions | Decision log |
| Source code | Git repository |
| Test evidence | Test-management system |

The specific tools will depend on the organisation.

---

# 9. Communication Risks

Provide:

| Communication Risk | Impact | Mitigation | Owner |
|---|---|---|---|

Possible risks include:

```text id="comm-risks"
Stakeholders receive inconsistent status information
Critical decisions are not documented
Language misunderstandings
Time-zone delays
Information overload
Executive reports contain too much detail
Technical issues are communicated without business impact
Vendor escalations happen too late
Actions do not have owners
Multiple document versions circulate
```

---

# 10. Communication Effectiveness Measures

Possible indicators include:

- overdue decisions,
- overdue actions,
- repeated clarification requests,
- escalation response time,
- meeting action closure rate,
- stakeholder feedback,
- number of unresolved communication dependencies.

Do not measure communication solely by the number of meetings or reports produced.

---

# Example Input

```text id="comm-example-input"
Project:
Customer Portal Implementation

Delivery Approach:
Hybrid Agile

Teams:
Budapest development team
London Product Owner
US-based identity provider
External QA partner

Primary Language:
English

Time Zones:
CET
GMT
EST

Tools:
Jira
Confluence
Microsoft Teams
Email

Governance:
Weekly project meeting
Monthly steering committee

Known Challenge:
Identity-provider decisions frequently arrive late because
technical issues are escalated without clear decision deadlines.
```

---

# Example Output Excerpt

## Communication Objective

Ensure that cross-team dependencies and decisions affecting the identity integration are escalated with sufficient context and explicit decision deadlines.

## Communication Matrix

| Stakeholder | Information | Method | Frequency | Owner |
|---|---|---|---|---|
| Development Team | Priorities, blockers, dependencies | Jira + team coordination | Daily | Delivery Lead |
| Product Owner | Scope, priorities, decisions | Teams + Jira | Weekly / ongoing | PM |
| Identity Provider | Integration issues and decisions | Technical call + written action log | Weekly / as required | Integration Lead |
| Steering Committee | Status, risks, decisions | Steering pack | Monthly | Project Manager |

## Escalation Improvement

All identity-provider escalations should include:

- business or delivery impact,
- available options,
- recommended action,
- accountable decision-maker,
- required decision date.

---

# Quality Review

Before approving the communication plan, confirm:

- [ ] Stakeholders are identified
- [ ] Information needs differ by audience
- [ ] Communication owners are clear
- [ ] Frequencies are appropriate
- [ ] Escalation triggers are defined
- [ ] Decision deadlines are visible
- [ ] Language requirements are addressed
- [ ] Time-zone impact is addressed
- [ ] Documentation sources are clear
- [ ] Meetings have defined purposes
- [ ] Communication risks have owners
- [ ] Sensitive information is controlled

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- communication management,
- stakeholder engagement,
- team collaboration,
- governance,
- issue escalation,
- leadership.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- governance,
- team / resources,
- delivery,
- communication,
- decision-making.

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

Validate the communication plan with:

- Project Manager
- Project Sponsor
- Business Owner
- Product Owner where relevant
- Delivery Lead
- Vendor leads
- PMO
- key international stakeholders

AI can help structure the communication model.

The project team must confirm whether the proposed channels, frequencies, escalation paths, and decision rights fit the organisation.

---

# Confidentiality

Project communications may contain sensitive information.

Protect:

- personal information,
- customer information,
- security incidents,
- vendor negotiations,
- confidential financial data,
- contract information,
- sensitive technical architecture.

Use access-controlled channels where appropriate.

---

# Prompt Metadata

```text id="comm-metadata"
Prompt ID: PLAN-006
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Sponsor / PMO / Delivery Lead
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT communication management framework |
