# Project Charter

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** INIT-003 | **Category:** Project Initiation

---


## 1. Ready-to-Use Prompt

**Purpose:** Use this prompt to create a structured project charter for an IT or digital initiative: establish project objectives, business value, scope, accountability, and governance to support formal project authorization.

The project charter should establish:

- why the project exists,
- what value it is expected to create,
- what is in and out of scope,
- who is accountable,
- what constraints and risks exist,
- and how project authority is defined.

The charter should support alignment before detailed planning and delivery begin.

**Use case:** Prepare a project charter when initiating an IT initiative, confirming sponsorship and funding, or defining approval authority before detailed planning.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
digital transformation, stakeholder management, risk management,
and project governance.

CONTEXT

Project: [PROJECT NAME]
Sponsor: [SPONSOR]
Project Manager: [PROJECT MANAGER]
Business Owner: [BUSINESS OWNER]
Project type: [PROJECT TYPE]
Business problem: [PROBLEM]
Strategic purpose: [BUSINESS OBJECTIVE]
Expected business value: [BENEFITS]
Target completion: [DATE]
Budget: [BUDGET OR RANGE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Stakeholders: [LIST]
Dependencies: [LIST]
Constraints: [LIST]
Known risks: [LIST]

TASK

Create a professional Project Charter from the available information.

1. Define the business justification, expected value, and
   consequences of not proceeding.
2. Identify 3–5 project objectives, measurable where supported
   by available information; flag missing targets.
3. Classify scope as In Scope, Out of Scope, or To Be Confirmed.
4. Identify key deliverables, proposed owners, and target dates.
5. Document assumptions, validation requirements, and potential impacts.
6. Assess schedule, budget, resource, technology, security,
   compliance, vendor, and business availability constraints.
7. Identify high-level risks and appropriate initial responses.
8. Define key milestones, dependencies, and delivery checkpoints.
9. Summarize the available budget and financial limitations.
10. Identify stakeholders, responsibilities, governance bodies,
    and decision-making authority.
11. Distinguish Project Manager authority from decisions requiring
    sponsor or steering committee approval.
12. Define success criteria covering business value, delivery,
    budget, quality, operational readiness, and stakeholder acceptance.
13. Prepare an authorization section for formal stakeholder sign-off.

Preserve confirmed facts and distinguish them from assumptions.
Flag unclear scope, contradictions, missing ownership, and
unresolved governance decisions.
Do not invent budget figures, dates, targets, or approval authority.
Separate business outcomes from project deliverables.

OUTPUT FORMAT

Produce a Project Charter containing:

1. PROJECT PURPOSE AND BUSINESS JUSTIFICATION
   Business Problem | Strategic Purpose | Expected Value |
   Consequences of Not Proceeding

2. PROJECT OBJECTIVES
   Objective | Success Measure | Target Date | Accountable Owner

3. HIGH-LEVEL SCOPE
   In Scope | Out of Scope | To Be Confirmed

4. KEY DELIVERABLES
   Deliverable | Description | Target Date | Owner

5. KEY ASSUMPTIONS
   Assumption | Impact if Incorrect | Validation Owner | Review Date

6. KEY CONSTRAINTS
   Constraint | Category | Project Impact

7. HIGH-LEVEL RISKS
   Risk | Probability | Impact | Initial Response | Owner

8. KEY MILESTONES
   Milestone / Checkpoint | Target Date | Dependency | Owner

9. BUDGET SUMMARY
   Available Budget | Financial Constraints | Approval Status

10. STAKEHOLDERS AND GOVERNANCE
    Stakeholder / Governance Body | Role |
    Decision Authority | Engagement Requirement

11. PROJECT MANAGER AUTHORITY
    Independent Decisions | Sponsor Approval |
    Steering Committee / Governance Approval

12. SUCCESS CRITERIA
    Dimension | Success Criterion | Measurement |
    Acceptance Authority

13. AUTHORIZATION
    Project Sponsor | Project Manager | Business Owner |
    Date | Charter Version | Approval Status

Use concise Markdown tables where appropriate.
Mark missing information as "Not yet defined".
Label proposed owners, dates, and decisions as unconfirmed.
Do not imply authorization without documented approval.
```

---

## 2. Quality Check

Apply this quality control after generating the Project Charter.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Project Charter.

Verify:
1. Completeness: All 13 required charter sections are addressed.
2. Accuracy: Facts, assumptions, estimates, and gaps are distinguished.
3. Business alignment: Objectives, expected value, and success
   measures are consistent.
4. Scope and feasibility: Boundaries, constraints, dependencies,
   and material risks are adequately identified.
5. Governance: Sponsor accountability, Project Manager authority,
   approval requirements, and unresolved decisions are explicit.
6. Authorization: No unapproved commitments or implied sign-offs.
7. Actionability: Critical gaps have clear proposed resolution actions.

OUTPUT

Quality verdict: PASS / REVISE

Provide a review table:
Area | Status (Clear / Needs Clarification) |
Finding | Required Correction

Identify the top three issues requiring resolution before approval.

Do not invent missing facts, metrics, authorities, or approvals.
Flag consequential decisions requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Customer Self-Service Portal — Project Authorization

**Scenario:** A company proposes a customer self-service portal to reduce manual support requests and improve digital service delivery. The Project Sponsor needs a charter establishing business justification, delivery boundaries, financial expectations, and decision authority before approving the initiative.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Initiation |
| Project type | Software implementation |
| Delivery approach | Hybrid Agile |
| Target completion | 30 September 2027 |
| Budget | €750,000 |
| Sponsor | Director of Customer Operations |
| Key dependencies | Customer identity API, CRM integration, security approval, production infrastructure |
| Management decision | Determine whether the project is sufficiently defined for formal authorization |

### Example Input

```text
Project: Customer Self-Service Portal
Sponsor: Director of Customer Operations
Project Manager: Project Manager
Business Owner: Customer Operations
Project type: Software implementation

Business problem:
Customers rely heavily on email and telephone support
for routine account-management requests.

Strategic purpose:
Reduce manual service demand and improve digital customer access.

Expected business value:
Lower support workload and faster customer response times.

Target completion: 30 September 2027
Budget: €750,000
Delivery approach: Hybrid Agile

Key stakeholders:
Customer Operations, IT, Information Security, Finance,
Customer Service, External Development Partner

Dependencies:
Customer identity API, CRM integration, security approval,
production infrastructure

Constraints:
Limited internal developer availability.
External vendor dependency.
Fixed regulatory launch deadline.

Known risks:
API integration delay.
Security approval delay.
Incomplete business requirements.
```

### Example Output — Project Charter

#### 1. Project Purpose and Business Justification

Develop a secure Customer Self-Service Portal to reduce reliance on manual support channels and improve access to routine account services.

**Expected value:** Reduced service workload, faster customer response times, and improved scalability.

**Consequence of not proceeding:** Continued dependence on manual support channels and limited digital self-service capability.

#### 2. Project Objectives

| Objective | Success Measure | Target Date | Accountable Owner |
|---|---|---|---|
| Launch the customer portal | Approved production deployment | 30 Sep 2027 | Project Manager (proposed) |
| Reduce manual requests | Reduction against an agreed baseline; target TBD | 6 months after go-live (proposed) | Customer Operations (proposed) |
| Achieve release readiness | Required acceptance and security approvals completed | Before go-live | QA / Delivery Lead (proposed) |

#### 3. High-Level Scope

| In Scope | Out of Scope | To Be Confirmed |
|---|---|---|
| No formally approved items | No confirmed exclusions | Self-service capabilities, CRM integration, identity integration, customer-facing functionality |

*Functional boundaries require stakeholder agreement before scope approval.*

#### 4. Key Deliverables

| Deliverable | Description | Target Date | Owner |
|---|---|---|---|
| Customer portal (proposed) | Digital self-service solution | 30 Sep 2027 | TBD |
| CRM integration (proposed) | Customer data exchange | TBD | TBD |
| Identity integration (proposed) | Secure customer access | TBD | TBD |

#### 5. Key Assumptions

| Assumption | Impact if Incorrect | Validation Owner | Review Date |
|---|---|---|---|
| Required APIs can support the solution | Additional integration effort | TBD | TBD |
| External partner capacity will be available | Delivery delays | TBD | TBD |

#### 6. Key Constraints

| Constraint | Category | Project Impact |
|---|---|---|
| Fixed regulatory launch deadline | Schedule / Compliance | Limited schedule flexibility |
| Limited internal developers | Resources | Reduced delivery capacity |
| External development dependency | Vendor | Delivery affected by supplier availability |

#### 7. High-Level Risks

| Risk | Probability | Impact | Initial Response | Owner |
|---|---|---|---|---|
| API integration delay | Not assessed | Schedule impact | Validate API readiness | TBD |
| Security approval delay | Not assessed | Release delay | Engage Security early | TBD |
| Incomplete requirements | Not assessed | Rework and scope uncertainty | Conduct requirements review | TBD |

#### 8. Key Milestones

| Milestone / Checkpoint | Target Date | Dependency | Owner |
|---|---|---|---|
| Requirements approval | TBD | Business stakeholder alignment | TBD |
| Integration readiness | TBD | Identity and CRM APIs | TBD |
| Security approval | TBD | Security assessment | TBD |
| Production launch | 30 Sep 2027 | Release readiness and approvals | TBD |

#### 9. Budget Summary

| Available Budget | Financial Constraints | Approval Status |
|---|---|---|
| €750,000 stated budget | Resource limitations and vendor dependency | Not confirmed |

*The available information does not establish whether the budget is formally approved.*

#### 10. Stakeholders and Governance

| Stakeholder | Role | Decision Authority | Engagement Requirement |
|---|---|---|---|
| Director of Customer Operations | Project Sponsor | To be confirmed | Project authorization |
| Customer Operations | Business Owner | To be confirmed | Business requirements and benefits |
| IT | Technical stakeholder | To be confirmed | Architecture and integration |
| Information Security | Security stakeholder | To be confirmed | Security approval |
| Finance | Financial stakeholder | To be confirmed | Budget validation |
| External Development Partner | Delivery supplier | Contract-dependent | Delivery coordination |

#### 11. Project Manager Authority

| Decision Area | Proposed Authority |
|---|---|
| Routine delivery coordination | Project Manager — subject to confirmation |
| Budget or scope changes | Sponsor approval — to be confirmed |
| Major changes and escalations | Applicable governance body — not yet defined |

*Formal decision limits must be agreed before authorization.*

#### 12. Success Criteria

| Dimension | Success Criterion | Measurement | Acceptance Authority |
|---|---|---|---|
| Business value | Reduced manual support demand | Baseline vs. post-launch volume; target TBD | TBD |
| Delivery | Launch by target date | Actual vs. target completion | TBD |
| Budget | Delivery within approved funding | Actual vs. approved budget | TBD |
| Quality | Required acceptance criteria met | UAT results and outstanding defects | TBD |
| Operational readiness | Support and deployment readiness confirmed | Readiness assessment | TBD |
| Stakeholder acceptance | Required approvals obtained | Recorded sign-offs | TBD |

#### 13. Authorization

| Role | Name / Authority | Approval Status | Date |
|---|---|---|---|
| Project Sponsor | Director of Customer Operations | Pending | TBD |
| Project Manager | Not specified | Pending | TBD |
| Business Owner | Customer Operations | Pending | TBD |

**Charter version:** 1.0 (draft example)

### Management Decisions

1. **Business justification:** Confirm measurable business benefits and establish the baseline for reducing manual requests.
2. **Scope and feasibility:** Approve initial scope boundaries and validate CRM and identity integration requirements.
3. **Financial governance:** Confirm the €750,000 budget approval and resource commitments.
4. **Authorization:** Define Project Manager authority, governance escalation paths, and required signatories before approval.

### Applied Quality Review

**Quality verdict: REVISE**

| Area | Status | Finding | Required Correction |
|---|---|---|---|
| Business justification | Needs Clarification | Benefits lack measurable targets | Agree benefit measures and baselines |
| Scope | Needs Clarification | No approved scope boundaries | Confirm inclusions and exclusions |
| Governance | Needs Clarification | Decision authority is undefined | Establish approval responsibilities |
| Budget | Needs Clarification | Approval status is unknown | Confirm authorized funding |

**Top three approval blockers:** Unapproved scope, undefined governance authority, and unconfirmed budget authorization.

**Governance:** The charter supports relevant PMI-aligned practices in business justification, stakeholder accountability, risk management, and project authorization. Formal approval remains the responsibility of the designated project governance authorities. Protect confidential, commercial, personal, and security-sensitive information.

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
