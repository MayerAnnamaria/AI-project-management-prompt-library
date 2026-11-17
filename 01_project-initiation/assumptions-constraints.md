# Assumptions and Constraints Register

## Purpose

Use this prompt to create a structured assumptions and constraints register for an IT project.

The purpose is to make hidden project dependencies visible before they become delivery issues.

Assumptions should be treated as conditions believed to be true but not yet fully confirmed.

Constraints are fixed limitations that restrict how the project can be delivered.

---

## Best Used For

**Project phase:**  
Initiation / Planning

**Project type:**  
Software development / System implementation / Digital transformation / Data project / Infrastructure project

**Primary user:**  
Project Manager / Project Coordinator / PMO / Business Analyst

**Recommended frequency:**  
At initiation, then reviewed regularly throughout delivery

---

# Prompt

```text id="assumptions-01"
ROLE

You are a senior IT Project Manager experienced in software delivery,
cross-functional coordination, risk management, stakeholder management,
and project governance.

TASK

Create an assumptions and constraints register for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[BUSINESS OBJECTIVE]

Current phase:
[INITIATION / PLANNING / DELIVERY]

Target date:
[DATE]

Budget:
[BUDGET OR BUDGET RANGE]

Team:
[TEAM STRUCTURE]

Systems involved:
[LIST]

External vendors:
[LIST]

Known dependencies:
[LIST]

Known limitations:
[LIST]

Known assumptions:
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
Project Impact
Affected Area
Mitigation / Management Approach
Owner
Review Date
```

---

# Categories

Use the following categories where relevant:

```text id="assumptions-categories"
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
Environment
Operations
Quality
```

Do not force every project into every category.

Only include categories supported by the project context.

---

# Analysis Rules

When creating the register:

1. Do not invent project facts.
2. Separate confirmed constraints from assumptions.
3. Identify assumptions that could materially affect:
   - timeline,
   - cost,
   - scope,
   - quality,
   - security,
   - operational readiness.
4. Highlight assumptions with no clear validation owner.
5. Identify assumptions that should be converted into risks.
6. Identify constraints that require escalation.
7. Flag assumptions that depend on external vendors.
8. Identify assumptions that depend on stakeholder availability.
9. Highlight contradictions between assumptions and known constraints.
10. Make each statement specific and testable.

---

# Example Input

```text id="assumptions-example-input"
Project:
CRM replacement

Target go-live:
1 October 2027

Delivery model:
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
| A-03 | Vendor API documentation is complete | Integration development may be delayed | Integration Lead | To Validate |
| A-04 | Existing infrastructure can support the new CRM | Additional infrastructure work may be required | Solution Architect | To Validate |

---

# Example Output — Constraints

| ID | Constraint | Category | Project Impact | Owner |
|---|---|---|---|---|
| C-01 | Fixed regulatory go-live date | Schedule | Limited recovery time if delivery slips | Project Sponsor |
| C-02 | No additional internal developers available | Resources | Reduced flexibility for parallel work | Engineering Manager |
| C-03 | Weekend-only production deployment | Operations | Limits release windows | Operations Lead |
| C-04 | Four-week security review | Security | Must be planned into critical path | Security Lead |

---

# Assumption-to-Risk Review

After producing the register, identify assumptions that should be converted into risks.

Use this table:

| Assumption | Why It Is a Risk | Probability | Impact | Recommended Action |
|---|---|---|---|---|

Example:

```text id="assumption-risk-example"
Assumption:
Business users will be available for UAT.

Risk:
Business availability may be lower than expected during the planned UAT period.

Impact:
Testing may be delayed, affecting go-live readiness.
```

---

# Constraint Escalation Review

Identify constraints that require senior management attention.

Provide:

```text id="constraint-escalation"
Constraint
Why Escalation Is Required
Decision Needed
Decision Owner
Decision Deadline
```

---

# Quality Review

Before accepting the register, verify:

- [ ] Every assumption is testable
- [ ] Every material assumption has an owner
- [ ] Validation dates are defined
- [ ] Constraints are separated from risks
- [ ] External dependencies are visible
- [ ] High-impact assumptions are highlighted
- [ ] Contradictions are identified
- [ ] Review dates are included
- [ ] No unsupported assumptions are presented as facts

---

# Human Review Required

Validate the register with relevant stakeholders, including:

- Project Sponsor
- Business Owner
- Product Owner
- Solution Architect
- Security Lead
- Data Lead
- QA Lead
- External vendors where applicable

The assumptions register should remain a living project artifact.

It should be reviewed when:

- a major milestone is reached,
- a dependency changes,
- a risk materialises,
- scope changes,
- or a major project decision is made.

---

# Prompt Metadata

```text id="assumptions-metadata"
Prompt ID: INIT-004
Category: Project Initiation
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor / Business Owner
Project Type: IT / Digital Transformation
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial assumptions and constraints register |
