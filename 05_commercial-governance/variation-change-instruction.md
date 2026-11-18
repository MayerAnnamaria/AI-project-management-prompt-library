# Variation / Change Instruction

**Prompt ID:** COMM-003 | **Category:** Commercial & Project Governance | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Convert proposed changes into clearly defined, commercially traceable instructions that support impact assessment, formal approval, and controlled implementation.

**Use case:** Manage additional functionality, integrations, data migration, infrastructure changes, or vendor services that may exceed the approved project scope or contractual boundaries.

Copy the prompt and replace the placeholders.

```text
ROLE

You are a Senior IT Project Manager and Commercial Manager
experienced in software delivery, contract administration,
supplier management, integrated change control, and governance.

CONTEXT

Project: [PROJECT NAME]
Contract / type: [CONTRACT NAME / TYPE]
Customer: [PARTY]
Supplier: [PARTY]
Project phase: [PHASE]
Delivery approach: [PREDICTIVE / AGILE / KANBAN / HYBRID]
Contract model: [FIXED PRICE / TIME & MATERIALS / OTHER]
Relevant clause: [VERIFIED CONTRACT WORDING / NOT PROVIDED]

Change ID: [ID]
Change status: [PROPOSED / UNDER ASSESSMENT / APPROVED]
Change type: [ADDITION / REDUCTION / MODIFICATION]
Requested by: [ROLE]
Approval authority: [VERIFIED ROLE / UNKNOWN]

CHANGE DETAILS

Business reason: [WHY CHANGE IS REQUIRED]
Original approved scope: [DETAILS]
Proposed change: [DESCRIPTION]
Included deliverables: [LIST]
Excluded deliverables: [LIST / NOT DEFINED]
Proposed acceptance criteria: [IF AVAILABLE]

Known impacts:
- Cost: [AMOUNT / TO BE ASSESSED]
- Schedule: [DETAILS / TO BE ASSESSED]
- Resources: [DETAILS]
- Technical: [DETAILS]
- Testing and security: [DETAILS]
- Operations and support: [DETAILS]
- Risks and dependencies: [LIST]

Supplier pricing required: [YES / NO]
Pricing deadline: [VERIFIED DATE / NOT DEFINED]
Supplier assessment deadline: [DATE / NOT DEFINED]
Implementation authorization: [STATUS]

TASK

Prepare a formal Change / Variation Instruction or,
if approval is pending, a Change Assessment Request.

STEP 1 — DEFINE THE CHANGE

1. Explain the business justification and expected value.
2. Compare the original scope with the proposed change.
3. Define included deliverables, exclusions, interfaces,
   responsibilities, and acceptance criteria.
4. Identify whether the change affects contractual
   boundaries or is normal delivery reprioritization.
5. Verify change authority and applicable contract clauses.

STEP 2 — ASSESS IMPACT

6. Request or review assessment of:
   - Functional and technical scope
   - Architecture and integrations
   - Cost and commercial assumptions
   - Schedule, milestones, and critical dependencies
   - Resources and supplier capacity
   - Testing and regression
   - Security and compliance
   - Documentation, training, and support
   - Delivery risks and operational readiness
7. Require itemized pricing where commercially necessary.
8. Distinguish verified impacts from supplier estimates.
9. Identify missing information and unrealistic assumptions.
10. Compare the supplier proposal against the defined change.

STEP 3 — GOVERNANCE AND APPROVAL

11. Identify the decision authority and required approvals.
12. Specify response deadlines and consequences of delay.
13. Recommend approval, revision, deferral, or rejection
    based on supported evidence.
14. Prevent unauthorized implementation before approval,
    unless the contract expressly permits instruction
    through a verified alternative process.
15. Define updates required after approval:
    - Scope and requirements baseline
    - Schedule and budget
    - Architecture and test plan
    - Risk and change registers
    - Release and vendor documentation

STEP 4 — IMPLEMENTATION CONTROL

16. Define implementation actions, owners, and deadlines.
17. Establish measurable acceptance conditions.
18. Track delivery, evidence, and formal change closure.

RULES

- Do not invent contractual rights, clause references,
  pricing provisions, deadlines, or approval authority.
- Do not describe a proposal as an approved instruction.
- Do not assume additional work is commercially authorized.
- Distinguish backlog reprioritization from formal scope change.
- Flag unverified assumptions and missing cost estimates.
- Do not confirm implementation until authority is established.

OUTPUT FORMAT

1. CHANGE SUMMARY

Change ID | Description | Business Reason |
Original Scope | Proposed Scope | Current Status

2. FORMAL CHANGE / ASSESSMENT REQUEST

Reference and Subject
Contract / Verified Authority
Purpose and Background
Detailed Change Scope
Exclusions and Boundaries
Supplier Assessment Required
Pricing and Schedule Requirements
Response Deadline
Approval Process and Next Steps

3. IMPACT ASSESSMENT

Area | Current Baseline | Proposed Impact |
Evidence / Assumption | Risk | Required Action

4. COMMERCIAL REVIEW

Cost Element | Quantity / Effort | Rate |
Estimated Total | Assumptions | Evidence

5. DEPENDENCIES AND RISKS

Risk / Dependency | Potential Impact |
Proposed Owner | Mitigation | Escalation Trigger

6. ACCEPTANCE CRITERIA

Deliverable | Proposed Criterion |
Verification Evidence | Acceptance Owner

7. APPROVAL AND CHANGE CONTROL

Decision Required | Approval Authority |
Current Status | Conditions | Deadline

8. IMPLEMENTATION AND BASELINE UPDATES

Action | Proposed Owner | Due Date |
Required Evidence | Completion Status

MANAGEMENT SUMMARY

- Business justification and project value
- Main cost, schedule, and technical exposure
- Outstanding supplier clarifications
- Approval recommendation
- Immediate management actions

Use concise Markdown tables.
Mark missing information as "To be confirmed".
Separate proposed changes from approved commitments.
```

---

## 2. Quality Check

Use this independent review before issuing or approving the change.

```text
QUALITY CHECK

Act as an independent Senior PMO and Commercial
Quality Assurance Manager.

Review the Change / Variation Instruction.

Verify:

1. Scope: Original and proposed requirements are clearly
   distinguished, with exclusions and acceptance criteria.
2. Contractual Basis: Clauses, instruction authority,
   and commercial rules are verified.
3. Impact: Cost, schedule, resources, technical design,
   testing, security, and support implications are covered.
4. Financial Accuracy: Pricing, effort, rates, and assumptions
   are supported without duplicated or unexplained charges.
5. Dependencies: Critical interfaces, supplier commitments,
   and implementation risks are identified.
6. Feasibility: Proposed schedules and recovery options
   are realistic and evidence-based.
7. Governance: Approval authority, decision status,
   and implementation controls are explicit.
8. Traceability: Approved changes can be linked
   to updated baselines and acceptance evidence.
9. Supplier Perspective: Potential exclusions, claims,
   and unsupported assumptions are challenged.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent approvals, contractual entitlements,
pricing assumptions, or implementation commitments.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Additional SAP Integration

**Scenario:** A company is implementing a CRM platform. During delivery, the Finance department requests an additional integration with SAP ERP to synchronize customer credit status.

The integration was not included in the approved project scope. The Project Manager must request a supplier impact assessment before submitting the proposed change for approval.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Implementation |
| Phase | Development / Integration |
| Delivery approach | Hybrid |
| Contract model | Fixed Price |
| Original integrations | Billing Platform and Customer Portal |
| Proposed change | CRM-to-SAP credit-status integration |
| Change ID | CR-014 |
| Change status | Proposed |
| Cost and schedule impact | Not yet assessed |
| Management objective | Establish scope, pricing, risks, and approval requirements |

### Example Input

```text
Project: CRM System Implementation
Contract: Software Implementation Agreement
Change ID: CR-014

Original scope:
CRM integration with Billing Platform
and Customer Portal.

Proposed change:
Additional outbound CRM-to-SAP integration
for approved customer credit status.

Business reason:
Finance requires credit-status information
to be synchronized with SAP ERP.

Requested deliverables:
- Interface design
- Field mapping
- API development
- Authentication configuration
- SIT and UAT support
- Technical documentation

Proposed exclusions:
- Changes to SAP credit-calculation logic
- Historical data migration
- Additional CRM user licences

Known cost impact:
Not yet assessed.

Known schedule impact:
Not yet assessed.

Supplier response required:
- Technical assessment
- Detailed pricing
- Resource estimate
- Milestone impact
- Dependencies and risks

Supplier response deadline:
15 September 2027.

Approval authority:
To be confirmed.

Implementation authorization:
Not approved.
```

### Example Output — Change Assessment Request

#### 1. Change Summary

| Field | Description |
|---|---|
| Change ID | CR-014 |
| Change | Additional CRM-to-SAP Integration |
| Business reason | Synchronize approved customer credit status |
| Original scope | Billing Platform and Customer Portal integrations |
| Proposed scope | Additional outbound SAP integration |
| Change status | Proposed — Under Assessment |
| Commercial impact | Not yet known |
| Implementation status | Not authorized |

#### 2. Formal Change / Assessment Request

**Subject: CR-014 — Request for Impact Assessment: Additional CRM-to-SAP Integration**

Dear Supplier Representative,

As part of the CRM implementation project, Finance has identified an additional requirement to synchronize approved customer credit status from CRM to SAP ERP.

The approved implementation scope currently covers integrations with the Billing Platform and Customer Portal. The proposed SAP integration is therefore being submitted for formal scope and commercial assessment.

The requested scope includes interface design, field mapping, API development, authentication configuration, integration and user acceptance testing support, and technical documentation.

The proposed change excludes modifications to SAP credit-calculation logic, historical data migration, and additional CRM user licences. These boundaries remain subject to confirmation during assessment.

Please provide by **15 September 2027**:

1. Technical solution and impact assessment.
2. Itemized commercial proposal with assumptions.
3. Resource requirements and availability.
4. Schedule and milestone impact.
5. Customer, supplier, and third-party dependencies.
6. Testing, security, and operational implications.
7. Key delivery risks and mitigation proposals.

This request is for assessment only. Implementation is not authorized until the applicable change-control requirements have been satisfied and approval has been confirmed.

Kind regards,  
[Authorized Project Representative]

#### 3. Impact Assessment

| Area | Current Baseline | Proposed Impact | Status |
|---|---|---|---|
| Scope | Two integrations | Additional SAP interface | Defined provisionally |
| Cost | Approved fixed-price scope | Additional effort likely | Assessment required |
| Schedule | Existing delivery plan | Potential development and testing impact | Unknown |
| Resources | Current supplier team | API / SAP expertise may be required | Unknown |
| Testing | Existing integration test plan | Additional SIT and UAT coverage | Assessment required |
| Security | Existing integration controls | New authentication and access considerations | Assessment required |
| Operations | Existing support scope | New interface monitoring and support | Assessment required |

#### 4. Commercial Review

| Cost Element | Required Supplier Detail | Current Status |
|---|---|---|
| Solution design | Estimated effort and rates | Not provided |
| API development | Estimated effort and rates | Not provided |
| SAP-side changes | Scope and ownership | Not confirmed |
| Integration testing | Effort and responsibilities | Not provided |
| Security configuration | Effort and dependencies | Not provided |
| Documentation | Effort and deliverables | Not provided |
| Support | Ongoing cost implications | Not confirmed |

**Commercial position:** No additional contract value can be established from the available information.

#### 5. Dependencies and Risks

| Risk / Dependency | Potential Impact | Proposed Owner | Response |
|---|---|---|---|
| SAP API availability | Integration delay | SAP Technical Lead | Confirm endpoint and access |
| Field mapping ambiguity | Development rework | Business Analyst | Approve mapping specification |
| Authentication requirements | Security or testing delays | Security Lead | Review integration design |
| Supplier resource availability | Schedule pressure | Supplier Delivery Lead | Confirm capacity |
| Regression impact | Existing CRM functionality affected | QA Lead | Extend regression test coverage |

These are potential exposures requiring technical validation.

#### 6. Acceptance Criteria

| Deliverable | Proposed Criterion | Evidence |
|---|---|---|
| Interface design | Approved integration specification | Design sign-off |
| Data mapping | Credit-status fields match approved mapping | Mapping review |
| API integration | Approved credit status transferred correctly | SIT evidence |
| Error handling | Failed transactions identified and recorded | Negative test results |
| Security | Required integration controls validated | Security review |
| Business acceptance | Finance validates agreed scenarios | UAT sign-off |

Acceptance criteria remain proposed until formally agreed.

#### 7. Approval and Change Control

| Field | Current Position |
|---|---|
| Change ID | CR-014 |
| Assessment status | Pending supplier response |
| Commercial approval | Not granted |
| Technical approval | Not granted |
| Implementation authorization | Not granted |
| Approval authority | To be confirmed |
| Supplier response deadline | 15 September 2027 |

**Decision required:** Determine whether the additional SAP integration should be approved after technical, financial, and schedule evaluation.

#### 8. Implementation and Baseline Updates

| Action | Proposed Owner | Timing |
|---|---|---|
| Submit change impact assessment | Supplier Delivery Lead | 15 September |
| Review technical feasibility | Solution Architect | After assessment |
| Validate business requirements | Finance / Business Analyst | Before approval |
| Evaluate commercial proposal | Commercial Manager | Before approval |
| Obtain change approval | Authorized Change Authority | Before implementation |
| Update scope and delivery baselines | Project Manager | After approval |
| Execute and verify integration | Supplier / QA | After authorization |
| Close change with acceptance evidence | Project Manager | After acceptance |

### Management Decisions

1. **Scope:** Confirm the interface requirements, exclusions, and business acceptance criteria.
2. **Commercial:** Obtain itemized pricing and validate whether the proposed costs are reasonable under the contract.
3. **Delivery:** Assess milestone, resource, testing, and security impacts before commitment.
4. **Governance:** Approve, defer, revise, or reject CR-014 through the authorized change-control process.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The assessment request describes the change, commercial boundaries, required supplier response, and approval controls. However, cost, schedule, resource availability, technical dependencies, and approval authority remain unconfirmed.

**Required corrections:**
- Verify the contract's change-control provisions.
- Confirm required SAP interfaces and responsibilities.
- Obtain supplier pricing and schedule assessment.
- Finalize measurable acceptance criteria.
- Confirm the authorized change approver.

**Approval blockers:** Missing cost and schedule assessments, incomplete technical dependency validation, and unconfirmed approval authority.

**Governance:** Supports PMI-aligned integrated change control, scope management, cost and schedule management, procurement, risk assessment, and project governance.

AI-assisted change documentation supports assessment and decision-making but does not authorize additional work or establish contractual entitlement. Material changes require appropriate technical, financial, commercial, and governance approval. Protect confidential contracts, supplier rates, architecture, security information, and customer data.
