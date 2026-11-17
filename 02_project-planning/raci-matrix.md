# RACI Matrix and Governance Review

## Purpose

Use this prompt to create and review a Responsibility Assignment Matrix for an IT project.

A RACI matrix clarifies who is:

**R — Responsible**  
Performs or coordinates the work.

**A — Accountable**  
Owns the final outcome or decision.

**C — Consulted**  
Provides input before the activity or decision is completed.

**I — Informed**  
Receives relevant information after or during the activity.

The objective is not simply to fill every cell.

The objective is to make **ownership and decision rights explicit**.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery

**Project type:**  
Software implementation / Digital transformation / Data / Infrastructure / ERP / Product delivery / Multi-vendor initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Business Analyst

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At project setup and after major team, scope, or governance changes

---

# Prompt 1 — Create the RACI Matrix

```text id="raci-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, cross-functional coordination, stakeholder
management, governance, and accountability design.

TASK

Create a RACI matrix for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Project roles:
[LIST ROLES]

External vendors:
[LIST]

Governance bodies:
[LIST]

Major workstreams:
[LIST]

Key activities:
[LIST]

Key decisions:
[LIST]

Known ownership concerns:
[LIST]

OUTPUT FORMAT

Create a RACI matrix:

Activity / Decision | Role 1 | Role 2 | Role 3 | Role 4 | ...

Use:

R = Responsible
A = Accountable
C = Consulted
I = Informed

Then provide:

1. Accountability gaps
2. Duplicate accountability
3. Activities without a Responsible owner
4. Overloaded roles
5. Decision-right conflicts
6. Cross-team ownership gaps
7. Recommended governance improvements
```

---

# Core RACI Rules

Use the following rules when generating the matrix.

## Rule 1 — One Accountable Owner

Each activity or decision should normally have **one clear Accountable owner**.

Avoid:

```text id="raci-bad-a"
Production Release Approval

Project Manager = A
Product Owner = A
IT Director = A
```

This creates unclear final authority.

Prefer:

```text id="raci-good-a"
Production Release Approval

IT Director = A
Project Manager = R
Product Owner = C
Security Lead = C
Operations Lead = C
```

The exact ownership must match the organisation's governance model.

---

# Rule 2 — Every Activity Needs Ownership

Avoid rows with:

```text id="raci-no-owner"
C | C | I | I | C
```

No one owns the actual work.

Important activities should normally have at least:

- one Responsible role,
- one Accountable role.

---

# Rule 3 — Avoid Excessive Consultation

A matrix such as:

```text id="raci-too-many-c"
R | A | C | C | C | C | C | C
```

may indicate unnecessarily complex decision-making.

Ask:

> Do all these stakeholders genuinely need to be consulted before the decision?

Too many mandatory consultations can create delivery delays.

---

# Rule 4 — Accountability Is Not the Same as Seniority

Do not automatically assign the most senior person as Accountable.

Accountability should follow:

- decision authority,
- ownership of the outcome,
- organisational mandate,
- governance rules.

---

# Rule 5 — Separate Work From Decisions

Where useful, distinguish between:

```text id="raci-work-decision"
Prepare release package
Approve production release
Execute deployment
Confirm post-release validation
```

These activities may have different Accountable owners.

---

# Typical IT Project Activities

Use only those relevant to the project.

```text id="raci-it-activities"
Project charter approval
Business requirements approval
Product / solution scope approval
Architecture approval
Backlog ownership
Technical design
Security review
Data migration
Environment readiness
Development / configuration
Integration development
System Integration Testing
UAT preparation
UAT execution
Defect triage
Release readiness
Go-live approval
Production deployment
Operational handover
Risk acceptance
Change approval
Vendor management
Budget approval
Executive reporting
Project close-out
```

---

# Delivery-Approach Considerations

## Agile / Scrum

Possible roles include:

- Product Owner
- Scrum Master
- Project Manager
- Developers
- QA
- Solution Architect
- Business Owner
- Security
- Operations

Be careful not to use RACI to override established Agile accountabilities.

For example, Product Owner responsibilities should not be redistributed simply because a RACI matrix is being created.

---

## Kanban

RACI may clarify ownership for:

- service ownership,
- replenishment decisions,
- workflow policies,
- blocked-item escalation,
- risk decisions,
- release decisions,
- operational support.

Flow ownership should remain clear without introducing unnecessary approval layers.

---

## Predictive

RACI may be closely aligned with:

- work packages,
- milestone approvals,
- change control,
- scope approval,
- formal governance.

---

## Hybrid

RACI is particularly useful where traditional governance interacts with Agile or flow-based delivery.

Example:

```text id="raci-hybrid"
Product backlog ownership → Product Owner

Technical implementation → Delivery Team

Project-level dependency coordination → Project Manager

Architecture approval → Architecture Authority

Budget approval → Sponsor

Production release approval → Defined governance authority
```

---

# Prompt 2 — RACI Governance Audit

After creating the matrix, run a separate governance review.

```text id="raci-audit"
ROLE

You are a senior PMO and project-governance specialist reviewing
an IT project's responsibility assignment model.

TASK

Audit the RACI matrix below for governance weaknesses.

RACI MATRIX

[PASTE MATRIX HERE]

Identify:

1. Rows with no Accountable owner
2. Rows with multiple Accountable owners
3. Rows with no Responsible owner
4. Roles carrying excessive accountability
5. Activities with excessive consultation
6. Activities where important stakeholders appear excluded
7. Decision rights that conflict with stated governance
8. Vendor / internal-team ownership ambiguity
9. Business / IT ownership ambiguity
10. Activities where escalation authority is unclear

OUTPUT FORMAT

Governance Issue
Affected Activity
Why It Matters
Risk
Recommended Correction
Decision Required
```

---

# Example Input

```text id="raci-example-input"
Project:
CRM Replacement

Delivery Approach:
Hybrid

Roles:
Sponsor
Project Manager
Product Owner
Business Analyst
Solution Architect
Development Lead
QA Lead
Security Lead
Operations Lead
Implementation Vendor

Key Activities:
Project charter approval
Requirements approval
Solution design
CRM configuration
Integration development
Data migration
SIT
UAT
Security approval
Release readiness
Go-live approval
Production deployment
Operational handover
```

---

# Example Matrix Excerpt

| Activity | Sponsor | PM | PO | Architect | Dev Lead | QA | Security | Operations |
|---|---|---|---|---|---|---|---|---|
| Project Charter Approval | A | R | C | I | I | I | I | I |
| Requirements Approval | I | C | A | C | C | C | I | C |
| Solution Design | I | C | C | A | R | C | C | C |
| SIT | I | C | C | C | R | A | I | I |
| Security Approval | I | I | I | C | C | I | A/R | C |
| Go-Live Approval | A | R | C | C | C | C | C | C |
| Production Deployment | I | C | I | C | R | C | C | A |

This example is illustrative only.

Actual accountabilities must follow the organisation's governance model.

---

# Decision-Rights Review

RACI alone may not be sufficient for important decisions.

For key governance decisions, also create:

| Decision | Recommends | Approves | Executes | Must Be Consulted | Escalation Authority |
|---|---|---|---|---|---|

Useful decisions may include:

- scope change,
- budget increase,
- release approval,
- risk acceptance,
- vendor escalation,
- milestone re-baseline,
- production rollback.

This makes decision authority more explicit than RACI alone.

---

# Cross-Team Dependency Review

For international or multi-team projects, identify ownership of cross-team dependencies.

Use:

| Dependency | Provider Team | Receiving Team | Accountable Owner | Required By | Escalation Owner |
|---|---|---|---|---|---|

This is particularly useful when teams work across:

- countries,
- time zones,
- business units,
- vendors,
- platforms.

---

# Governance Red Flags

Flag the matrix when:

```text id="raci-redflags"
No A
Multiple As
No R
One role owns almost every decision
Too many mandatory Cs
Vendor accountability is unclear
Business vs IT ownership is unclear
Approval authority does not match organisational authority
Critical decisions have no escalation path
```

---

# Quality Checklist

Before approving the RACI, confirm:

- [ ] Every critical activity has an Accountable owner
- [ ] Every critical activity has a Responsible owner
- [ ] Multiple Accountables have been reviewed
- [ ] Decision authority is clear
- [ ] Business and IT ownership are differentiated
- [ ] Vendor responsibilities are explicit
- [ ] Security responsibilities are visible
- [ ] Operational ownership is visible
- [ ] Consultation is not unnecessarily complex
- [ ] Escalation ownership is defined for critical decisions

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- responsibility assignment,
- team management,
- stakeholder engagement,
- governance,
- communication,
- decision-making,
- resource management.

## PMBOK Relevance

This prompt supports:

- governance,
- stakeholders,
- resources,
- delivery,
- accountability.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

RACI should support the chosen delivery model rather than replace its established accountabilities.

---

# Human Review Required

Validate the RACI with the actual role owners.

At minimum, review critical accountabilities with:

- Project Sponsor
- Project Manager
- Business Owner
- Product Owner where relevant
- Technical / Architecture Lead
- Security
- Operations
- Vendor leadership where relevant

AI can identify structural governance problems.

It cannot determine organisational authority unless that authority is provided in the project context.

---

# Confidentiality

Avoid including:

- unnecessary personal information,
- confidential organisational hierarchies,
- security-sensitive approval structures,
- restricted supplier information.

Use role names rather than personal names where practical.

---

# Prompt Metadata

```text id="raci-metadata"
Prompt ID: PLAN-003
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Sponsor / PMO / Business Owner
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
| 1.0 | YYYY-MM-DD | Initial IT RACI and governance review framework |
