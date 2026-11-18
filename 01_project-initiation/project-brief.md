# Project Brief

**Prompt ID:** INIT-002 | **Category:** Project Initiation | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Transform early project information into a structured brief that supports stakeholder alignment, scope clarification, and initial delivery planning.

**Use case:** Project initiation and discovery in IT, software development, and digital transformation initiatives.

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
Available information: [PASTE PROJECT NOTES / MEETING SUMMARY / REQUIREMENTS]

TASK

Create a professional project brief from the available information.

1. Summarize the business problem, proposed solution, expected value,
   and intended outcomes.
2. Identify project objectives and flag those without measurable criteria.
3. Classify scope as In Scope, Out of Scope, or To Be Confirmed.
4. Identify key deliverables, expected outcomes, owners, and dates.
5. Categorize business, functional, technical, data, security,
   operational, and compliance requirements.
6. Assess known schedule, budget, resource, technical, vendor,
   security, compliance, and operational constraints.
7. Identify critical dependencies and their delivery impacts.
8. Identify stakeholders, responsibilities, and decision authority.
9. Document initial project risks and proposed responses.
10. Record assumptions requiring validation.
11. Identify considerations relevant to the stated delivery approach.
12. Highlight unresolved questions, contradictions, unclear scope,
    missing ownership, and governance decisions.
13. Recommend the five highest-priority next steps.

Preserve confirmed facts and distinguish them from assumptions.
Do not invent missing information or infer unapproved scope.
Separate business outcomes from project deliverables.

OUTPUT FORMAT

Produce a structured Project Brief containing:

1. PROJECT OVERVIEW
   Business problem | Proposed Initiative | Expected Business Value

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
    Relevant methodology and delivery considerations

12. OPEN QUESTIONS
    Question | Decision Owner | Priority

13. RECOMMENDED NEXT STEPS
    Action | Priority | Proposed Owner | Expected Outcome

Use concise Markdown tables where appropriate.
Mark missing information as "Not yet defined".
Label proposed owners, dates, and actions as unconfirmed.
```

---

## 2. Quality Check

Apply the following quality control after generating the Project Brief.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Project Brief.

Verify:
1. Completeness: All 13 required sections are addressed.
2. Accuracy: Confirmed facts, assumptions, and gaps are distinguished.
3. Scope: Unapproved requirements are not presented as commitments.
4. Consistency: Objectives, scope, deliverables, and risks are aligned.
5. Governance: Ownership, dependencies, open decisions, and approvals
   are identified where supported.
6. Actionability: Next steps are specific, prioritized, and feasible.

OUTPUT
Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Corrective actions: [RECOMMENDED IMPROVEMENTS]

Do not invent missing facts, metrics, owners, or deadlines.
Flag decisions requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Customer Self-Service Portal — Project Initiation

**Scenario:** A company wants to reduce customer service workload through a digital self-service portal. Initial stakeholder discussions have identified business needs, technical dependencies, and an indicative budget, but several scope and governance decisions remain unresolved.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Initiation / Discovery |
| Target launch | September (year unconfirmed) |
| Indicative budget | €500,000 (not approved) |
| External vendor | Development partner available from March |
| Key dependencies | CRM API, authentication, security approval |
| Management decision | Clarify scope, feasibility, ownership, and funding before detailed planning |

### Example Input

```text
Project: Customer Self-Service Portal

Business problem:
Customers currently contact support for address changes,
invoice copies, payment-status inquiries, and account updates.
Customer Service reports excessive request volumes.

Business objective:
Reduce manual customer service workload through digital self-service.

Known information:
- Existing authentication may be reusable.
- CRM API may require modifications.
- Security approval is required for authentication.
- External development partner can start in March.
- Indicative budget: €500,000 (Finance approval pending).
- Target launch: September (year unconfirmed).
- Marketing requests mobile-responsive design.
- Operations requests a reporting dashboard.
- Online bank-detail changes are not yet agreed.
```

### Example Output — Project Brief

**1. Project Overview**

Develop a Customer Self-Service Portal to reduce manual support requests and improve digital access to routine customer services.

Expected business value includes lower support workload, improved service accessibility, and faster customer interactions.

**2. Project Objectives**

| Objective | Expected Outcome | Measurement | Owner |
|---|---|---|---|
| Reduce manual service requests | Lower support workload | Request volume reduction; target TBD | Not defined |
| Improve digital access | More self-service transactions | Portal adoption rate; target TBD | Not defined |

**3. High-Level Scope**

| In Scope | Out of Scope | To Be Confirmed |
|---|---|---|
| No items formally approved | No exclusions confirmed | Address updates, invoice retrieval, payment-status visibility, account updates, mobile-responsive design, bank-detail changes, reporting dashboard |

**4. Key Deliverables**

| Deliverable | Expected Outcome | Owner | Target Date |
|---|---|---|---|
| Customer portal (proposed) | Digital self-service capability | TBD | September, year TBD |
| Authentication integration (proposed) | Secure customer access | TBD | TBD |

**5. Key Requirements**

| Category | Requirement | Status |
|---|---|---|
| Business | Reduce service workload | Identified; target not defined |
| Functional | Address updates and invoice retrieval | Proposed |
| Technical | CRM API integration | Feasibility unconfirmed |
| Data | Not yet defined | Missing |
| Security | Authentication approval | Required |
| Operational | Reporting dashboard | Proposed |
| Compliance | Not yet defined | Missing |

**6. Key Constraints**

| Constraint / Limitation | Category | Delivery Impact |
|---|---|---|
| Indicative budget of €500,000 | Budget | Funding not confirmed |
| September target | Schedule | Feasibility requires assessment |
| External partner start in March | Vendor | Influences delivery planning |

**7. Key Dependencies**

| Dependency | Type | Impact | Owner | Required By | Status |
|---|---|---|---|---|---|
| CRM API assessment | Technical | Integration effort uncertain | TBD | TBD | Open |
| Security approval | Security | Authentication cannot be approved without review | TBD | TBD | Open |
| Finance approval | Financial | Funding commitment unresolved | TBD | TBD | Open |

**8. Key Stakeholders**

| Stakeholder | Role / Interest | Decision Authority | Engagement |
|---|---|---|---|
| Customer Service | Operational needs | TBD | Requirements validation |
| IT | Technical feasibility | TBD | Architecture assessment |
| Finance | Funding | TBD | Budget confirmation |
| Security | Authentication review | Security approval | Security assessment |
| Marketing | Mobile experience | TBD | Design consultation |
| Operations | Reporting needs | TBD | Scope clarification |

**9. High-Level Risks**

| Risk | Cause | Potential Impact | Initial Response | Owner |
|---|---|---|---|---|
| CRM integration delay | Legacy API limitations | Schedule and cost impact | Technical assessment | TBD |
| Authentication issues | Reuse feasibility unknown | Security or delivery delay | Architecture and security review | TBD |
| Scope expansion | Unresolved feature requests | Additional effort and cost | Agree scope baseline | TBD |

**10. Assumptions**

| Assumption | Reason | Impact if Incorrect | Validation | Owner |
|---|---|---|---|---|
| Existing login can be reused | Preliminary IT input | Additional development effort | Technical assessment | TBD |
| Vendor can begin in March | Initial availability information | Schedule delay | Confirm commitment | TBD |

**11. Delivery Approach**

The delivery methodology has not been confirmed. Assess technical dependencies, scope uncertainty, and governance requirements before selecting an appropriate approach.

**12. Open Questions**

| Question | Decision Owner | Priority |
|---|---|---|
| Is the €500,000 budget approved? | Finance / accountable approver TBD | High |
| Is September a fixed deadline? | TBD | High |
| Can the existing authentication be reused? | TBD | High |
| Are bank-detail changes included? | TBD | High |
| Is the dashboard part of the initial release? | TBD | Medium |

**13. Recommended Next Steps**

| Action | Priority | Proposed Owner | Expected Outcome |
|---|---|---|---|
| Confirm funding | High | Finance | Approved funding position |
| Assess CRM and authentication feasibility | High | IT Lead | Technical feasibility findings |
| Agree initial scope | High | Business Owner | Defined scope boundaries |
| Confirm delivery timeline | High | Project Manager | Feasible initial schedule |
| Establish project governance | High | Project Sponsor | Confirmed decision authority |

### Management Decisions

1. **Funding:** Confirm the available budget before committing to delivery.
2. **Scope:** Agree on the initial release features and deferred functionality.
3. **Technical feasibility:** Validate CRM integration and authentication dependencies.
4. **Governance:** Confirm accountable decision-makers and approve the project brief before detailed planning.

### Applied Quality Review

**Quality verdict: REVISE**

The example brief identifies the key business needs and delivery uncertainties. However, scope approval, funding, measurable objectives, and decision ownership remain unresolved.

**Required corrections:** Confirm scope boundaries, budget approval, delivery feasibility, and accountable stakeholders before treating the brief as an approved planning baseline.

---

**PM Governance:** This prompt supports relevant PMI-aligned practices in project initiation, stakeholder engagement, scope definition, uncertainty management, and value delivery.

The Project Brief is a preliminary decision-support artifact, not an approved project charter or scope baseline. Human validation is required before project commitments are established. Anonymize confidential commercial, personal, and security-sensitive information.

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
