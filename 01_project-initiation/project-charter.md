# Project Charter

## Purpose

Use this prompt to create a structured project charter for an IT or digital transformation initiative.

A project charter should establish the project mandate, business purpose, high-level scope, objectives, major risks, governance, and decision authority before detailed delivery begins.

---

## Best Used For

**Project phase:**  
Initiation

**Project type:**  
IT implementation / Software development / Digital transformation / Data project / System migration

**Primary user:**  
Project Manager / Project Coordinator / PMO / Delivery Manager

**Recommended frequency:**  
Once at project initiation, then reviewed after major scope or governance changes

---

# Prompt

```text id="charter-01"
ROLE

You are a senior IT Project Manager experienced in software implementation,
digital transformation, cross-functional delivery, stakeholder management,
risk management, and project governance.

TASK

Create a professional project charter for the project described below.

PROJECT CONTEXT

Project name:
[PROJECT NAME]

Sponsor:
[SPONSOR / BUSINESS OWNER]

Project Manager:
[PROJECT MANAGER]

Project type:
[SOFTWARE IMPLEMENTATION / DIGITAL TRANSFORMATION / SYSTEM MIGRATION / DATA PROJECT]

Business problem:
[PROBLEM THE PROJECT IS INTENDED TO SOLVE]

Strategic purpose:
[WHY THE ORGANISATION IS INVESTING IN THE PROJECT]

Target completion:
[DATE]

Budget:
[BUDGET OR BUDGET RANGE]

Delivery methodology:
[AGILE / SCRUM / WATERFALL / HYBRID]

Key stakeholders:
[LIST]

Known dependencies:
[LIST]

Known constraints:
[LIST]

Known risks:
[LIST]

OUTPUT FORMAT

Create the project charter with the following sections:

1. Project Purpose and Business Justification

Explain:
- the business problem,
- why the project is required,
- and the expected organisational benefit.

2. Project Objectives

Create 3-5 SMART objectives.

For each objective include:
- objective,
- success measure,
- target date,
- accountable owner.

3. High-Level Scope

Separate clearly into:

IN SCOPE
OUT OF SCOPE

Identify any scope boundaries that require clarification.

4. Key Deliverables

Provide a table:

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
- Regulatory / Compliance
- Vendors
- Business Availability

7. High-Level Risks

Provide:

Risk | Probability | Impact | Initial Response | Owner

Do not invent project-specific risks without explaining the assumption.

8. High-Level Milestones

Provide:

Milestone | Target Date | Dependency | Owner

9. Budget Summary

Summarise the available project budget.

Where detailed financial information is unavailable, identify the information gap
rather than inventing figures.

10. Key Stakeholders and Governance

Provide:

Stakeholder / Governance Body
Role
Decision Authority
Engagement Requirement

11. Project Manager Authority

Define what decisions the Project Manager can make independently and what
requires sponsor or steering committee approval.

12. Success Criteria

Define the conditions that must be met for the project to be considered successful.

Include:

- business outcome,
- schedule,
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

# Analysis Rules

When producing the charter:

1. Separate confirmed information from assumptions.
2. Do not invent missing budget, timeline, scope, or governance information.
3. Flag contradictory project information.
4. Highlight unclear scope boundaries.
5. Identify objectives that are not measurable.
6. Identify dependencies that could affect the project start or completion date.
7. Highlight governance gaps where decision ownership is unclear.
8. Use concise professional business language.

---

# Quality Review

After creating the charter, perform a short quality review.

Use this format:

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

# Example Input

```text id="charter-example-input"
Project Name:
Customer Self-Service Portal

Sponsor:
Director of Customer Operations

Project Manager:
Project Manager

Project Type:
Software implementation

Business Problem:
Customers currently rely on email and telephone support for account changes,
creating long response times and high service workload.

Strategic Purpose:
Introduce digital self-service capabilities and reduce manual support demand.

Target Completion:
30 September 2027

Budget:
€750,000

Delivery Methodology:
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

The Customer Self-Service Portal project will introduce secure digital
self-service functionality for common customer account activities.

The project is intended to reduce dependency on manual customer-service
processes, improve response times, and provide customers with a more scalable
digital service channel.

---

## SMART Objective Example

| Objective | Success Measure | Target Date | Owner |
|---|---|---|---|
| Launch the customer portal | Production release completed and approved | 30 Sep 2027 | Project Manager |
| Reduce manual account-change requests | 30% reduction within 6 months of launch | 31 Mar 2028 | Customer Operations |
| Achieve security readiness | All critical security findings resolved before production | Before go-live | Security Lead |

---

# Human Review Required

Before approving the charter, validate:

- business objectives with the sponsor,
- budget with Finance,
- technical dependencies with IT,
- security requirements with Information Security,
- operational readiness with the business owner,
- governance authority with the steering committee.

The AI-generated charter is a drafting and decision-support tool.

Formal approval remains with the accountable project stakeholders.

---

# Confidentiality

Do not include:

- production credentials,
- API keys,
- confidential customer data,
- personal employee data,
- commercially sensitive supplier pricing,
- confidential contract terms,
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
Reviewer: PMO / Project Sponsor
Project Type: IT / Digital Transformation
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT project charter framework |
