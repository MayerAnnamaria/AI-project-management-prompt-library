# Project Brief

**Prompt ID:** INIT-002 | **Category:** Project Initiation | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Transform preliminary project information into a structured brief supporting stakeholder alignment, scope definition, and delivery planning.

**Use case:** Consolidate incomplete stakeholder requirements, discovery notes, and early project proposals to clarify scope, feasibility, ownership, and decisions before detailed planning.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software
delivery, requirements analysis, stakeholder management,
and project governance.

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
2. Identify project objectives and flag missing measurable criteria.
3. Classify scope as In Scope, Out of Scope, or To Be Confirmed.
4. Identify deliverables, expected outcomes, owners, and target dates.
5. Categorize business, functional, technical, data, security,
   operational, and compliance requirements.
6. Assess known schedule, budget, resource, technology, security,
   compliance, vendor, business availability, and operational constraints.
7. Identify dependencies and their potential delivery impacts.
8. Identify stakeholders, interests, responsibilities,
   decision authority, and engagement needs.
9. Document initial risks, causes, impacts, and proposed responses.
10. Record assumptions and required validation actions.
11. Identify considerations relevant to the stated delivery approach.
12. Flag unclear requirements, scope gaps, contradictions,
    unresolved ownership, and missing governance decisions.
13. Recommend the five highest-priority actions for project progression.

Preserve confirmed facts. Separate assumptions from evidence.
Distinguish business outcomes from project deliverables.
Do not invent missing information or infer unapproved scope.

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
Label proposed ownership, dates, and commitments as unconfirmed.
```

---

## 2. Quality Check

Apply this quality control to the generated Project Brief.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Project Brief.

Verify:
1. Completeness: All 13 required sections are addressed.
2. Accuracy: Facts, assumptions, and information gaps are distinguished.
3. Scope: Unapproved requirements are not treated as commitments.
4. Consistency: Objectives, scope, deliverables, risks, and
   dependencies are aligned.
5. Governance: Ownership, decisions, and required approvals are visible.
6. Actionability: Next steps are feasible, prioritized, and specific.

OUTPUT
Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]

Do not invent facts, metrics, owners, or deadlines.
Flag decisions requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Customer Self-Service Portal — Project Initiation

**Scenario:** A company plans to introduce a customer self-service portal to reduce support requests. Initial discussions have identified potential functionality, technical dependencies, and an indicative budget, but scope and funding remain unapproved.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Initiation / Discovery |
| Target launch | September (year unconfirmed) |
| Indicative budget | €500,000 (unapproved) |
| Development partner | Available from March |
| Dependencies | CRM API, authentication, security approval |
| Management decision | Confirm scope, technical feasibility, funding, and ownership before detailed planning |

### Example Input

```text
Project: Customer Self-Service Portal

Business problem:
Customers contact support for address changes, invoice
copies, payment-status inquiries, and account updates.
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

**1. Project Overview**

Develop a Customer Self-Service Portal to reduce manual support requests and improve access to routine account services.

Expected value includes lower service workload, faster customer interactions, and improved digital accessibility.

**2. Project Objectives**

| Objective | Expected Outcome | Measurement | Owner |
|---|---|---|---|
| Reduce manual requests | Lower support workload | Request volume reduction; target TBD | Not defined |
| Improve digital access | Increased self-service adoption | Adoption rate; target TBD | Not defined |

**3. High-Level Scope**

| In Scope | Out of Scope | To Be Confirmed |
|---|---|---|
| No approved items | No confirmed exclusions | Address updates, invoice retrieval, payment-status visibility, account updates, mobile responsiveness, bank-detail changes, reporting dashboard |

**4. Key Deliverables**

| Deliverable | Description | Expected Outcome | Owner | Target Date |
|---|---|---|---|---|
| Customer portal (proposed) | Digital self-service interface | Reduced manual interactions | TBD | September, year TBD |
| Authentication integration (proposed) | Customer access capability | Secure access | TBD | TBD |

**5. Key Requirements**

| Category | Requirement | Status |
|---|---|---|
| Business | Reduce support workload | Identified; target undefined |
| Functional | Address updates, invoice retrieval | Proposed |
| Technical | CRM API integration | Feasibility unconfirmed |
| Data | Not yet defined | Missing |
| Security | Authentication approval | Required |
| Operational | Reporting dashboard | Proposed |
| Compliance | Not yet defined | Missing |

**6. Key Constraints**

| Constraint / Limitation | Category | Delivery Impact |
|---|---|---|
| €500,000 indicative budget | Budget | Funding requires approval |
| September target | Schedule | Delivery feasibility unconfirmed |
| Partner availability from March | Vendor | Influences delivery planning |

*These are preliminary planning limitations, not confirmed approved baselines.*

**7. Key Dependencies**

| Dependency | Type | Impact | Owner | Required By | Status |
|---|---|---|---|---|---|
| CRM API assessment | Technical | Integration effort uncertain | TBD | TBD | Open |
| Authentication approval | Security | Required for approved access design | TBD | TBD | Open |
| Funding approval | Financial | Delivery commitment unresolved | TBD | TBD | Open |

**8. Key Stakeholders**

| Stakeholder | Role | Interest | Decision Authority | Engagement Requirement |
|---|---|---|---|---|
| Customer Service | Business stakeholder | Reduce service workload | TBD | Validate customer needs |
| IT | Technical stakeholder | Integration feasibility | TBD | Assess architecture |
| Finance | Financial stakeholder | Funding | TBD | Confirm budget approval |
| Security | Security reviewer | Secure authentication | Authentication approval | Review access design |
| Marketing | Business stakeholder | Mobile experience | TBD | Clarify design needs |
| Operations | Operational stakeholder | Reporting | TBD | Define dashboard scope |

**9. High-Level Risks**

| Risk | Cause | Potential Impact | Initial Response | Owner |
|---|---|---|---|---|
| CRM integration delay | Legacy API limitations | Schedule and cost impact | Assess technical feasibility | TBD |
| Authentication redesign | Existing solution may be unsuitable | Additional effort | Conduct architecture review | TBD |
| Scope expansion | Unresolved feature requests | Budget and schedule impact | Confirm release scope | TBD |

**10. Assumptions**

| Assumption | Reason | Impact if Incorrect | Validation Required | Owner |
|---|---|---|---|---|
| Existing authentication can be reused | Preliminary IT input | Additional development effort | Technical assessment | TBD |
| Partner can start in March | Initial availability information | Schedule delay | Confirm availability | TBD |

**11. Delivery Approach**

The delivery methodology is not yet defined. Review scope uncertainty, technical dependencies, and governance requirements before selecting the approach.

**12. Open Questions**

| Question | Decision Owner | Priority |
|---|---|---|
| Is the €500,000 budget approved? | Finance / approver TBD | High |
| Is September a fixed launch deadline? | TBD | High |
| Can existing authentication be reused? | TBD | High |
| Are bank-detail changes included? | TBD | High |
| Is the dashboard part of the first release? | TBD | Medium |

**13. Recommended Next Steps**

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
4. **Governance:** Assign decision authority and approve the brief before detailed planning.

### Applied Quality Review

**Quality verdict: REVISE**

The preliminary brief identifies the business problem and principal uncertainties, but several planning inputs remain unconfirmed.

**Required corrections:** Validate funding, scope boundaries, technical feasibility, measurable objectives, and accountable decision-makers before using the brief as an approved planning reference.

---

**PM Governance:** Supports relevant PMI-aligned practices in project initiation, stakeholder engagement, scope clarification, uncertainty management, and value delivery.

The Project Brief supports early decision-making but does not replace an approved charter or scope baseline. Human validation is required before project commitments. Protect confidential personal, commercial, and technical information.

### Prompt Metadata

| Field | Value |
|---|---|
| Prompt ID | INIT-002 |
| Category | Project Initiation |
| Version | 1.0 |
| Status | Draft |
| Owner | Project Manager |
| Reviewer | Sponsor / Business Owner / PMO |
| Project Type | IT / Digital Transformation |
| Delivery Approach | Framework-neutral |
| Risk Level | Low |
| AI Model Tested | Not recorded |
| Last Reviewed | Not recorded |

### Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT project brief framework |
