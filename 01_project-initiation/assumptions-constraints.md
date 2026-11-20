# Assumptions and Constraints Register

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** INIT-001 | **Category:** Project Initiation

---


## 1. Ready-to-Use Prompt

**Purpose:** Identify and validate project assumptions and constraints to support risk and dependency management.

**Use case:** Assess unverified assumptions, resource limitations, and critical dependencies during project initiation, planning, and milestone reviews.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
risk management, dependency management, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target date: [DATE]
Budget: [BUDGET, IF RELEVANT]
Team and stakeholders: [ROLES]
Systems and vendors: [DETAILS]
Known dependencies: [LIST]
Known assumptions: [LIST]
Known constraints: [LIST]

TASK

Create an assumptions and constraints register for the project.

1. Do not invent project facts or present unverified information as confirmed.
2. Distinguish assumptions from confirmed constraints.
3. Assess assumptions affecting schedule, cost, scope, quality,
   security, and operational readiness.
4. Flag assumptions without assigned validation owners.
5. Identify assumptions that should be assessed as project risks.
6. Identify constraints requiring management attention or escalation.
7. Highlight assumptions dependent on external vendors.
8. Identify assumptions dependent on stakeholder availability.
9. Flag contradictions between assumptions and known constraints.
10. Ensure every assumption is specific, testable, and actionable.

OUTPUT FORMAT

TABLE 1 — ASSUMPTIONS REGISTER

ID | Assumption | Category | Impact if Incorrect |
Validation Action | Owner | Validation Date | Status

TABLE 2 — CONSTRAINTS REGISTER

ID | Constraint | Category | Project Impact |
Management Approach | Owner | Review Date

MANAGEMENT SUMMARY

1. Top three assumptions requiring validation
2. Assumptions requiring risk assessment
3. Vendor and stakeholder dependencies
4. Constraints requiring escalation
5. Contradictions and information gaps
6. Recommended management actions and decisions

QUALITY CHECK

Act as a Senior QA Manager and review the generated register.

Verify that:
- All 10 task requirements have been addressed.
- Assumptions are specific, testable, and clearly distinguished
  from confirmed constraints.
- Relevant delivery impacts and dependencies are identified.
- Recommended actions are feasible and have clear ownership.
- Missing information and unsupported conclusions are flagged.

Provide a quality verdict: PASS / REVISE.
List corrections required before stakeholder approval.

Do not invent missing information, owners, dates, or numerical estimates.
Label suggested ownership and deadlines as proposals requiring confirmation.
```

---

## 2. Practical IT Use Case

### CRM Replacement — Planning and Delivery Readiness

**Scenario:** An organization is replacing its CRM system. The Project Manager must validate critical assumptions and identify constraints that could affect the regulatory go-live date.

| Attribute | Project Context |
|---|---|
| Project | CRM Replacement |
| Phase | Planning |
| Delivery approach | Hybrid |
| Target go-live | 1 October 2027 |
| Team | 1 PM, 2 BAs, 5 Developers, 2 QA Engineers, external migration vendor |
| Management decision | Which assumptions require validation, and which constraints could jeopardize delivery? |

### Example Input

```text
Project: CRM Replacement
Business objective: Replace the existing CRM platform
Project phase: Planning
Delivery approach: Hybrid
Target go-live: 1 October 2027

Team:
- 1 Project Manager
- 2 Business Analysts
- 5 Developers
- 2 QA Engineers
- External migration vendor

Known assumptions:
- Customer data can be migrated without major cleansing.
- Business users will be available for UAT in August.
- Vendor API documentation is complete.
- Existing infrastructure supports the new CRM.

Confirmed constraints:
- Fixed regulatory go-live date.
- No additional internal developers available.
- Production deployment only during weekend maintenance windows.
- Security review requires four weeks.
```

### Example Output — Assumptions Register

| ID | Assumption | Impact if Incorrect | Proposed Owner | Status |
|---|---|---|---|---|
| A-01 | Customer data requires no major cleansing | Migration delays and additional costs | Data Lead | To Validate |
| A-02 | Business users are available for UAT in August | Testing and go-live at risk | Business Owner | To Validate |
| A-03 | Vendor API documentation is complete | Integration delays | Integration Lead | To Validate |
| A-04 | Existing infrastructure is sufficient | Additional infrastructure work | Solution Architect | To Validate |

**Validation actions:** Profile source data, confirm UAT resource commitments, request vendor documentation approval, and assess infrastructure capacity.

All owners are proposed and must be confirmed. Validation dates remain open.

### Example Output — Constraints Register

| ID | Constraint | Project Impact | Proposed Owner |
|---|---|---|---|
| C-01 | Fixed regulatory go-live | Limited schedule flexibility | Project Sponsor |
| C-02 | No additional internal developers | Limited recovery capacity | Engineering Manager |
| C-03 | Weekend-only deployment | Restricted release windows | Operations Lead |
| C-04 | Four-week security review | Mandatory scheduling dependency | Security Lead |

### Management Decisions

**1. Validate migration readiness**

Conduct data profiling to confirm whether cleansing is necessary. Assess schedule and budget impacts if
