# Procurement Plan

**Prompt ID:** PLAN-005 | **Category:** Project Planning | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Plan and control external IT procurement to ensure supplier capability, cost transparency, delivery readiness, and governance.

**Use case:** Select software vendors, implementation partners, or specialist IT services when internal capacity or expertise is insufficient, or when new technology must be acquired.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in IT procurement,
vendor management, software delivery, commercial governance,
and third-party risk management.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Project budget: [AMOUNT / RANGE]
Target completion: [DATE]

External services required: [LIST]
Software / licences: [LIST]
Cloud / infrastructure: [LIST]
Implementation partners / consultants: [LIST]
Existing vendors: [LIST]

Procurement policies: [RULES]
Contract constraints: [LIST]
Required approvals: [ROLES]
Security / compliance requirements: [LIST]
Known vendor risks: [LIST]
Local / organisational requirements: [LIST]

TASK

Create a professional Procurement Plan for the project.

1. Define procurement objectives aligned with scope, budget,
   quality, and delivery requirements.
2. Identify required procurement packages and justify
   external sourcing versus internal delivery.
3. Recommend appropriate procurement methods, subject to
   organisational rules and approval.
4. Establish objective supplier evaluation criteria,
   qualification requirements, and supporting evidence.
5. Develop procurement milestones, lead times, and dependencies
   linked to project delivery.
6. Assess commercial models, payment terms, acceptance criteria,
   SLAs, change control, intellectual property, and exit provisions.
7. Identify security, data protection, regulatory, and
   supplier qualification requirements.
8. Define procurement approval authorities and governance pathways.
9. Establish vendor performance measures, review cadence,
   escalation procedures, and accountable owners.
10. Assess procurement risks, including supplier capacity,
    lock-in, cost escalation, and contractual dependencies.
11. Identify missing packages, unrealistic timelines,
    unclear ownership, or commercial-model conflicts.
12. Recommend prioritized procurement actions and decisions.

Adapt procurement practices to the delivery approach.
Do not invent vendor quotations, approval thresholds,
contract terms, or supplier qualifications.
Distinguish confirmed requirements from recommendations.

OUTPUT FORMAT

1. PROCUREMENT OBJECTIVES
   Objective | Business Justification | Expected Outcome

2. PROCUREMENT STRATEGY
   Procurement Area | Proposed Method | Rationale |
   Key Constraint | Approval Required

3. PROCUREMENT PACKAGES
   Package | Requirement | Method | Estimated Value |
   Required By | Owner | Approval

4. SUPPLIER EVALUATION
   Criterion | Weight (If Approved) | Evidence Required |
   Evaluation Method

5. SUPPLIER QUALIFICATION
   Requirement | Evidence | Verification Owner | Status

6. PROCUREMENT TIMELINE
   Stage | Target Date | Dependency | Owner | Status

7. COMMERCIAL & CONTRACT CONSIDERATIONS
   Topic | Proposed Approach | Risk / Dependency |
   Required Review

8. GOVERNANCE & APPROVAL
   Decision | Approval Authority | Required Evidence |
   Decision Deadline

9. VENDOR PERFORMANCE
   KPI | Measurement | Target | Review Frequency | Owner

10. PROCUREMENT RISKS
    Risk | Cause | Probability | Impact |
    Mitigation | Owner

11. RECOMMENDED ACTIONS
    Action | Priority | Proposed Owner |
    Required By | Expected Outcome

MANAGEMENT SUMMARY

- Critical procurement and delivery dependencies
- Supplier selection and qualification gaps
- Commercial, security, and contractual risks
- Decisions and approvals required

Use concise Markdown tables.
Mark unknown values as "Not yet defined".
Label proposed arrangements as requiring confirmation.
```

---

## 2. Quality Check

Apply this control after generating the Procurement Plan.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Procurement Plan.

Verify:

1. Completeness: All 11 procurement components are addressed,
   including potential missing procurement packages.
2. Alignment: Procurement requirements support project scope,
   budget, delivery approach, and schedule.
3. Supplier Evaluation: Criteria are objective, evidence-based,
   and consistent with organisational procurement rules.
4. Feasibility: Lead times, supplier capacity, dependencies,
   and mobilisation requirements are realistic or flagged.
5. Commercial & Security: Contract models, acceptance criteria,
   service levels, security, compliance, and exit arrangements
   are adequately considered.
6. Governance: Evaluation ownership, approval authority,
   vendor oversight, and escalation requirements are identified.
7. Actionability: Risks and gaps have prioritized corrective
   actions and proposed owners.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]

Do not invent suppliers, prices, contractual terms,
qualification evidence, or approval decisions.
Flag matters requiring Procurement, Legal, Finance,
Security, or stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development Project — External Development Partner Procurement

**Scenario:** A company is expanding an internal web application with new customer reporting functionality. The existing development team lacks sufficient capacity to meet the target release, so the Project Manager must evaluate external development support and establish procurement requirements before onboarding a supplier.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Planning |
| Delivery approach | Scrum |
| Target release | End of Q3 2027 |
| Internal team | 3 Developers, 1 QA Engineer, 1 Product Owner |
| Procurement need | External frontend and backend development capacity |
| Budget | €120,000 indicative procurement allocation |
| Required reviews | Procurement, Finance, IT Security, Legal |
| Key constraint | Internal development capacity is insufficient |
| Management decision | Select an appropriate sourcing and commercial approach before supplier onboarding |

### Example Input

```text
Project: Web Application Reporting Enhancement

Business objective:
Deliver additional reporting capabilities to existing users.

Delivery approach: Scrum
Target release: End of Q3 2027

Internal team:
- 3 Developers
- 1 QA Engineer
- 1 Product Owner

Known limitation:
Internal developers cannot complete all planned work
within the target release window.

Procurement requirements:
- 1 external frontend developer
- 1 external backend developer
- Integration with the existing development team
- Code quality and security requirements
- Vendor participation in agreed delivery activities

Indicative procurement allocation: €120,000

Required approvals:
Procurement, Finance, IT Security, Legal

Known risks:
- Supplier onboarding delay
- Insufficient technical capability
- Vendor resource replacement
- Unclear responsibilities between internal and external teams
- Scope changes during development

Contract constraints:
Not yet defined.

Existing supplier framework:
Not yet confirmed.
```

### Example Output — Procurement Plan

#### 1. Procurement Objectives

| Objective | Business Justification | Expected Outcome |
|---|---|---|
| Secure external development capacity | Internal capacity shortfall | Additional frontend and backend capability |
| Protect release schedule | Q3 delivery commitment | Improved delivery capacity |
| Maintain technical quality | Shared application codebase | Consistent coding and security standards |
| Establish commercial control | €120,000 indicative allocation | Transparent supplier costs and approvals |

#### 2. Procurement Strategy

| Procurement Area | Proposed Method | Rationale | Key Constraint | Approval Required |
|---|---|---|---|---|
| External development | Existing framework or competitive sourcing | Access qualified specialists | Limited onboarding time | Procurement |
| Commercial model | Time & Materials with approved capacity limits | Supports evolving Scrum priorities | Budget control | Finance / Procurement |
| Technical qualification | Capability assessment | Validate relevant development skills | Existing architecture | IT Lead |
| Security qualification | Supplier security review | Protect application and data | Access requirements | IT Security |

*The preferred sourcing route and contract model require validation against organisational procurement policies.*

#### 3. Procurement Packages

| Package | Requirement | Method | Estimated Value | Required By | Proposed Owner | Approval |
|---|---|---|---|---|---|---|
| Frontend development | 1 external developer | To be confirmed | TBD | Before assigned development work | Procurement Lead | Pending |
| Backend development | 1 external developer | To be confirmed | TBD | Before assigned development work | Procurement Lead | Pending |
| Supplier onboarding | Access, agreements, technical induction | Internal approval process | TBD | Before supplier access | IT Lead | Pending |

**Budget constraint:** €120,000 indicative allocation. Supplier rates, effort, and total committed costs remain unconfirmed.

#### 4. Supplier Evaluation

| Criterion | Weight | Evidence Required | Evaluation Method |
|---|---|---|---|
| Technical capability | Not approved | Relevant technical experience | Technical interview |
| Relevant delivery experience | Not approved | Reference projects | Reference review |
| Resource availability | Not approved | Named capacity and start dates | Supplier confirmation |
| Commercial proposal | Not approved | Rate card and cost forecast | Commercial evaluation |
| Security and compliance | Not approved | Security controls and policies | Security assessment |
| Team integration | Not approved | Collaboration approach | Delivery review |

Evaluation weights must be agreed before supplier scoring.

#### 5. Supplier Qualification

| Requirement | Evidence | Proposed Verification Owner | Status |
|---|---|---|---|
| Relevant development skills | Technical assessment | IT Lead | Pending |
| Resource availability | Supplier confirmation | Vendor Manager | Pending |
| Security controls | Security questionnaire / evidence | Security Lead | Pending |
| Confidentiality requirements | Approved agreements | Legal / Procurement | Pending |
| Financial and commercial suitability | Supplier due diligence | Procurement | Pending |

#### 6. Procurement Timeline

| Stage | Target Date | Dependency | Proposed Owner | Status |
|---|---|---|---|---|
| Confirm development scope | TBD | Product backlog and technical assessment | Product Owner | Open |
| Approve procurement strategy | TBD | Procurement policy review | Procurement | Open |
| Obtain supplier proposals | TBD | Approved sourcing method | Procurement | Open |
| Complete technical evaluation | TBD | Supplier submissions | IT Lead | Open |
| Complete security and legal review | TBD | Supplier documentation | Security / Legal | Open |
| Contract approval and signature | TBD | Financial and legal authorization | Procurement | Open |
| Supplier onboarding | TBD | Executed agreement and access approvals | IT Lead | Open |

**Delivery dependency:** Supplier mobilization must be completed before externally assigned development activities begin.

#### 7. Commercial & Contract Considerations

| Topic | Proposed Approach | Risk / Dependency | Required Review |
|---|---|---|---|
| Pricing model | Time & Materials with capacity limits | Cost overruns | Procurement / Finance |
| Deliverable acceptance | Agreed acceptance criteria and Definition of Done | Disputed completion | Product Owner / IT Lead |
| Resource continuity | Replacement and notice provisions | Knowledge loss | Procurement / Legal |
| Intellectual property | Confirm ownership and usage rights | Code ownership uncertainty | Legal |
| Confidentiality | Approved contractual protections | Sensitive information exposure | Legal / Security |
| Change control | Approved backlog and commercial change procedures | Scope and cost escalation | Project Manager / Procurement |
| Exit and knowledge transfer | Defined handover obligations | Supplier dependency | IT Lead / Legal |

Contract terms require qualified Legal and Procurement review.

#### 8. Governance & Approval

| Decision | Approval Authority | Required Evidence | Decision Deadline |
|---|---|---|---|
| Procurement method | Procurement — subject to policy | Sourcing justification | TBD |
| Supplier selection | Authorized selection body — TBD | Evaluation results | TBD |
| Financial commitment | Authorized budget approver — TBD | Cost forecast and allocation | TBD |
| Security clearance | IT Security | Security assessment | Before access |
| Contract execution | Authorized signatories — TBD | Approved contractual terms | Before onboarding |

#### 9. Vendor Performance

| KPI | Measurement | Target | Review Frequency | Proposed Owner |
|---|---|---|---|---|
| Delivery predictability | Completed vs. planned agreed work | TBD | Each sprint | Delivery Lead |
| Defect quality | Defects attributable to delivered changes | TBD | Each sprint | QA Lead |
| Resource continuity | Changes to assigned personnel | TBD | Monthly (proposed) | Vendor Manager |
| Budget performance | Actual vs. forecast supplier cost | Within approved limits | Monthly (proposed) | Project Manager |
| Acceptance performance | Accepted vs. submitted deliverables | TBD | Each sprint | Product Owner |

Performance targets require agreement before supplier onboarding.

#### 10. Procurement Risks

| Risk | Cause | Probability | Impact | Mitigation | Proposed Owner |
|---|---|---|---|---|---|
| Supplier onboarding delay | Procurement and access lead times | Not assessed | Release schedule | Start approvals early | Project Manager |
| Insufficient technical capability | Inadequate qualification | Not assessed | Rework and quality | Technical assessment | IT Lead |
| Vendor resource replacement | Supplier staffing changes | Not assessed | Delivery continuity | Contractual continuity provisions | Vendor Manager |
| Commercial overrun | Variable effort and changing priorities | Not assessed | Budget | Forecast and capacity controls | Project Manager |
| Unclear code ownership | Incomplete contract terms | Not assessed | Legal and operational risk | Legal review | Procurement / Legal |

#### 11. Recommended Actions

| Action | Priority | Proposed Owner | Required By | Expected Outcome |
|---|---|---|---|---|
| Confirm development capacity gap | High | IT Lead | Before sourcing | Validated procurement requirement |
| Approve procurement strategy | High | Procurement | Before supplier engagement | Compliant sourcing approach |
| Define supplier evaluation criteria | High | Procurement / IT Lead | Before evaluation | Objective selection process |
| Validate commercial allocation | High | Finance | Before contract approval | Confirmed budget limits |
| Complete security and contractual reviews | High | Security / Legal | Before onboarding | Approved supplier access and agreement |

### Management Decisions

1. **Sourcing strategy:** Determine whether an existing supplier agreement or competitive procurement is the most suitable approach.
2. **Commercial model:** Approve a contract structure that supports iterative delivery while controlling budget exposure.
3. **Supplier qualification:** Confirm technical capability, security suitability, and resource availability before selection.
4. **Governance:** Establish approval authority, supplier performance expectations, and exit arrangements before onboarding.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The procurement requirements and delivery dependencies are identified, but supplier pricing, selection criteria, contract terms, and approval authority remain unconfirmed.

**Required corrections:**
- Confirm sourcing requirements and approved procurement method.
- Obtain supplier rates and validate the €120,000 allocation.
- Approve supplier evaluation criteria and qualification requirements.
- Establish contractual, security, and onboarding approvals.
- Confirm delivery ownership and vendor performance expectations.

**Approval blockers:** Unconfirmed supplier costs, incomplete commercial terms, and unresolved approval responsibilities.

**Governance:** This prompt supports relevant PMI-aligned practices in procurement planning, financial management, stakeholder coordination, risk management, and supplier governance.

The Procurement Plan is a management decision-support artifact. Formal supplier selection, contractual commitments, and financial approvals remain with authorized Procurement, Finance, Legal, Security, and project stakeholders. Protect confidential vendor pricing, proposals, contracts, and commercially sensitive information.
