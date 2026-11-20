# Stakeholder Analysis Matrix

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** STAKE-001 | **Category:** Stakeholder Management

---


## 1. Ready-to-Use Prompt

**Purpose:** Identify and prioritize project stakeholders based on their influence, interests, decision authority, concerns, and engagement needs.

**Use case:** Develop or update a stakeholder analysis during project initiation, delivery, organizational change, or major milestones to improve alignment, manage dependencies, and support timely decisions.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager experienced in
stakeholder engagement, international software delivery,
organizational change, governance, and communication.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Current phase: [PHASE]
Delivery approach: [PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]
Target completion: [DATE]

Project organization: [DETAILS]
Known stakeholders: [LIST]
Decision-makers: [LIST]
External suppliers: [LIST]
Affected business areas: [LIST]
Countries / languages: [IF RELEVANT]
Known concerns and feedback: [DETAILS]
Critical stakeholder dependencies: [LIST]
Previous stakeholder assessments: [IF AVAILABLE]

TASK

Create an evidence-based Stakeholder Analysis Matrix
and a practical engagement plan.

STEP 1 — IDENTIFY AND ASSESS STAKEHOLDERS

1. Identify internal and external stakeholders,
   including sponsors, decision-makers, delivery teams,
   suppliers, operational owners, and affected users.
2. Assess each stakeholder's:
   - Role and project relationship
   - Primary interest and expected outcome
   - Power: High / Medium / Low
   - Interest: High / Medium / Low
   - Attitude: Supportive / Neutral / Resistant / Unknown
   - Decision authority and critical dependencies
   - Key concerns and change impact
3. Classify stakeholders using the Power–Interest Matrix:
   - High Power / High Interest: Manage Closely
   - High Power / Low Interest: Keep Satisfied
   - Low Power / High Interest: Keep Informed
   - Low Power / Low Interest: Monitor
4. Base assessments on documented authority,
   responsibilities, feedback, and observed behavior.
5. Mark unsupported assessments as provisional
   or "Requires validation".

STEP 2 — PRIORITIZE ENGAGEMENT

6. Identify the three stakeholders requiring
   the most active management attention.
7. Consider decision authority, dependency ownership,
   operational impact, influence, and engagement risk.
8. Explain the consequences of insufficient engagement.
9. Recommend specific actions addressing stakeholder
   concerns and project dependencies.
10. Identify missing or insufficiently engaged stakeholders.

STEP 3 — DEVELOP COMMUNICATION AND RISK CONTROLS

11. Define an engagement approach for each stakeholder:
    - Engagement objective
    - Communication method
    - Frequency
    - Required decisions or inputs
    - Responsible project role
12. Identify stakeholder-related delivery risks,
    delayed decisions, unresolved concerns, or
    resource dependencies.
13. Recommend escalation only where justified
    by project impact or governance requirements.
14. Define monitoring indicators such as approval delays,
    reduced participation, or withdrawn commitments.
15. Compare stakeholder attitudes and engagement
    effectiveness over time where evidence exists.
16. Recommend review points during major milestones,
    organizational changes, or significant escalations.

Adapt engagement to the delivery approach:
- Agile / Scrum: Product Owner collaboration,
  Sprint Reviews, user feedback, release decisions.
- Kanban: Service expectations, prioritization,
  blocked dependencies, delivery predictability.
- Predictive: Milestone approvals, formal governance,
  change control, and acceptance.
- Hybrid: Continuous delivery engagement combined
  with executive governance.

For international projects, consider language,
time zones, and confirmed communication preferences.

RULES

- Do not infer stakeholder attitudes without evidence.
- Do not equate constructive challenge with resistance.
- Do not assume organizational seniority equals influence.
- Distinguish formal authority from informal influence.
- Do not invent stakeholder commitments or approvals.
- Avoid personal judgments or cultural stereotypes.
- Protect confidential stakeholder information.

OUTPUT FORMAT

1. STAKEHOLDER ANALYSIS MATRIX

Stakeholder | Role | Primary Interest |
Power | Interest Level | Current Attitude |
Key Concern | Decision Authority

2. POWER–INTEREST PRIORITIZATION

Stakeholder | Power | Interest |
Quadrant | Engagement Priority | Rationale

3. ENGAGEMENT AND COMMUNICATION PLAN

Stakeholder | Engagement Objective |
Recommended Action | Communication Method |
Frequency | Proposed Relationship Owner

4. TOP 3 PRIORITY STAKEHOLDERS

Stakeholder | Why Critical |
Risk if Engagement Fails |
Next Action | Proposed Owner

5. STAKEHOLDER DEPENDENCIES AND RISKS

Stakeholder | Dependency / Concern |
Project Impact | Required By |
Mitigation / Escalation

6. ENGAGEMENT TREND AND WARNING SIGNALS

Stakeholder | Previous Position |
Current Position | Trend |
Evidence | Recommended Response

7. STAKEHOLDER GAPS

Missing / Under-engaged Role |
Potential Impact | Recommended Action |
Priority

MANAGEMENT SUMMARY

- Highest-priority stakeholder relationships
- Critical decisions and dependencies
- Main engagement risks
- Immediate management actions
- Recommended review cadence

Use concise Markdown tables.
Mark unsupported assumptions as "Requires validation".
Prioritize practical engagement over generic communication.
```

---

## 2. Quality Check

Run this independent review before using the matrix for formal stakeholder planning.

```text
QUALITY CHECK

Act as an independent Senior PMO and Stakeholder
Engagement Assurance Manager.

Review the Stakeholder Analysis Matrix and supporting evidence.

Verify:

1. Completeness: Sponsors, decision-makers, technical
   teams, suppliers, operational owners, and affected users
   are appropriately represented.

2. Assessment Quality: Power, interest, influence,
   and decision authority are assessed separately.

3. Evidence: Stakeholder attitudes and concerns
   are supported by available information rather
   than assumptions or subjective judgments.

4. Prioritization: The top three stakeholder
   priorities reflect actual project influence,
   dependencies, and delivery risk.

5. Engagement: Strategies define specific actions,
   communication methods, frequency, and ownership.

6. Dependencies: Critical approvals, resources,
   and stakeholder-controlled deliverables are visible.

7. Risk: Warning signals, escalation needs,
   and unresolved concerns are identified.

8. Consistency: Communication effort is proportional
   to stakeholder needs and project impact.

9. Governance: The analysis respects confidentiality
   and distinguishes proposed actions from commitments.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Validation Required: [UNSUPPORTED ASSESSMENTS]
Management Attention: [CRITICAL ENGAGEMENT GAPS]

Do not invent stakeholder attitudes, influence,
authority, or commitments.
```

---

## 3. Practical IT Use Case

### CRM Replacement — Stakeholder Alignment and Operational Readiness

**Scenario:** A company is replacing its legacy CRM platform. The Executive Sponsor supports the project, but the Customer Service Director is concerned about potential operational disruption. The Security team has not yet been fully engaged, and frontline employees have received limited communication.

The Project Manager must identify stakeholder priorities and establish an engagement plan before UAT and deployment.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM Replacement |
| Phase | Development / UAT Preparation |
| Delivery approach | Hybrid |
| Business objective | Improve customer-service efficiency |
| Main stakeholders | Sponsor, Customer Service, Product Owner, IT, Security, Vendor, End Users |
| Key concern | Operational adoption and readiness |
| Management objective | Secure decisions, reduce resistance risk, and improve engagement |

### Example Input

```text
Project: CRM Replacement

Business objective:
Improve customer-service efficiency and replace
the existing legacy CRM platform.

Current phase:
Development / UAT Preparation

Delivery approach:
Hybrid

Stakeholders:
- Executive Sponsor
- Customer Service Director
- Product Owner
- Solution Architect
- Security Lead
- Data Migration Lead
- CRM Implementation Vendor
- Customer Service Agents
- Operations Lead
- Finance

Known information:
- Executive Sponsor strongly supports the project.
- Customer Service Director has raised concerns
  about operational disruption during rollout.
- Product Owner manages functional priorities.
- Security has not yet been fully engaged.
- Vendor relationship is positive.
- Customer Service Agents received limited
  communication about upcoming changes.
- Operations will support the solution after go-live.

Known dependencies:
- Business must confirm UAT participants.
- Security approval required before deployment.
- Operations must accept support handover.

Stakeholder power and interest assessments:
Not yet validated.
```

### Example Output — Stakeholder Analysis

#### 1. Stakeholder Analysis Matrix

| Stakeholder | Primary Interest | Power | Interest | Attitude | Key Concern |
|---|---|---|---|---|---|
| Executive Sponsor | Business value, delivery success | High* | High* | Supportive | Benefits and timeline |
| Customer Service Director | Operational continuity | High* | High | Unknown | Disruption during rollout |
| Product Owner | Functionality and priorities | High* | High | Unknown | Scope and business value |
| Solution Architect | Technical integrity | Medium* | High* | Unknown | Integration complexity |
| Security Lead | Security readiness | High* | Medium* | Unknown | Compliance and approval |
| Data Migration Lead | Migration quality | Medium* | High* | Unknown | Data integrity |
| CRM Vendor | Delivery performance | Medium* | High* | Supportive* | Delivery commitments |
| Service Agents | Usability and workload | Low* | High | Unknown | Process changes |
| Operations Lead | Support readiness | Medium* | High | Unknown | Handover and support |
| Finance | Budget oversight | Medium* | Medium* | Unknown | Financial control |

*Power, interest, and vendor attitude are provisional. The positive vendor relationship is reported, but it does not alone establish a supportive attitude toward every project decision.*

The Customer Service Director's concerns do not establish resistance.

#### 2. Power–Interest Prioritization

| Stakeholder | Proposed Quadrant | Engagement Approach |
|---|---|---|
| Executive Sponsor | High / High | Manage Closely |
| Customer Service Director | High / High | Manage Closely |
| Product Owner | High / High | Manage Closely |
| Security Lead | High / Medium | Keep Satisfied and involve early |
| Service Agents | Low / High | Keep Informed and involve in testing |
| Operations Lead | Medium / High | Active operational engagement |
| CRM Vendor | Medium / High | Weekly delivery coordination |

**Validation required:** Confirm formal authority and the proposed classifications before finalizing engagement priorities.

#### 3. Engagement and Communication Plan

| Stakeholder | Engagement Objective | Recommended Action | Method / Frequency |
|---|---|---|---|
| Executive Sponsor | Maintain governance alignment | Review delivery exposure and decisions | Monthly Steering Committee |
| Customer Service Director | Protect operational continuity | Review UAT, training, and cutover plans | Biweekly readiness meeting |
| Product Owner | Align functionality and priorities | Resolve requirements and acceptance questions | Weekly working session |
| Security Lead | Secure timely approvals | Review security evidence and outstanding controls | Early workshop and milestones |
| Service Agents | Improve adoption | Provide demos and gather feedback | UAT sessions and demonstrations |
| Operations Lead | Confirm service readiness | Review support model and handover evidence | Biweekly transition review |
| CRM Vendor | Maintain delivery accountability | Review commitments, dependencies, and risks | Weekly supplier meeting |
| Finance | Maintain cost visibility | Review material budget changes | Monthly or event-driven |

All meeting frequencies are proposed and subject to stakeholder agreement.

#### 4. Top 3 Priority Stakeholders

| Stakeholder | Why Critical | Risk if Engagement Fails | Next Action |
|---|---|---|---|
| Customer Service Director | Controls or influences operational readiness | Cutover disruption or weak business preparation | Arrange readiness workshop |
| Security Lead | Required for deployment approval | Late security issues could delay release | Confirm approval criteria and schedule |
| Product Owner | Owns functional priorities | Unresolved requirements may affect UAT | Validate acceptance priorities |

The Executive Sponsor remains a key governance stakeholder. The three above are prioritized because of the immediate, reported readiness dependencies.

#### 5. Stakeholder Dependencies and Risks

| Stakeholder | Dependency | Potential Impact | Proposed Response |
|---|---|---|---|
| Customer Service Director / Business | Confirm UAT participants | UAT resource shortages | Establish resource commitments |
| Security Lead | Security approval | Deployment delay | Agree review dates and evidence |
| Operations Lead | Support acceptance | Incomplete handover | Prepare operational readiness checklist |
| Product Owner | Functional decisions | Requirements or testing delays | Track decision deadlines |
| CRM Vendor | Supplier deliverables | Schedule and quality risk | Monitor supplier commitments |

#### 6. Engagement Trend and Warning Signals

| Stakeholder | Current Evidence | Trend | Monitoring Focus |
|---|---|---|---|
| Executive Sponsor | Strong project support reported | Unknown | Timely governance decisions |
| Customer Service Director | Operational concern raised | Unknown | Engagement and readiness decisions |
| Security Lead | Limited engagement | Unknown | Review participation and approvals |
| Service Agents | Limited communication | Unknown | Feedback, participation, training readiness |
| Vendor | Positive relationship reported | Unknown | Delivery commitments and responsiveness |

Previous stakeholder assessments are unavailable; therefore, improvement or deterioration cannot be established.

#### 7. Stakeholder Gaps

| Gap | Potential Impact | Recommended Action | Priority |
|---|---|---|---|
| Security not fully engaged | Late approval risk | Schedule security review | High |
| Limited end-user communication | Poor adoption readiness | Introduce demos and feedback sessions | High |
| UAT resource commitments unconfirmed | Testing disruption | Confirm named participants | High |
| Operations handover not yet evidenced | Support readiness gap | Establish acceptance checklist | High |
| Stakeholder authority unclear | Delayed decisions | Validate decision and escalation roles | Medium |

### Management Decisions

1. **Operational readiness:** Engage the Customer Service Director in UAT, training, and cutover decisions.
2. **Security governance:** Confirm approval criteria, responsible reviewers, and required evidence before deployment.
3. **User adoption:** Include customer-service agents in demonstrations, testing, and structured feedback.
4. **Stakeholder accountability:** Confirm decision rights, dependency ownership, and appropriate engagement frequency.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The analysis identifies the main stakeholder groups, their potential influence, readiness dependencies, and targeted engagement actions. However, power levels, stakeholder attitudes, decision authority, and communication arrangements remain partially unvalidated.

**Required corrections:**
- Confirm stakeholder authority and influence.
- Validate current attitudes through direct engagement.
- Agree communication frequency and relationship ownership.
- Confirm UAT resource commitments.
- Establish Security and Operations approval responsibilities.

**Validation Required:** Provisional power–interest assessments, vendor attitude, and stakeholder decision rights.

**Management Attention:** Security engagement, operational readiness, and end-user communication.

**Governance:** Supports PMI-aligned stakeholder identification, engagement planning, communication management, organizational change, risk management, and project governance.

Stakeholder analysis must be updated as project conditions change. AI may help structure engagement strategies but should not make unsupported judgments about individuals. Protect confidential stakeholder assessments, internal relationships, sensitive feedback, and organizational information.
