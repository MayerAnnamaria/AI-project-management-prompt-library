# Scope Definition and Gap Review

**Prompt ID:** INIT-003 | **Category:** Project Initiation | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Define and validate project scope to reduce ambiguity, scope creep, rework, and delivery risk.

**Use case:** Draft or review scope boundaries, requirements, integrations, and responsibilities during project initiation, early planning, or major scope changes.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Business Analyst specializing
in software delivery, requirements management, scope definition,
stakeholder alignment, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Expected business value: [BENEFITS]
Project phase: [INITIATION / PLANNING]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Primary users: [USERS / BUSINESS UNITS]
Systems and integrations: [LIST]
Business processes: [LIST]
Known requirements: [LIST]
Dependencies: [LIST]
Constraints: [LIST]
Exclusions: [LIST]
Assumptions: [LIST]
Existing scope definition: [PASTE IF AVAILABLE]

TASK

Define the project scope and perform a structured gap review.

STEP 1 — SCOPE DEFINITION

1. Identify confirmed in-scope items, exclusions, and items
   requiring stakeholder confirmation.
2. Define key deliverables, capabilities, and system boundaries.
3. Identify business and technical responsibilities.
4. Document integrations, dependencies, and ownership.
5. Record assumptions and their potential delivery impacts.
6. Define measurable acceptance criteria where supported.

STEP 2 — SCOPE GAP REVIEW

7. Identify ambiguous, incomplete, or conflicting requirements.
8. Highlight missing deliverables, interfaces, and responsibilities.
9. Flag dependencies and integrations without accountable owners.
10. Identify scope items likely to generate change requests.
11. Identify missing or non-measurable acceptance criteria.
12. Review assumptions affecting schedule, cost, or feasibility.
13. Identify unclear boundaries between internal teams and vendors.
14. Highlight potential exclusions requiring stakeholder decisions.
15. Identify conflicts between business expectations and
    technical capabilities or boundaries.

Do not invent requirements, deliverables, or scope exclusions.
Distinguish confirmed scope from assumptions and proposals.
Flag vague terms such as "user-friendly", "fast", or "seamless".
Separate business outcomes from project deliverables.
Identify decisions requiring sponsor or governance approval.

OUTPUT FORMAT

PART A — SCOPE DEFINITION

1. IN SCOPE
   Scope Item | Description | Owner | Acceptance Criteria | Status

2. OUT OF SCOPE
   Exclusion | Rationale | Approval Status

3. TO BE CONFIRMED
   Item | Open Question | Decision Owner | Priority

4. KEY DELIVERABLES
   Deliverable | Description | Owner | Target Date

5. SYSTEM INTERFACES
   Interface | Source / Target | Responsibility | Dependency

6. BUSINESS RESPONSIBILITIES
   Activity | Business Owner | Responsibility

7. TECHNICAL RESPONSIBILITIES
   Component | Technical Owner | Responsibility

8. DEPENDENCIES
   Dependency | Impact | Owner | Required By | Status

9. ASSUMPTIONS
   Assumption | Impact if Incorrect | Validation Required | Owner

10. ACCEPTANCE CRITERIA
    Scope Item | Measurable Criterion | Validation Method | Status

PART B — SCOPE GAP REVIEW

GAP ANALYSIS
Gap / Issue | Location in Scope | Delivery Risk |
Potential Impact | Required Clarification | Proposed Owner | Priority

MANAGEMENT SUMMARY

1. Top five scope gaps requiring resolution
2. High-impact dependencies and ownership gaps
3. Potential scope creep and change-control concerns
4. Decisions requiring stakeholder approval
5. Recommended corrective actions

Use concise Markdown tables.
Mark missing information as "Not yet defined".
Label proposed owners, exclusions, and commitments as unconfirmed.
```

---

## 2. Quality Check

Apply this control after generating the scope definition and gap review.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the scope deliverables.

Verify:

1. Completeness: All 10 scope sections and the gap analysis
   address the available project information.
2. Accuracy: Confirmed scope, proposals, assumptions, and
   information gaps are clearly distinguished.
3. Clarity: Requirements and boundaries are specific,
   consistent, and unambiguous.
4. Ownership: Responsibilities, interfaces, and dependencies
   have confirmed or explicitly proposed owners.
5. Testability: Acceptance criteria are measurable or flagged
   for clarification.
6. Governance: Scope changes, exclusions, and approval
   requirements are identified.
7. Actionability: Recommended corrections are prioritized
   and feasible.

OUTPUT

Quality verdict: PASS / REVISE

Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [UNRESOLVED CRITICAL ITEMS]

Do not invent missing requirements, owners, dates, or approvals.
Flag conclusions requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Customer Self-Service Portal — Scope Definition and Gap Review

**Scenario:** A company plans to introduce a customer self-service portal to reduce manual support requests. Initial requirements identify core customer functions and integration needs, but acceptance criteria, technical ownership, and several scope boundaries remain unresolved.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Initiation / Early Planning |
| Business objective | Reduce manual customer-service workload |
| Systems | CRM, identity platform, billing system |
| Integrations | CRM API, billing API |
| Target | Before the Q4 campaign |
| Known exclusion | Online contract cancellation |
| Management decision | Confirm scope boundaries, integration ownership, and acceptance criteria before detailed planning |

### Example Input

```text
Project: Customer Self-Service Portal

Business objective:
Reduce manual customer-service workload.

Expected value:
Lower service costs and faster response times.

Known requirements:
- Customers can log in.
- Customers can update contact details.
- Customers can download invoices.
- Customers can view payment status.
- Portal should be mobile-friendly.

Systems:
CRM, Identity Platform, Billing System

Integrations:
CRM API, Billing API

Known constraint:
Go-live before the Q4 campaign.

Confirmed exclusion:
Online contract cancellation.

Open question:
Can customers update bank details online?
```

### Example Output — Scope Definition

#### 1. In Scope

No implementation scope has been formally approved.

| Proposed Scope Item | Description | Owner | Acceptance Criteria | Status |
|---|---|---|---|---|
| Customer authentication | Login using an identity platform | TBD | Authentication requirements TBD | Proposed |
| Contact-detail updates | Allow approved customer information changes | TBD | Fields and validation rules TBD | Proposed |
| Invoice retrieval | Access invoices through the billing system | TBD | Document access rules TBD | Proposed |
| Payment-status visibility | Display customer payment status | TBD | Data accuracy and refresh criteria TBD | Proposed |
| Responsive interface | Support mobile and desktop browsers | TBD | Supported devices and browsers TBD | Proposed |

#### 2. Out of Scope

| Exclusion | Rationale | Approval Status |
|---|---|---|
| Online contract cancellation | Explicitly excluded in project input | Stated exclusion; formal approval unconfirmed |

No other exclusions have been confirmed.

#### 3. To Be Confirmed

| Item | Open Question | Decision Owner | Priority |
|---|---|---|---|
| Bank-detail updates | Are customers permitted to change bank details? | TBD | High |
| Payment history | Is historical information required beyond current status? | TBD | Medium |
| Administration interface | Do support agents require additional functionality? | TBD | Medium |

#### 4. Key Deliverables

| Deliverable | Description | Owner | Target Date |
|---|---|---|---|
| Customer portal (proposed) | Customer-facing self-service application | TBD | Before Q4 campaign |
| CRM integration (proposed) | Exchange customer contact information | TBD | TBD |
| Billing integration (proposed) | Access invoice and payment information | TBD | TBD |

#### 5. System Interfaces

| Interface | Source / Target | Responsibility | Dependency |
|---|---|---|---|
| Customer identity | Portal ↔ Identity platform | TBD | Authentication capabilities |
| CRM API | Portal ↔ CRM | TBD | API access and data update rules |
| Billing API | Portal ↔ Billing system | TBD | Invoice and payment-status access |

#### 6. Business Responsibilities

| Activity | Business Owner | Responsibility |
|---|---|---|
| Scope approval | TBD | Confirm functional boundaries |
| Customer data rules | TBD | Define permitted account updates |
| Acceptance testing | TBD | Validate business requirements |

*Responsibilities are proposed; accountable owners require confirmation.*

#### 7. Technical Responsibilities

| Component | Technical Owner | Responsibility |
|---|---|---|
| Authentication integration | TBD | Validate identity-platform capabilities |
| CRM integration | TBD | Define API ownership and data exchange |
| Billing integration | TBD | Confirm invoice and payment-data access |
| Portal frontend | TBD | Implement approved responsive requirements |

#### 8. Dependencies

| Dependency | Impact | Owner | Required By | Status |
|---|---|---|---|---|
| Identity integration | Authentication feasibility | TBD | TBD | Unconfirmed |
| CRM API readiness | Contact-detail updates | TBD | TBD | Unconfirmed |
| Billing API readiness | Invoice and payment visibility | TBD | TBD | Unconfirmed |

#### 9. Assumptions

| Assumption | Impact if Incorrect | Validation Required | Owner |
|---|---|---|---|
| Identity platform supports portal login | Additional authentication development | Technical assessment | TBD |
| CRM API supports contact updates | Integration changes and delays | API capability review | TBD |
| Billing API provides required information | Additional development or integration effort | Data and API assessment | TBD |

#### 10. Acceptance Criteria

| Scope Item | Measurable Criterion | Validation Method | Status |
|---|---|---|---|
| Authentication | Successful and unsuccessful login scenarios defined and verified | Functional testing | Criteria TBD |
| Contact updates | Approved fields update correctly and persist | Integration testing | Criteria TBD |
| Invoice retrieval | Authorized customers can access permitted invoices | Functional and security testing | Criteria TBD |
| Payment status | Displayed status matches the agreed source of truth | Data validation | Criteria TBD |
| Responsive design | Portal meets agreed device and browser requirements | Cross-device testing | Criteria TBD |

*These are proposed validation approaches. Final measurable thresholds and acceptance criteria require stakeholder agreement.*

### Example Output — Scope Gap Review

| Gap / Issue | Location in Scope | Delivery Risk | Potential Impact | Required Clarification | Proposed Owner | Priority |
|---|---|---|---|---|---|---|
| "Mobile-friendly" undefined | Responsive interface | Inconsistent expectations | Rework and acceptance disputes | Define supported devices, browsers, and criteria | Product Owner | High |
| Bank-detail updates unresolved | To Be Confirmed | Scope uncertainty | Security and integration effort | Confirm business decision and security requirements | Business Owner | High |
| CRM API ownership unclear | System Interfaces | Unmanaged dependency | Integration delay | Assign interface owner and readiness date | Technical Lead | High |
| Performance criteria missing | Acceptance Criteria | Non-functional requirements gap | Performance issues at launch | Define response-time and load requirements | Solution Architect | High |
| Q4 deadline undefined | Constraints | Schedule ambiguity | Planning uncertainty | Confirm campaign date and delivery commitment | Project Sponsor | High |

### Management Decisions

1. **Scope:** Confirm the initial release capabilities, exclusions, and bank-detail update requirements.
2. **Ownership:** Assign accountable business and technical owners for system interfaces and dependencies.
3. **Acceptance:** Agree measurable functional, performance, security, and device-support criteria.
4. **Schedule:** Confirm the Q4 campaign deadline and assess integration feasibility before committing to delivery.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The proposed scope identifies the principal capabilities and integrations, but approval status, interface ownership, acceptance criteria, and the launch deadline remain insufficiently defined.

**Required corrections:** Confirm scope boundaries, assign owners, define measurable acceptance criteria, and validate dependencies and the delivery date.

**Approval blockers:** Unresolved critical scope decisions, missing ownership, and incomplete acceptance requirements.

**Governance:** This workflow supports relevant PMI-aligned practices in scope definition, requirements management, stakeholder alignment, risk identification, and change control. Scope approval remains with accountable stakeholders. Protect confidential project, commercial, personal, and security-sensitive information.
