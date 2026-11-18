# Project Brief

**Prompt ID:** INIT-002 | **Category:** Project Initiation | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Convert preliminary project information into a structured brief that supports stakeholder alignment, scope clarification, and informed planning decisions.

**Use case:** Consolidate incomplete stakeholder requirements, discovery notes, and early project proposals to identify scope gaps, dependencies, and decisions before detailed planning.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
requirements analysis, stakeholder management, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [INITIATION / DISCOVERY]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target date: [DATE, IF KNOWN]
Budget: [BUDGET, IF KNOWN]
Stakeholders: [KNOWN ROLES]
Systems and vendors: [DETAILS]
Project information: [PASTE NOTES / REQUIREMENTS / MEETING SUMMARY]

TASK

Create a structured Project Brief from the available information.

1. Summarize the business problem, proposed initiative, expected value,
   and intended outcomes.
2. Identify objectives and flag missing measurable criteria.
3. Classify scope as In Scope, Out of Scope, or To Be Confirmed.
4. Identify deliverables, expected outcomes, owners, and target dates.
5. Categorize business, functional, technical, data, security,
   operational, and compliance requirements.
6. Assess schedule, budget, resource, technology, security,
   compliance, vendor, business availability, and operational constraints.
7. Identify dependencies and their potential delivery impacts.
8. Identify stakeholders, responsibilities, decision authority,
   and engagement requirements.
9. Document initial risks, causes, impacts, and proposed responses.
10. Record assumptions and required validation actions.
11. Identify considerations relevant to the stated delivery approach.
12. Flag unclear requirements, scope gaps, contradictions,
    unresolved ownership, and missing governance decisions.
13. Recommend the five highest-priority next steps.

Preserve confirmed facts and distinguish them from assumptions.
Separate business outcomes from project deliverables.
Do not invent information or infer unapproved scope.

OUTPUT FORMAT

Produce a Project Brief with the following sections:

1. PROJECT OVERVIEW
   Business Problem | Proposed Initiative | Expected Value

2. PROJECT OBJECTIVES
   Objective | Expected Outcome | Measurement | Owner

3. HIGH-LEVEL SCOPE
   In Scope | Out of Scope | To Be Confirmed

4. KEY DELIVERABLES
   Deliverable | Description | Expected Outcome | Owner | Target Date

5. KEY REQUIREMENTS
   Category | Requirement | Status
   Categories: Business, Functional, Technical, Data,
   Security, Operational, Compliance

6. KEY CONSTRAINTS
   Constraint | Category | Delivery Impact

7. KEY DEPENDENCIES
   Dependency | Type | Impact | Owner | Required By | Status

8. KEY STAKEHOLDERS
   Stakeholder | Role | Interest | Decision Authority |
   Engagement Requirement

9. HIGH-LEVEL RISKS
   Risk | Cause | Potential Impact | Initial Response | Owner

10. ASSUMPTIONS
    Assumption | Reason | Impact if Incorrect |
    Validation Required | Owner

11. DELIVERY APPROACH
    Relevant framework and delivery considerations

12. OPEN QUESTIONS
    Question | Decision Owner | Priority

13. RECOMMENDED NEXT STEPS
    Action | Priority | Proposed Owner | Expected Outcome

Use concise Markdown tables where appropriate.
Mark missing information as "Not yet defined".
Label proposed owners, dates, and commitments as unconfirmed.
```

---

## 2. Quality Check

Apply this quality control to the generated Project Brief.

```text
QUALITY CHECK

Act as a Senior QA Manager and validate the Project Brief.

Verify:
1. Completeness: All 13 required sections are addressed.
2. Accuracy: Facts, assumptions, and information gaps are distinguished.
3. Scope: Unapproved requirements are not presented as commitments.
4. Consistency: Objectives, deliverables, risks, and dependencies align.
5. Governance: Ownership, decisions, and required approvals are visible.
6. Actionability: Next steps are specific, feasible, and prioritized.

OUTPUT
Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]

Flag unsupported conclusions and decisions requiring human validation.
Do not invent missing facts, metrics, owners, or deadlines.
```

---

## 3. Practical IT Use Case

### Customer Self-Service Portal — Project Initiation

**Scenario:** A company plans to introduce a customer self-service portal to reduce support requests. Preliminary stakeholder discussions have identified business needs, technical dependencies, and an indicative budget, but scope, feasibility, and funding require confirmation.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Initiation / Discovery |
| Target launch | September (year unconfirmed) |
| Indicative budget | €500,000 (unapproved) |
| External vendor | Development partner available from March |
| Dependencies | CRM API, authentication, security approval |
| Management decision | Confirm scope, feasibility, funding, and ownership before detailed planning |

### Example Input

```text
Project: Customer Self-Service Portal

Business problem:
Customers contact support for address changes, invoice copies,
payment-status inquiries, and account updates.
Customer Service reports excessive request volumes.

Business objective:
Reduce manual service requests through digital self-service.

Known information:
- Existing authentication may be reusable.
- CRM API may require modifications.
- Security approval is required for authentication.
- External development partner can start in March.
- Indicative budget: €500,000; Finance approval pending.
- Target launch: September; year unconfirmed.
- Marketing requests mobile-responsive design.
- Operations requests a reporting dashboard.
- Online bank-detail changes are not yet agreed.
```

### Example Output — Project Brief

#### 1. Project Overview

Develop a Customer Self-Service Portal to reduce manual support requests and improve digital access to routine account services.

**Expected business value:** Lower service workload, faster customer interactions, and improved service accessibility.

#### 2. Project Objectives

| Objective | Expected Outcome | Measurement | Owner |
|---|---|---|---|
| Reduce manual requests | Lower support workload | Request volume reduction; target TBD | Not defined |
| Improve digital access | Increased self-service adoption | Adoption rate; target TBD | Not defined |

#### 3. High-Level Scope

| In Scope | Out of Scope | To Be Confirmed |
|---|---|---|
| No approved items | No confirmed exclusions | Address updates, invoice retrieval, payment-status visibility, account updates, mobile responsiveness, bank-detail changes, reporting dashboard |

#### 4. Key Deliverables

| Deliverable | Description | Expected Outcome | Owner | Target Date |
|---|---|---|---|---|
| Customer portal (proposed) | Digital self-service interface | Reduced manual interactions | TBD | September, year TBD |
| Authentication integration (proposed) | Customer access capability | Secure access | TBD | TBD |

#### 5. Key Requirements

| Category | Requirement | Status |
|---|---|---|
| Business | Reduce support workload | Identified; target undefined |
| Functional | Address updates, invoice retrieval | Proposed |
| Technical | CRM API integration | Feasibility unconfirmed |
| Data | Not yet defined | Missing |
| Security | Authentication approval | Required |
| Operational | Reporting dashboard | Proposed |
| Compliance | Not yet defined | Missing |

#### 6. Key Constraints

| Constraint / Limitation | Category | Delivery Impact |
|---|---|---|
| €500,000 indicative budget | Budget | Funding approval pending |
| September target | Schedule | Feasibility unconfirmed |
| Vendor availability from March | Vendor | Influences delivery planning |

*These are preliminary planning limitations, not approved project baselines.*

#### 7. Key Dependencies

| Dependency | Type | Impact | Owner | Required By | Status |
|---|---|---|---|---|---|
| CRM API assessment | Technical | Integration effort uncertain | TBD | TBD | Open |
| Authentication approval | Security | Required before solution approval | TBD | TBD | Open |
| Funding approval | Financial | Delivery commitment unresolved | TBD | TBD | Open |

#### 8. Key Stakeholders

| Stakeholder | Role | Interest | Decision Authority | Engagement Requirement |
|---|---|---|---|---|
| Customer Service | Business stakeholder | Reduce workload | TBD | Validate requirements |
| IT | Technical stakeholder | Integration feasibility | TBD | Architecture assessment |
| Finance | Financial stakeholder | Funding | TBD | Confirm budget |
| Security | Security reviewer | Authentication | Authentication approval | Review access design |
| Marketing | Business stakeholder | Mobile experience | TBD | Clarify design requirements |
| Operations | Operational stakeholder | Reporting | TBD | Define dashboard scope |

#### 9. High-Level Risks

| Risk | Cause | Potential Impact | Initial Response | Owner |
|---|---|---|---|---|
| CRM integration delay | Legacy API limitations | Schedule and cost overruns | Technical assessment | TBD |
| Authentication redesign | Existing solution may be unsuitable | Additional development effort | Architecture review | TBD |
| Scope expansion | Unresolved feature requests | Budget and timeline impact | Confirm release scope | TBD |

#### 10. Assumptions

| Assumption | Reason | Impact if Incorrect | Validation Required | Owner |
|---|---|---|---|---|
| Existing authentication can be reused | Preliminary IT input | Additional development effort | Technical assessment | TBD |
| Vendor can start in March | Initial availability information | Schedule delay | Confirm availability | TBD |

#### 11. Delivery Approach

The delivery methodology is not yet confirmed. Evaluate scope uncertainty, technical dependencies, and governance requirements before selecting the delivery approach.

#### 12. Open Questions

| Question | Decision Owner | Priority |
|---|---|---|
| Is the €500,000 budget approved? | Finance / approver TBD | High |
| Is September a fixed deadline? | TBD | High |
| Can existing authentication be reused? | TBD | High |
| Are bank-detail changes included? | TBD | High |
| Is the dashboard part of the first release? | TBD | Medium |

#### 13. Recommended Next Steps

| Action | Priority | Proposed Owner | Expected Outcome |
|---|---|---|---|
| Confirm funding | High | Finance | Funding decision |
| Assess CRM and authentication feasibility | High | IT Lead | Technical assessment |
| Define initial release scope | High | Business Owner | Agreed scope proposal |
| Validate delivery schedule | High | Project Manager | Feasible timeline |
| Establish decision authority | High | Project Sponsor | Governance structure |

### Management Decisions

1. **Funding:** Confirm the approved budget and financial authority.
2. **Scope:** Agree on initial release functionality and exclusions.
3. **Technical feasibility:** Validate CRM integration and authentication requirements.
4. **Governance:** Establish decision authority and obtain approval before detailed planning.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The business problem and major dependencies are identified, but funding, scope approval, measurable objectives, technical feasibility, and decision ownership remain unresolved.

**Required corrections:** Validate these outstanding items with accountable stakeholders before treating the brief as an approved planning reference.

**Governance:** This preliminary brief supports relevant PMI-aligned initiation, stakeholder, scope, and uncertainty management practices. It does not replace an approved project charter or scope baseline. Human validation is required before delivery commitments are established, and confidential project information must be protected.
