# Project Charter

## Purpose

Use this prompt to create a structured project charter for an IT or digital initiative.

The project charter should establish:

- why the project exists,
- what value it is expected to create,
- what is in and out of scope,
- who is accountable,
- what constraints and risks exist,
- and how project authority is defined.

The charter should support alignment before detailed planning and delivery begin.

---

## Best Used For

**Project phase:**  
Initiation

**Project type:**  
Software implementation / Digital transformation / System migration / Data project / Infrastructure project / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At project initiation and after major scope or governance changes

---

# Prompt

```text id="charter-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, digital transformation, stakeholder management,
risk management, quality assurance, and project governance.

TASK

Create a professional project charter for the project described below.

PROJECT CONTEXT

Project name:
[PROJECT NAME]

Sponsor:
[SPONSOR]

Project Manager:
[PROJECT MANAGER]

Business owner:
[BUSINESS OWNER]

Project type:
[PROJECT TYPE]

Business problem:
[BUSINESS PROBLEM]

Strategic purpose:
[WHY THE PROJECT EXISTS]

Expected business value:
[EXPECTED VALUE / BENEFITS]

Target completion:
[DATE]

Budget:
[BUDGET OR RANGE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Key stakeholders:
[LIST]

Known dependencies:
[LIST]

Known constraints:
[LIST]

Known risks:
[LIST]

OUTPUT FORMAT

Create the charter with the following sections:

1. Project Purpose and Business Justification

Explain:
- the business problem,
- why the project is required,
- expected organisational value,
- and the consequence of not proceeding.

2. Project Objectives

Create 3-5 measurable objectives.

For each objective include:
- objective,
- success measure,
- target date,
- accountable owner.

3. High-Level Scope

Separate into:

IN SCOPE
OUT OF SCOPE
TO BE CONFIRMED

4. Key Deliverables

Provide:

Deliverable | Description | Target Date | Owner

5. Key Assumptions

Provide:

Assumption | Impact if Incorrect | Validation Owner | Review Date

6. Key Constraints

Assess constraints across:

- Schedule
- Budget
- Resources
- Technology
- Security
- Compliance
- Vendors
- Business Availability

7. High-Level Risks

Provide:

Risk | Probability | Impact | Initial Response | Owner

8. Key Milestones or Delivery Checkpoints

Provide:

Milestone / Checkpoint
Target Date
Dependency
Owner

9. Budget Summary

Summarise the available budget and any major financial constraints.

If detailed financial information is not available, identify the gap
instead of inventing figures.

10. Key Stakeholders and Governance

Provide:

Stakeholder / Governance Body
Role
Decision Authority
Engagement Requirement

11. Project Manager Authority

Define:

- decisions the Project Manager can make independently,
- decisions requiring sponsor approval,
- decisions requiring steering committee or governance approval.

12. Success Criteria

Define success across:

- business value,
- delivery,
- budget,
- quality,
- operational readiness,
- stakeholder acceptance.

13. Authorization

Create a sign-off section:

Project Sponsor:
Project Manager:
Business Owner:
Date:
Charter Version:
```

---

# Delivery-Approach Considerations

Use these only where relevant.

## Agile / Scrum

Consider:

- product vision,
- Product Owner accountability,
- iterative delivery,
- backlog ownership,
- release goals,
- Definition of Done,
- incremental value delivery.

## Kanban

Consider:

- service delivery objective,
- flow-based work management,
- WIP policies,
- Service Level Expectations,
- operational demand,
- continuous delivery constraints.

## Predictive

Consider:

- baseline schedule,
- milestone commitments,
- defined scope baseline,
- critical path,
- formal change control.

## Hybrid

Consider both fixed governance commitments and iterative delivery mechanisms.

---

# Analysis Rules

When producing the charter:

1. Separate confirmed information from assumptions.
2. Do not invent missing budget, timeline, scope, or governance information.
3. Flag contradictory project information.
4. Highlight unclear scope boundaries.
5. Identify objectives that are not measurable.
6. Identify dependencies that could affect project success.
7. Highlight governance gaps where accountability is unclear.
8. Distinguish business outcomes from project deliverables.
9. Use concise professional business language.

---

# Quality Review

After creating the charter, perform a structured review.

| Review Area | Status | Observation | Recommended Action |
|---|---|---|---|
| Business justification | Clear / Needs Clarification | | |
| Objectives | Clear / Needs Clarification | | |
| Scope | Clear / Needs Clarification | | |
| Deliverables | Clear / Needs Clarification | | |
| Dependencies | Clear / Needs Clarification | | |
| Risks | Clear / Needs Clarification | | |
| Governance | Clear / Needs Clarification | | |
| Success criteria | Clear / Needs Clarification | | |

Then provide:

**Top 3 items requiring clarification before charter approval.**

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- business value,
- stakeholder alignment,
- governance,
- risk,
- scope,
- delivery planning,
- accountability,
- decision-making.

## PMBOK Relevance

This prompt supports project initiation and early alignment around:

- value,
- stakeholders,
- governance,
- scope,
- risk,
- planning,
- accountability.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

---

# Example Input

```text id="charter-example-input"
Project Name:
Customer Self-Service Portal

Sponsor:
Director of Customer Operations

Project Manager:
Project Manager

Business Owner:
Customer Operations

Project Type:
Software implementation

Business Problem:
Customers currently rely heavily on email and telephone support
for routine account-management requests.

Strategic Purpose:
Reduce manual service demand and improve digital customer access.

Expected Business Value:
Lower service workload and faster customer response times.

Target Completion:
30 September 2027

Budget:
€750,000

Delivery Approach:
Hybrid Agile

Key Stakeholders:
Customer Operations
IT
Information Security
Finance
Customer Service
External Development Partner

Known Dependencies:
Customer identity API
CRM integration
Security approval
Production infrastructure

Known Constraints:
Limited internal developer availability
External vendor dependency
Fixed regulatory launch deadline

Known Risks:
API integration delay
Security approval delay
Incomplete business requirements
```

---

# Example Output Excerpt

## Project Purpose and Business Justification

The Customer Self-Service Portal project will introduce secure digital self-service capabilities for routine account-management activities.

The project is intended to reduce manual service demand, improve response times, and create a more scalable digital customer-service model.

---

## Example Objective

| Objective | Success Measure | Target Date | Owner |
|---|---|---|---|
| Launch customer self-service portal | Production deployment completed and approved | 30 Sep 2027 | Project Manager |
| Reduce manual requests | Agreed reduction in eligible manual service requests | 6 months after go-live | Customer Operations |
| Achieve production readiness | No unresolved critical release blockers | Before go-live | QA / Delivery Lead |

---

# Human Review Required

Validate the charter with:

- Project Sponsor
- Business Owner
- Finance
- IT / Architecture
- Information Security
- Product Owner where relevant
- Delivery Lead
- PMO or governance body where applicable

The AI-generated charter is a drafting and decision-support tool.

Formal project authorization remains with the accountable project stakeholders.

---

# Confidentiality

Do not include:

- credentials,
- API keys,
- confidential customer data,
- personal employee data,
- commercially sensitive supplier pricing,
- protected contractual information,
- security-sensitive architecture.

Anonymise project information where required.

---

# Prompt Metadata

```text id="charter-metadata"
Prompt ID: INIT-001
Category: Project Initiation
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
| 1.0 | YYYY-MM-DD | Initial IT project charter framework |
