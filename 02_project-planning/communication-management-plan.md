# Communication Management Plan

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** PLAN-006 | **Category:** Project Planning

---


## 1. Ready-to-Use Prompt

**Purpose:** Establish clear, timely, and accountable project communication to improve stakeholder alignment, delivery coordination, and decision-making.

**Use case:** Define reporting responsibilities, meeting cadence, and escalation procedures when coordinating software development teams, managing delivery blockers, or preparing releases.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
stakeholder communication, cross-functional coordination,
risk management, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Project duration: [DURATION]
Primary language: [LANGUAGE]
Countries / time zones: [IF RELEVANT]
Stakeholders and teams: [ROLES]
External vendors: [IF RELEVANT]
Governance bodies: [LIST]
Communication challenges: [LIST]
Communication tools: [JIRA / CONFLUENCE / TEAMS / EMAIL / OTHER]
Document repository: [LOCATION]

TASK

Create a Communication Management Plan for the project.

1. Define 3–5 communication objectives aligned with delivery needs.
2. Identify stakeholder information requirements, channels,
   formats, frequency, and accountable owners.
3. Differentiate executive, business, technical, delivery-team,
   and vendor communication requirements.
4. Define governance reporting for status, budget, risks,
   issues, scope changes, dependencies, and decisions.
5. Establish operational coordination and information-sharing rules.
6. Define language, time-zone, and response protocols where relevant.
7. Establish escalation levels, triggers, recipients,
   response deadlines, and decision authority.
8. Define meeting cadence, purpose, participants,
   expected outputs, and ownership.
9. Establish document ownership, version control,
   approval, distribution, and confidentiality requirements.
10. Identify authoritative information sources to prevent
    inconsistent or duplicated project records.
11. Assess communication risks and recommend mitigation actions.
12. Define measurable indicators of communication effectiveness.

Adapt communication practices to the delivery approach.
Avoid unnecessary meetings and duplicated reporting.
Ensure material decisions and commitments are documented.

OUTPUT FORMAT

1. COMMUNICATION OBJECTIVES
   Objective | Expected Outcome | Success Measure

2. STAKEHOLDER COMMUNICATION MATRIX
   Stakeholder | Information Need | Channel |
   Frequency | Owner | Format

3. GOVERNANCE COMMUNICATION
   Topic | Audience | Cadence | Owner | Evidence

4. TEAM COMMUNICATION
   Activity | Participants | Purpose | Output | Owner

5. LANGUAGE & TIME-ZONE PROTOCOL
   Language | Time-Zone Reference | Collaboration Window |
   Response Expectations

6. ESCALATION PATHWAY
   Trigger | Level | Owner | Recipient |
   Response Timeframe | Decision Required

7. MEETING CADENCE
   Meeting | Purpose | Frequency | Participants |
   Owner | Required Output

8. DOCUMENT CONTROL & DISTRIBUTION
   Information | Authoritative Source | Owner |
   Access | Approval / Version Control

9. COMMUNICATION RISKS
   Risk | Delivery Impact | Mitigation | Owner

10. COMMUNICATION EFFECTIVENESS
    KPI | Measurement Method | Target | Review Frequency

MANAGEMENT SUMMARY

- Critical communication gaps and dependencies
- Escalation and decision-making priorities
- Recommended communication improvements
- Required management approvals

Use concise Markdown tables.
Do not invent responsibilities, response times, or KPIs.
Mark proposed arrangements as requiring confirmation.
```

---

## 2. Quality Check

Apply this control after generating the Communication Management Plan.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the communication plan.

Verify:

1. Completeness: All 10 required components are addressed.
2. Relevance: Information matches stakeholder and decision needs.
3. Accountability: Communication owners and escalation paths are clear.
4. Feasibility: Meeting schedules, channels, and response
   expectations are practical.
5. Governance: Material decisions, approvals, and documents
   are properly recorded and controlled.
6. Risk: Communication delays, dependencies, and confidentiality
   concerns are identified.
7. Measurement: Communication KPIs are measurable and relevant.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent missing information or approval authority.
Flag arrangements requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development Project — Release Communication

**Scenario:** A software development team is preparing a new application release. Developers, QA engineers, and business stakeholders use Jira and Microsoft Teams, but critical defects are escalated late, acceptance criteria are occasionally unclear, and stakeholders receive inconsistent release-status updates.

The Project Manager must establish communication responsibilities, reporting procedures, and escalation rules to improve release coordination.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Enhancement |
| Phase | Development / Testing |
| Delivery approach | Scrum |
| Release target | End of Sprint 6 |
| Team | 4 Developers, 2 QA Engineers, 1 Product Owner, 1 Project Manager |
| Tools | Jira, Confluence, Microsoft Teams |
| Current challenge | Late defect escalation, unclear decisions, inconsistent status reporting |
| Management decision | Establish communication and escalation procedures before release |

### Example Input

```text
Project: Web Application Enhancement

Business objective:
Deliver new reporting functionality to business users.

Project phase: Development / Testing
Delivery approach: Scrum
Release target: End of Sprint 6

Team:
- 1 Project Manager
- 1 Product Owner
- 4 Developers
- 2 QA Engineers

Tools:
Jira, Confluence, Microsoft Teams

Known communication challenges:
- Critical defects are sometimes escalated late.
- Developers receive unclear acceptance criteria.
- Business stakeholders request status updates individually.
- Some decisions are made verbally without documentation.
- Release readiness information is distributed across tools.
- Responsibilities for escalation are not clearly defined.
```

### Example Output — Communication Management Plan

#### 1. Communication Objectives

| Objective | Expected Outcome | Success Measure |
|---|---|---|
| Improve defect escalation | Earlier management visibility of release blockers | Escalation response time |
| Clarify requirements | Fewer unresolved acceptance questions | Open clarification count |
| Standardize status reporting | Consistent stakeholder information | Reporting completeness |
| Improve decision traceability | Documented project decisions | Overdue decision count |

*Performance targets require agreement.*

#### 2. Stakeholder Communication Matrix

| Stakeholder | Information Need | Channel | Frequency | Proposed Owner | Format |
|---|---|---|---|---|---|
| Developers | Priorities, requirements, blockers | Jira / Teams | Daily | Development Lead | Task board |
| QA Engineers | Build readiness, defects, fixes | Jira | Daily | QA Lead | Defect report |
| Product Owner | Scope, acceptance, priorities | Jira / Teams | Ongoing | Project Manager | Backlog and decision log |
| Business Stakeholders | Progress, delivery impact, readiness | Teams / Email | Weekly (proposed) | Project Manager | Status report |
| Project Sponsor | Major risks and decisions | Email / Review | Milestone-based | Project Manager | Executive summary |

#### 3. Governance Communication

| Topic | Audience | Cadence | Proposed Owner | Evidence |
|---|---|---|---|---|
| Release readiness | Sponsor / Product Owner | Before release | Project Manager | Readiness assessment |
| Critical defects | Delivery leadership | Event-driven | QA Lead | Jira defect record |
| Scope changes | Product Owner / PM | As required | Project Manager | Change decision record |
| Project status | Business stakeholders | Weekly (proposed) | Project Manager | Status report |

#### 4. Team Communication

| Activity | Participants | Purpose | Expected Output | Proposed Owner |
|---|---|---|---|---|
| Daily coordination | Scrum Developers | Inspect progress and adapt plan | Updated Sprint Backlog | Developers |
| Backlog clarification | Product Owner, Developers, QA | Resolve requirement ambiguity | Clarified backlog items | Product Owner |
| Defect triage | Developers, QA, Product Owner | Prioritize and assign defects | Prioritized defect list | QA Lead |
| Release coordination | PM, Product Owner, Developers, QA | Assess release readiness | Readiness findings | Project Manager |

Use existing Scrum events wherever possible. Do not create parallel meetings unnecessarily.

#### 5. Language & Time-Zone Protocol

| Item | Proposed Protocol |
|---|---|
| Working language | To be confirmed |
| Meeting language | Agreed project language |
| Time-zone reference | Team-local time zone, if co-located |
| Documentation | Consistent agreed language |
| Response expectations | Based on issue priority and agreed working hours |

No distributed-team arrangements are specified in the project input. International communication procedures should be added only if required.

#### 6. Escalation Pathway

| Trigger | Level | Proposed Owner | Recipient | Response Timeframe | Decision Required |
|---|---|---|---|---|---|
| Routine technical blocker | Team | Developer | Development Lead | TBD | Technical resolution |
| Unclear acceptance criteria | Product | Developer / QA | Product Owner | TBD | Requirement clarification |
| Critical defect affecting release | Project | QA Lead | Project Manager / Product Owner | TBD | Remediation priority |
| Release milestone at risk | Management | Project Manager | Sponsor / authorized approver | TBD | Recovery or release decision |
| Security-critical defect | Specialist | QA / Security Lead | Security authority | Per security policy | Risk treatment |

**Reusable escalation message:**

```text
ISSUE: [DESCRIPTION]
IMPACT: [BUSINESS / DELIVERY IMPACT]
STATUS: [CURRENT STATUS]
OPTIONS: [AVAILABLE ACTIONS]
RECOMMENDATION: [PROPOSED RESPONSE]
DECISION OWNER: [ROLE]
DECISION DEADLINE: [DATE / TIME]
```

Response deadlines and decision rights require approval.

#### 7. Meeting Cadence

| Meeting | Purpose | Frequency | Participants | Proposed Owner | Required Output |
|---|---|---|---|---|---|
| Daily Scrum | Inspect progress toward Sprint Goal | Daily | Developers | Developers | Adapted plan |
| Sprint Planning | Define Sprint Goal and planned work | Each sprint | Scrum Team | Scrum Team | Sprint Backlog |
| Sprint Review | Inspect Increment and progress | Each sprint | Scrum Team / Stakeholders | Scrum Team | Feedback and backlog adaptations |
| Sprint Retrospective | Improve team effectiveness | Each sprint | Scrum Team | Scrum Team | Improvement actions |
| Defect triage | Address release-impacting defects | As required | Developers, QA, PO | QA Lead | Prioritized defects |
| Release review | Confirm readiness and blockers | Before release | PM, PO, QA, Development | Project Manager | Release recommendation |

Meeting ownership and cadence must align with Scrum accountabilities and existing team practices.

#### 8. Document Control & Distribution

| Information | Proposed Source | Owner | Access / Control |
|---|---|---|---|
| Sprint tasks and backlog | Jira | Product Owner / Developers | Authorized project team |
| Defect records | Jira | QA Lead | Project team |
| Project documentation | Confluence | Project Manager | Version-controlled |
| Requirements and acceptance criteria | Jira / Confluence | Product Owner | Controlled updates |
| Release readiness | Confluence / approved repository | Project Manager | Authorized stakeholders |
| Management decisions | Decision log | Project Manager | Traceable approvals |

Confirm authoritative systems and access permissions with the organization.

#### 9. Communication Risks

| Risk | Delivery Impact | Mitigation | Proposed Owner |
|---|---|---|---|
| Late defect escalation | Delayed release decisions | Establish escalation triggers | QA Lead |
| Unclear acceptance criteria | Rework and testing delays | Introduce backlog clarification | Product Owner |
| Inconsistent status reporting | Conflicting stakeholder expectations | Establish standard status report | Project Manager |
| Undocumented decisions | Repeated discussions and scope disputes | Maintain decision log | Project Manager |
| Fragmented release information | Incomplete readiness assessment | Establish single readiness record | Project Manager |

#### 10. Communication Effectiveness

| KPI | Measurement Method | Target | Review Frequency |
|---|---|---|---|
| Critical defect escalation time | Time from classification to escalation | TBD | Weekly (proposed) |
| Overdue decisions | Decisions past agreed deadline | TBD | Weekly (proposed) |
| Requirement clarification age | Time open questions remain unresolved | TBD | Sprint review |
| Action closure rate | Actions closed by due date / actions due | TBD | Weekly (proposed) |
| Release reporting completeness | Required readiness items reported | TBD | Before release |

### Management Decisions

1. **Defect escalation:** Agree on defect severity criteria, escalation triggers, and response responsibilities.
2. **Requirement clarity:** Establish a consistent process for clarifying and approving acceptance criteria before implementation and testing.
3. **Release communication:** Standardize release readiness reporting and identify the accountable release decision-maker.
4. **Document control:** Confirm Jira and Confluence as authoritative project information sources, subject to organizational approval.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The plan addresses the main communication challenges and provides a structured approach for development, QA, stakeholder reporting, and release coordination. However, escalation response times, authority, and KPI targets remain unconfirmed.

**Required corrections:**
- Approve critical defect escalation thresholds and response times.
- Confirm accountable communication and decision owners.
- Agree on stakeholder reporting frequency.
- Validate release readiness documentation and approval procedures.
- Define measurable communication performance targets.

**Approval blockers:** Undefined critical escalation timeframes and unconfirmed release decision authority.

**Governance:** This prompt supports relevant PMI-aligned practices in communication management, stakeholder engagement, issue escalation, quality assurance, and project governance.

The Communication Management Plan requires stakeholder validation before implementation. Protect confidential project, personal, commercial, and security-sensitive information through authorized systems.
