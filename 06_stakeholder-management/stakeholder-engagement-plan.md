# Stakeholder Engagement Plan

**Prompt ID:** STAKE-002 | **Category:** Stakeholder Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Develop a structured stakeholder engagement plan that supports timely decisions, cross-functional collaboration, business readiness, and successful project adoption.

**Use case:** Plan stakeholder involvement during IT project initiation, delivery, organizational change, UAT preparation, deployment, and operational handover.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager experienced in stakeholder
engagement, organizational change, international software delivery,
vendor governance, and cross-functional communication.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]
Target completion: [DATE]

Stakeholder matrix: [PASTE MATRIX OR LIST]
Known concerns: [LIST]
Decision-makers and approval authority: [LIST]
Critical dependencies: [LIST]
Affected business areas: [LIST]
External vendors: [LIST]
Countries / time zones / languages: [IF RELEVANT]
Existing engagement activities: [IF AVAILABLE]
Previous engagement feedback: [IF AVAILABLE]

TASK

Create a practical, outcome-oriented Stakeholder Engagement Plan.

STEP 1 — DEFINE ENGAGEMENT PRIORITIES

1. Identify stakeholder groups requiring active involvement.
2. Define engagement objectives linked to project outcomes:
   - Sponsor alignment and timely decisions
   - Requirements validation and scope clarity
   - Business readiness and user adoption
   - Technical and security approvals
   - Vendor coordination and dependency resolution
   - Operational handover
3. Prioritize engagement based on stakeholder influence,
   decision authority, concerns, change impact, and dependencies.
4. Distinguish confirmed stakeholder needs from assumptions.

STEP 2 — DEVELOP ENGAGEMENT ACTIVITIES

5. Define specific activities for each priority stakeholder:
   - Engagement objective
   - Activity and communication channel
   - Timing / frequency
   - Responsible project role
   - Expected outcome
   - Success measure
6. Match engagement methods to stakeholder needs:
   - Executives: Decisions, business value, material risks
   - Product Owner: Priorities, requirements, acceptance
   - Technical teams: Architecture, interfaces, blockers
   - End users: Demos, feedback, UAT, training
   - Operations: Support readiness and handover
   - Vendors: Delivery commitments and dependencies
7. Ensure activities support two-way engagement,
   not merely one-way reporting.

STEP 3 — MANAGE DECISIONS AND CONCERNS

8. Identify critical decisions, decision owners,
   required inputs, and deadlines.
9. Define how concerns and feedback are:
   - Received
   - Acknowledged
   - Assessed
   - Assigned
   - Resolved or escalated
   - Communicated back to stakeholders
10. Separate vendor delivery governance from
    commercial or contractual governance.
11. Identify engagement risks such as delayed approvals,
    insufficient user participation, or late operational involvement.
12. Recommend escalation where project impact justifies it.

STEP 4 — MEASURE AND ADJUST ENGAGEMENT

13. Define meaningful engagement indicators:
    - Decision turnaround time
    - Overdue stakeholder actions
    - UAT participation
    - Training and readiness progress
    - Unresolved concerns
    - Approval delays
    - Stakeholder feedback
14. Use approved targets where available;
    otherwise recommend measures without inventing thresholds.
15. Identify ineffective, insufficient, or excessive engagement.
16. Recommend adjustments at major milestones,
    organizational changes, or significant escalations.

Adapt engagement to the delivery model:
- Agile / Scrum: Sprint Reviews, demos, Product Owner
  collaboration, and release planning.
- Kanban: Service performance, blocked dependencies,
  flow expectations, and priority policies.
- Predictive: Milestone reviews, formal approvals,
  stage gates, and change control.
- Hybrid: Continuous delivery engagement combined
  with formal project governance.

For international projects, consider language,
time zones, accessibility, and confirmed communication needs.

RULES

- Do not invent stakeholder attitudes or commitments.
- Do not assume communication equals engagement.
- Do not recommend unnecessary meetings.
- Do not assign approval authority without evidence.
- Avoid cultural stereotypes and personal judgments.
- Protect sensitive stakeholder assessments.
- Distinguish proposed activities from agreed commitments.

OUTPUT FORMAT

1. ENGAGEMENT OBJECTIVES

Objective | Stakeholder Group |
Expected Project Outcome | Priority

2. STAKEHOLDER ENGAGEMENT PLAN

Stakeholder | Engagement Objective |
Activity | Method | Frequency |
Proposed Owner | Success Measure

3. DECISION-MAKER ENGAGEMENT

Decision | Decision Authority |
Required Information | Required By |
Escalation if Delayed

4. END-USER AND BUSINESS READINESS

Stakeholder Group | Change Impact |
Engagement Activity | Timing |
Readiness Evidence | Proposed Owner

5. VENDOR AND EXTERNAL PARTNER ENGAGEMENT

Stakeholder | Delivery / Commercial Objective |
Governance Activity | Frequency |
Dependency | Proposed Owner

6. FEEDBACK AND CONCERN MANAGEMENT

Concern / Feedback | Channel |
Proposed Owner | Required Action |
Escalation Trigger | Status

7. ENGAGEMENT EFFECTIVENESS

Indicator | Current Position |
Target / Desired Direction |
Review Frequency | Improvement Action

8. ENGAGEMENT RISKS AND ADJUSTMENTS

Risk / Gap | Project Impact |
Mitigation | Proposed Owner | Priority

9. PLAN REVIEW SCHEDULE

Review Point | Purpose |
Required Evidence | Responsible Role

MANAGEMENT SUMMARY

- Highest-priority engagement activities
- Decisions and dependencies requiring attention
- Main user adoption and readiness concerns
- Engagement effectiveness indicators
- Immediate management actions

Use concise Markdown tables.
Label proposed actions and unconfirmed ownership.
Focus on engagement outcomes rather than meeting volume.
```

---

## 2. Quality Check

Use this independent review to validate the engagement plan before implementation.

```text
QUALITY CHECK

Act as a Senior PMO and Organizational Change Assurance Manager.

Review the Stakeholder Engagement Plan against the
stakeholder matrix and available project information.

Verify:

1. Coverage: Sponsors, business owners, technical teams,
   vendors, operations, and affected users are included
   where relevant.

2. Prioritization: Engagement effort reflects stakeholder
   influence, project impact, decision authority,
   and critical dependencies.

3. Objectives: Each activity supports a defined
   project or stakeholder outcome.

4. Accountability: Activities have appropriate proposed
   owners, timing, and expected results.

5. Decision Management: Critical decisions, responsible
   authorities, deadlines, and escalation paths are visible.

6. User Readiness: Engagement supports requirements,
   testing, training, adoption, and operational transition.

7. Feedback: Concerns can be captured, assigned,
   resolved, and communicated back to stakeholders.

8. Measurement: Effectiveness is assessed using
   meaningful indicators, not meeting counts alone.

9. Efficiency: Communication frequency is appropriate,
   with unnecessary activities eliminated.

10. Governance: Assessments are evidence-based,
    confidential, and consistent with project authority.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Validation Required: [UNCONFIRMED ASSUMPTIONS]
Management Attention: [CRITICAL ENGAGEMENT GAPS]

Do not invent stakeholder commitments,
approval authority, attitudes, or KPI targets.
```

---

## 3. Practical IT Use Case

### CRM Replacement — UAT and Deployment Readiness

**Scenario:** A company is replacing its legacy CRM system. Technical delivery is progressing, but stakeholder involvement is uneven. The Customer Service Director is concerned about operational disruption, Security approval is still required, and frontline employees need preparation before UAT and deployment.

The Project Manager must coordinate targeted engagement to secure decisions, improve business readiness, and reduce deployment risk.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Replacement |
| Phase | UAT Preparation / Pre-Deployment |
| Delivery approach | Hybrid |
| Business objective | Improve customer-service efficiency |
| Key stakeholders | Sponsor, Service Director, Security, Product Owner, End Users, Vendor, Operations |
| Main concern | Business readiness and stakeholder coordination |
| Management objective | Ensure timely approvals, user participation, and operational handover |

### Example Input

```text
Project: CRM System Replacement

Business objective:
Improve customer-service efficiency by replacing
the legacy CRM platform.

Current phase:
UAT Preparation / Pre-Deployment

Delivery approach:
Hybrid

Stakeholders:

Executive Sponsor
- High power / High interest
- Supportive
- Responsible for major governance decisions

Customer Service Director
- High power / High interest
- Neutral
- Concerned about operational disruption

Product Owner
- High power / High interest
- Responsible for functional priorities

Security Lead
- High power / Medium interest
- Attitude unknown
- Production security approval required

Customer Service Agents
- Low power / High interest
- Attitude unknown
- Significant workflow changes expected

CRM Implementation Vendor
- Medium power / High interest
- Supportive
- Responsible for supplier delivery

Operations Lead
- Responsible for post-go-live support

Known concerns:
- UAT participants not fully confirmed
- Limited communication with service agents
- Security review not yet scheduled
- Operations handover planning incomplete

Critical dependencies:
- Business must provide UAT participants
- Security must approve production readiness
- Operations must accept support handover

Existing engagement metrics:
Not available.
```

### Example Output — Stakeholder Engagement Plan

#### 1. Engagement Objectives

| Objective | Stakeholder Group | Expected Outcome | Priority |
|---|---|---|---|
| Maintain governance alignment | Executive Sponsor | Timely management decisions | High |
| Protect business operations | Service Director | Agreed cutover and readiness approach | High |
| Confirm functional readiness | Product Owner | Approved acceptance priorities | High |
| Secure security approval | Security Lead | Completed approval evidence | High |
| Prepare users | Service Agents | Improved UAT and training readiness | High |
| Establish support ownership | Operations Lead | Accepted handover | High |
| Manage supplier dependencies | Vendor | Reliable delivery commitments | High |

#### 2. Stakeholder Engagement Plan

| Stakeholder | Activity | Frequency | Proposed Owner | Success Measure |
|---|---|---|---|---|
| Executive Sponsor | Steering Committee review | Monthly | Project Manager | Decisions within agreed deadlines |
| Service Director | Operational readiness workshop | Biweekly pre-release | Project Manager | Critical concerns addressed |
| Product Owner | Priorities and acceptance review | Weekly | Product Owner / PM | Acceptance decisions confirmed |
| Security Lead | Security readiness checkpoint | Milestone-based | Technical Lead | Approval gaps resolved |
| Service Agents | Demonstrations and UAT sessions | Before release | Change Lead | Participation and feedback captured |
| Vendor | Delivery and dependency review | Weekly | Project Manager | Commitments tracked |
| Operations Lead | Handover readiness review | Biweekly pre-release | Service Transition Lead | Handover criteria satisfied |

Engagement frequencies and proposed owners require agreement with the stakeholders.

#### 3. Decision-Maker Engagement

| Decision | Proposed Authority | Information Required | Deadline |
|---|---|---|---|
| Approve readiness for business testing | Business / Product Owner | UAT scope, testers, entry criteria | Before UAT |
| Confirm operational cutover approach | Authorized Business Owner | Operational impact and contingency plan | Before release |
| Approve security readiness | Security Authority | Security assessment and evidence | Before production |
| Accept operational handover | Operations / Service Owner | Support model, runbooks, known issues | Before hypercare exit |
| Approve material release changes | Project Governance | Schedule, business impact, alternatives | When required |

Formal approval authority must be validated against project governance arrangements.

#### 4. End-User and Business Readiness

| Group | Change Impact | Engagement Activity | Readiness Evidence |
|---|---|---|---|
| Service Agents | New CRM workflows | Demos, training, UAT | Attendance and test feedback |
| Team Leaders | Updated supervision processes | Process workshops | Reviewed operating procedures |
| Customer Service Director | Operational continuity | Cutover readiness review | Agreed operational actions |
| Product Owner | Functionality and acceptance | Requirements / UAT review | Approved acceptance results |
| Operations | Support responsibilities | Handover sessions | Accepted support documentation |

**Engagement priority:** Include service agents before final UAT, rather than relying only on communications immediately before go-live.

#### 5. Vendor and External Partner Engagement

| Activity | Purpose | Frequency | Proposed Owner |
|---|---|---|---|
| Delivery review | Progress, issues, and dependencies | Weekly | Project Manager |
| Technical review | Integration and design decisions | Milestone-based | Solution Architect |
| Commercial review | Contract changes and costs | As required | Commercial Manager |
| Escalation | Resolve material supplier issues | Event-driven | Authorized Project Leadership |

Delivery reviews should track implementation commitments. Commercial changes and contractual disputes should follow the appropriate governance process.

#### 6. Feedback and Concern Management

| Concern | Proposed Channel | Owner | Required Action | Status |
|---|---|---|---|---|
| Operational disruption | Readiness workshop | Project Manager | Agree cutover controls | Open |
| Limited end-user communication | Feedback / demo sessions | Change Lead | Establish communication plan | Open |
| UAT resource availability | Business coordination | Business Owner | Confirm participants | Open |
| Security approval readiness | Security review | Security Lead | Confirm criteria and schedule | Open |
| Support handover gaps | Transition workshop | Operations Lead | Define acceptance requirements | Open |

The statuses are initial proposed tracking states, not evidence of previously registered concerns.

#### 7. Engagement Effectiveness

| Indicator | Current Position | Desired Direction |
|---|---|---|
| Overdue stakeholder decisions | Not provided | Decreasing |
| Confirmed UAT participants | Incomplete | Full coverage of approved UAT needs |
| Open stakeholder concerns | Not provided | Critical concerns resolved |
| Security approval readiness | Review not scheduled | Agreed review path |
| User training readiness | Not provided | Required training completed |
| Operational handover | Planning incomplete | Acceptance criteria achieved |

**Management interpretation:** Success should be assessed through decision timeliness, readiness evidence, and closure of stakeholder concerns—not the number of meetings held.

#### 8. Engagement Risks and Adjustments

| Risk / Gap | Potential Impact | Recommended Action | Priority |
|---|---|---|---|
| Security engaged too late | Deployment approval delay | Schedule security workshop | High |
| UAT resources incomplete | Business testing disruption | Confirm named participants | High |
| Limited agent involvement | Adoption and usability concerns | Introduce early demos and feedback | High |
| Operational handover incomplete | Post-launch support gaps | Define handover checklist | High |
| Delayed business decisions | Schedule uncertainty | Establish decision deadlines | High |
| Unnecessary meetings | Stakeholder capacity pressure | Use targeted reviews and dashboards | Medium |

#### 9. Plan Review Schedule

| Review Point | Purpose | Responsible Role |
|---|---|---|
| Before UAT | Validate participants and acceptance readiness | Project Manager / Product Owner |
| Before deployment | Confirm business, security, and operational readiness | Project Manager |
| Following escalation | Review effectiveness of stakeholder actions | Project Manager |
| During hypercare | Assess user issues and support readiness | Service Manager |
| After organizational changes | Reconfirm engagement and decision ownership | Project Manager |

### Management Decisions

1. **Business readiness:** Confirm UAT participants, operational requirements, and cutover decision owners.
2. **Security:** Arrange formal engagement before the production approval deadline.
3. **User adoption:** Establish regular demonstrations, feedback opportunities, and role-specific training.
4. **Operational transition:** Agree support ownership, knowledge transfer, and handover acceptance requirements.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The plan establishes relevant stakeholder groups, engagement activities, decision dependencies, and effectiveness measures. However, several proposed owners, frequencies, decision authorities, and readiness targets require validation.

**Required corrections:**
- Confirm engagement owners and stakeholder availability.
- Validate formal decision and approval authority.
- Agree UAT participation and training requirements.
- Schedule Security and Operations readiness reviews.
- Establish baseline engagement measures and approved targets.

**Validation Required:** Decision authorities, resource commitments, communication frequency, and engagement success criteria.

**Management Attention:** Business testing resources, Security involvement, end-user readiness, and operational handover.

**Governance:** Supports PMI-aligned stakeholder engagement, communication management, organizational change, leadership, decision-making, and project governance.

Stakeholder engagement should be reviewed throughout project delivery. AI can recommend activities and identify gaps but cannot replace direct stakeholder relationships or authorize commitments. Protect confidential stakeholder assessments, feedback, organizational concerns, and escalation information.
