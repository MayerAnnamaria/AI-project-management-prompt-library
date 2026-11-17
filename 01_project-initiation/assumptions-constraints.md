# Assumptions and Constraints Register

## Purpose

Use this prompt to create a structured assumptions and constraints register for an IT project.

The objective is to make hidden dependencies and delivery limitations visible before they become project issues.

An **assumption** is something believed to be true for planning purposes but not yet fully validated.

A **constraint** is a fixed limitation that restricts how the project can be delivered.

---

## Best Used For

**Project phase:**  
Initiation / Planning

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Infrastructure project / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO / Business Analyst

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initiation, then reviewed throughout delivery

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in international
software delivery, risk management, stakeholder coordination,
dependency management, and project governance.

TASK

Create an assumptions and constraints register for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target date:
[DATE]

Budget:
[BUDGET OR RANGE]

Team:
[TEAM STRUCTURE]

Systems involved:
[LIST]

External vendors:
[LIST]

Known dependencies:
[LIST]

Known assumptions:
[LIST]

Known limitations:
[LIST]

OUTPUT FORMAT

Produce two tables.

TABLE 1 — ASSUMPTIONS

Columns:

Assumption ID
Assumption Statement
Category
Reason for Assumption
Impact if Incorrect
Validation Required
Owner
Validation Date
Status

TABLE 2 — CONSTRAINTS

Columns:

Constraint ID
Constraint Description
Category
Impact on Project
Affected Area
Management Approach
Owner
Review Date
```

---

# Recommended Categories

Use only where relevant:

```text
Schedule
Budget
Resources
Technology
Architecture
Integration
Data
Security
Compliance
Vendor
Business Availability
Operations
Quality
Environment
Governance
```

---

# Analysis Rules

When creating the register:

1. Do not invent project facts.
2. Separate assumptions from confirmed constraints.
3. Identify assumptions that could affect:
   - timeline,
   - cost,
   - scope,
   - quality,
   - security,
   - operational readiness.
4. Highlight assumptions without a validation owner.
5. Identify assumptions that should be converted into risks.
6. Identify constraints that may require escalation.
7. Highlight vendor-dependent assumptions.
8. Identify assumptions dependent on stakeholder availability.
9. Flag contradictions between assumptions and known constraints.
10. Make every assumption specific and testable.

---

# Delivery-Approach Considerations

Use only where relevant.

## Agile / Scrum

Consider assumptions related to:

- backlog readiness,
- Product Owner availability,
- team capacity,
- release goals,
- Definition of Done,
- stakeholder feedback availability.

## Kanban

Consider assumptions related to:

- demand volume,
- WIP limits,
- workflow capacity,
- Service Level Expectations,
- blocked work,
- operational intake.

## Predictive

Consider assumptions related to:

- baseline schedule,
- fixed scope,
- milestone commitments,
- resource availability,
- procurement lead times.

## Hybrid

Consider both fixed governance constraints and adaptive delivery assumptions.

---

# Example Input

```text
Project:
CRM replacement

Target go-live:
1 October 2027

Delivery approach:
Hybrid

Team:
1 Project Manager
2 Business Analysts
5 Developers
2 QA Engineers
External migration vendor

Known assumptions:
- Existing customer data can be migrated without major cleansing.
- Business users will be available for UAT in August.
- Vendor API documentation is complete.
- Current infrastructure can support the new CRM.

Known constraints:
- Fixed regulatory go-live date.
- No additional internal developers available.
- Production deployment allowed only during weekend maintenance windows.
- Security review requires four weeks.
```

---

# Example Output — Assumptions

| ID | Assumption | Impact if Incorrect | Owner | Status |
|---|---|---|---|---|
| A-01 | Customer data can be migrated without major cleansing | Migration timeline and budget may increase | Data Lead | To Validate |
| A-02 | Business users will be available for UAT in August | UAT and go-live may slip | Business Owner | To Validate |
| A-03 | Vendor API documentation is complete | Integration work may be delayed | Integration Lead | To Validate |
| A-04 | Existing infrastructure can support the new CRM | Additional infrastructure work may be required | Solution Architect | To Validate |

---

# Example Output — Constraints

| ID | Constraint | Category | Project Impact | Owner |
|---|---|---|---|---|
| C-01 | Fixed regulatory go-live date | Schedule | Limited recovery time if delivery slips | Project Sponsor |
| C-02 | No additional internal developers available | Resources | Reduced delivery flexibility | Engineering Manager |
| C-03 | Weekend-only production deployment | Operations | Limits release windows | Operations Lead |
| C-04 | Four-week security review | Security | Must be planned into delivery timeline | Security Lead |

---

# Assumption-to-Risk Review

After producing the register, identify assumptions that should be converted into project risks.

Use:

| Assumption | Why It Creates Risk | Probability | Impact | Recommended Action |
|---|---|---|---|---|

Example:

```text
Assumption:
Business users will be available for UAT.

Potential Risk:
Business availability may be lower than expected.

Impact:
Testing and go-live readiness may be delayed.
```

---

# Constraint Escalation Review

Identify constraints that require management or governance attention.

Provide:

```text
Constraint
Why Escalation Is Required
Decision Needed
Decision Owner
Decision Deadline
```

---

# Quality Checklist

Before accepting the register, confirm:

- [ ] Every assumption is testable
- [ ] Material assumptions have owners
- [ ] Validation dates are defined
- [ ] Constraints are separated from risks
- [ ] External dependencies are visible
- [ ] High-impact assumptions are highlighted
- [ ] Contradictions are identified
- [ ] Review dates are included
- [ ] Unsupported assumptions are not presented as facts

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- assumptions management,
- constraints management,
- risk identification,
- stakeholder alignment,
- dependency management,
- governance,
- planning.

## PMBOK Relevance

This prompt supports:

- planning,
- uncertainty,
- risk,
- governance,
- stakeholders,
- delivery.

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

Validate the register with relevant stakeholders, including:

- Project Sponsor
- Business Owner
- Product Owner where relevant
- Solution Architect
- Security Lead
- Data Lead
- QA Lead
- External vendors where applicable

The register should remain a living project artifact and be reviewed when:

- a major milestone is reached,
- a dependency changes,
- a risk materialises,
- scope changes,
- or a major project decision is made.

---

# Confidentiality

Do not include:

- customer personal data,
- employee personal data,
- credentials,
- passwords,
- API keys,
- confidential supplier pricing,
- confidential contract terms,
- proprietary architecture,
- security-sensitive information.

---

# Prompt Metadata

```text
Prompt ID: INIT-004
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor / Business Owner
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
| 1.0 | YYYY-MM-DD | Initial assumptions and constraints register |
