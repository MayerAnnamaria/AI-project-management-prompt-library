# RACI Matrix and Governance Review

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** PLAN-003 | **Category:** Project Planning

---


## 1. Ready-to-Use Prompt

**Purpose:** Define responsibilities and decision authority to improve accountability, cross-team coordination, and project governance.

**Use case:** Clarify ownership and approval responsibilities during project planning, software delivery, release preparation, or changes to team structure and governance.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
responsibility assignment, stakeholder management, cross-functional
coordination, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Project roles: [LIST]
Business and technical teams: [LIST]
External vendors: [IF RELEVANT]
Governance bodies: [LIST]
Key activities: [LIST]
Key decisions: [LIST]
Cross-team dependencies: [LIST]
Known ownership concerns: [LIST]
Existing approval authority: [IF KNOWN]
Existing RACI: [PASTE IF AVAILABLE]

TASK

Create a RACI matrix and perform a governance review.

STEP 1 — RESPONSIBILITY ASSIGNMENT

1. Identify activities, deliverables, and decisions requiring
   clear responsibility and accountability.
2. Assign R (Responsible), A (Accountable), C (Consulted),
   and I (Informed) based on available governance information.
3. Ensure each critical activity has a Responsible role and
   normally one Accountable owner.
4. Distinguish delivery execution from approval authority.
5. Separate business, technical, security, operations,
   and vendor responsibilities.
6. Identify cross-team dependencies and escalation ownership.
7. Align responsibilities with the stated delivery approach
   without overriding established framework accountabilities.

STEP 2 — GOVERNANCE REVIEW

8. Identify activities with missing or multiple Accountable owners.
9. Flag activities without a Responsible role.
10. Identify overloaded roles and excessive consultation.
11. Detect unclear business, IT, vendor, or cross-team ownership.
12. Flag decision-right conflicts and missing escalation authority.
13. Identify key stakeholders excluded from necessary consultation.
14. Recommend corrections to responsibilities and governance gaps.
15. Identify assignments requiring stakeholder confirmation.

Do not invent organisational authority or approved responsibilities.
Label suggested RACI assignments as proposed until validated.
Prioritize clear accountability over unnecessary role assignments.

OUTPUT FORMAT

TABLE 1 — RACI MATRIX

Activity / Decision | [ROLE 1] | [ROLE 2] | [ROLE 3] | ...

Use:
R = Responsible
A = Accountable
C = Consulted
I = Informed
A/R = Both Accountable and Responsible
– = No assigned involvement

TABLE 2 — GOVERNANCE GAP REVIEW

Issue | Affected Activity | Governance Risk |
Recommended Correction | Decision Required | Priority

TABLE 3 — DECISION RIGHTS

Decision | Recommends | Approves | Executes |
Consulted | Escalation Authority

TABLE 4 — CROSS-TEAM DEPENDENCIES

Dependency | Provider Team | Receiving Team |
Accountable Owner | Required By | Escalation Owner

MANAGEMENT SUMMARY

1. Critical accountability and ownership gaps
2. Conflicting or missing decision authority
3. Overloaded roles and unnecessary consultation
4. Cross-team and vendor dependencies
5. Recommended governance corrections and approvals

Use concise Markdown tables.
Mark unknown authority as "Not yet defined".
Clearly distinguish proposed assignments from confirmed roles.
```

---

## 2. Quality Check

Apply this control after generating the RACI matrix and governance review.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the RACI matrix.

Verify:

1. Completeness: Critical activities, decisions, and teams
   are represented.
2. Accountability: Each critical activity normally has one
   Accountable owner and at least one Responsible role.
3. Consistency: Assignments align with confirmed authority,
   delivery responsibilities, and governance structures.
4. Role Clarity: Business, technical, security, operational,
   and vendor ownership are clearly distinguished.
5. Efficiency: Excessive consultation, overloaded roles,
   and unnecessary approval layers are flagged.
6. Governance: Decision rights, dependencies, and escalation
   responsibilities are defined or marked for confirmation.
7. Actionability: Governance gaps have specific,
   prioritized corrective actions.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]

Do not invent decision authority, role assignments, or approvals.
Flag responsibilities requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development — Testing and Release Governance

**Scenario:** A software development team is preparing a new release. Developers, QA engineers, the Product Owner, and Operations have overlapping responsibilities for defect resolution, acceptance testing, and deployment.

The Project Manager must clarify responsibilities and decision authority to prevent delayed approvals, duplicated work, and unresolved release blockers.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Testing / Release Preparation |
| Delivery approach | Scrum |
| Team | Project Manager, Product Owner, Development Lead, QA Lead, Security Lead, Operations Lead |
| Key activities | Development, testing, defect management, UAT, release readiness, deployment |
| Current challenge | Unclear ownership of defect priorities, approvals, and deployment |
| Management decision | Confirm responsibilities and approval authority before release |

### Example Input

```text
Project: Web Application Reporting Enhancement

Business objective:
Deliver enhanced reporting functionality to business users.

Project phase: Testing / Release Preparation
Delivery approach: Scrum

Roles:
- Project Manager (PM)
- Product Owner (PO)
- Development Lead (DEV)
- QA Lead (QA)
- Security Lead (SEC)
- Operations Lead (OPS)

Key activities:
- Requirements clarification
- Technical implementation
- Defect triage
- Regression testing
- UAT coordination
- UAT acceptance
- Security review
- Release readiness assessment
- Production release approval
- Production deployment
- Post-release validation

Known ownership concerns:
- Developers and QA disagree on defect prioritization.
- UAT acceptance authority is unclear.
- Production deployment responsibilities are not documented.
- Release approval authority is not defined.
- Security review ownership needs confirmation.

Existing decision authority:
Not yet documented.
```

### Example Output — RACI Matrix

The following assignments illustrate a proposed responsibility model. They must be reviewed against the organization's governance structure.

**Role abbreviations:** PM = Project Manager; PO = Product Owner; DEV = Development Lead; QA = QA Lead; SEC = Security Lead; OPS = Operations Lead.

| Activity / Decision | PM | PO | DEV | QA | SEC | OPS |
|---|---|---|---|---|---|---|
| Requirements clarification | I | A | C | C | – | – |
| Technical implementation | I | C | A/R | C | C | – |
| Defect triage | C | A | R | R | C | – |
| Regression testing | I | C | C | A/R | – | – |
| UAT coordination | A | C | I | R | – | – |
| UAT acceptance | C | A | I | R | – | – |
| Security review | I | I | C | C | A/R | C |
| Release readiness assessment | A | C | R | R | C | C |
| Production release approval | R | C | C | C | C | C |
| Production deployment | I | I | R | C | C | A |
| Post-release validation | I | C | R | R | C | A |

**Governance exception:** Production release approval has no confirmed Accountable owner. An authorized release decision-maker must be identified before the matrix can be approved.

The proposed role assignments are illustrative and do not establish formal organizational authority. For Scrum teams, Product Owner and Developer accountabilities must remain consistent with the Scrum framework.

### Example Output — Governance Gap Review

| Issue | Affected Activity | Governance Risk | Recommended Correction | Decision Required | Priority |
|---|---|---|---|---|---|
| Missing approval authority | Production release approval | Unauthorized or delayed release | Identify Accountable approver | Confirm release authority | High |
| Unclear business acceptance | UAT acceptance | Acceptance disputes | Validate PO or business approval authority | Confirm acceptance owner | High |
| Defect prioritization conflict | Defect triage | Delayed resolution | Define severity and priority decision rights | Agree triage policy | High |
| Unclear deployment responsibility | Production deployment | Deployment delays | Confirm deployment owner and execution responsibilities | Approve operational roles | High |
| Security ownership unconfirmed | Security review | Release compliance risk | Confirm security approval responsibilities | Validate security authority | High |

### Example Output — Decision Rights

| Decision | Recommends | Approves | Executes | Consulted | Escalation Authority |
|---|---|---|---|---|---|
| Defect prioritization | QA / DEV | PO (proposed) | DEV / QA | PM | TBD |
| UAT acceptance | QA / Business Users | PO (proposed) | Business / QA | PM | TBD |
| Security clearance | Security Lead | Authorized Security Authority (TBD) | Security / DEV | PM | TBD |
| Release approval | PM | TBD | Delivery / Operations | PO, QA, Security | TBD |
| Production rollback | Operations / DEV | TBD | Operations / DEV | PM, Security | TBD |

*All decision rights require confirmation. The table does not imply that any approval has been granted.*

### Example Output — Cross-Team Dependencies

| Dependency | Provider Team | Receiving Team | Accountable Owner | Required By | Escalation Owner |
|---|---|---|---|---|---|
| Defect fixes | Development | QA | DEV (proposed) | Before regression completion | PM (proposed) |
| Test completion evidence | QA | Release decision-maker | QA (proposed) | Before release approval | PM (proposed) |
| Security clearance | Security | Release decision-maker | SEC (proposed) | Before release approval | TBD |
| Deployment readiness | Operations | Delivery Team | OPS (proposed) | Before deployment | PM (proposed) |
| UAT acceptance | Business / PO | Release decision-maker | PO (proposed) | Before release approval | TBD |

### Management Decisions

**1. Confirm release authority**

Identify who has final accountability for production release approval and establish the required evidence and escalation path.

**2. Clarify defect management**

Agree on severity classification, prioritization authority, defect ownership, and escalation responsibilities.

**3. Validate UAT and security approval**

Confirm who can formally accept business functionality and authorize security readiness.

**4. Establish deployment accountability**

Define deployment execution, operational ownership, post-release validation, and rollback decision rights.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The proposed RACI covers the main testing and release activities, but several decision rights remain unconfirmed. Production release approval has no Accountable owner, and the authority for UAT, security acceptance, and rollback requires validation.

**Required corrections:**
- Assign and confirm the authorized release approver.
- Validate Product Owner and business acceptance responsibilities.
- Confirm defect prioritization and escalation authority.
- Establish deployment and rollback decision rights.
- Obtain stakeholder agreement on the final RACI.

**Approval blockers:** Missing production release accountability and unconfirmed critical approval authority.

**Governance:** This prompt supports relevant PMI-aligned practices in responsibility assignment, stakeholder management, resource coordination, decision authority, and project governance.

The RACI matrix is a responsibility-planning artifact, not evidence of formal authorization. Accountable stakeholders must validate assignments before implementation. Use organizational roles rather than personal names where practical, and protect confidential governance and security information.
