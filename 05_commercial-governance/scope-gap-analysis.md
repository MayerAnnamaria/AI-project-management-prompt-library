# Scope Gap Analysis

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** COMM-004 | **Category:** Commercial & Project Governance

---


## 1. Ready-to-Use Prompt

**Purpose:** Identify missing, ambiguous, or commercially exposed requirements before they create delivery delays, change requests, acceptance disputes, or unplanned costs.

**Use case:** Review Statements of Work (SOWs), requirements specifications, RFPs, and supplier scope documents before approval, contract signature, vendor mobilization, or major change decisions.

Copy the prompt and replace the placeholders.

```text
ROLE

You are a Senior IT Project Manager and Business / Commercial
Analyst specializing in requirements management, software
implementation, vendor governance, scope control, and procurement.

CONTEXT

Project: [PROJECT NAME]
Document type: [SOW / RFP / REQUIREMENTS / CONTRACT SCOPE]
Project phase: [PHASE]
Business objective: [OBJECTIVE]
Delivery approach: [PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]
Supplier model: [INTERNAL / EXTERNAL / MULTI-VENDOR]
Contract model: [FIXED PRICE / TIME & MATERIALS / OTHER]
Known constraints: [LIST]
Approved scope boundaries: [IF AVAILABLE]

DOCUMENT TO REVIEW

[PASTE PROJECT SCOPE OR REQUIREMENTS]

TASK

Identify scope gaps that may create delivery, technical,
commercial, or acceptance risks.

STEP 1 — REQUIREMENTS QUALITY

1. Identify vague, incomplete, contradictory, or
   untestable requirements.
2. Evaluate clarity, necessity, feasibility,
   measurability, and traceability.
3. Highlight open-ended commitments such as
   "all necessary integrations" or "support as required".
4. Identify missing functional and non-functional
   requirements relevant to the project.
5. Distinguish confirmed omissions from areas requiring
   further stakeholder clarification.

STEP 2 — RESPONSIBILITIES AND DEPENDENCIES

6. Identify unclear Customer, Supplier, and third-party
   responsibilities.
7. Review interface ownership, API access, environments,
   test data, security, and external dependencies.
8. Identify hidden assumptions and missing exclusions.
9. Assess potential impact if critical dependencies
   or assumptions prove incorrect.

STEP 3 — ACCEPTANCE AND OPERATIONS

10. Review whether deliverables have measurable
    acceptance criteria, evidence, and approvers.
11. Identify missing testing, data migration,
    performance, security, privacy, and compliance
    requirements where relevant.
12. Review deployment, documentation, support,
    monitoring, recovery, and operational handover.

STEP 4 — COMMERCIAL AND DELIVERY RISK

13. Assess each gap from both Customer and Supplier
    perspectives.
14. Identify potential change requests, cost exposure,
    schedule impact, and acceptance disputes.
15. Assign a proposed priority:
    - Critical: Potential major delivery, security,
      commercial, or acceptance failure.
    - High: Material ambiguity requiring resolution
      before commitment.
    - Medium: Important clarification with manageable impact.
    - Low: Minor improvement.
16. Recommend specific wording, clarification questions,
    ownership, and required evidence.
17. Identify gaps that should block scope approval
    until appropriately resolved.

For Agile delivery, distinguish flexible backlog details
from contractual and commercial boundaries.

Do not invent system requirements, acceptance thresholds,
contractual commitments, or stakeholder approvals.

Treat suggested wording as a proposal requiring validation.

OUTPUT FORMAT

1. EXECUTIVE SCOPE ASSESSMENT

Overall Completeness | Critical Gaps |
Commercial Exposure | Approval Readiness

2. SCOPE GAP REGISTER

Gap ID | Requirement / Document Reference |
Gap / Ambiguity | Customer Risk | Supplier Risk |
Delivery Impact | Priority | Recommended Fix

3. REQUIREMENTS QUALITY REVIEW

Requirement | Quality Issue | Why It Matters |
Suggested Clarification | Validation Required

4. INTERFACE AND RESPONSIBILITY MATRIX

Interface / Dependency | Customer Responsibility |
Supplier Responsibility | Third Party |
Acceptance Owner | Missing Decision

5. ACCEPTANCE CRITERIA REVIEW

Deliverable | Current Criterion | Gap |
Proposed Measurable Criterion |
Required Evidence | Approver

6. ASSUMPTIONS AND EXCLUSIONS

Item | Type | Current Position |
Validation Owner | Risk if Incorrect

7. TECHNICAL AND OPERATIONAL GAPS

Area | Missing / Ambiguous Requirement |
Potential Impact | Required Clarification

8. RECOMMENDED SCOPE CORRECTIONS

Priority | Proposed Correction |
Proposed Owner | Required Evidence |
Approval Dependency

9. MANAGEMENT SUMMARY

- Highest-priority scope gaps
- Main Customer and Supplier exposure
- Decisions needed before commitment
- Recommended scope approval status

Approval status:
READY / READY WITH CONDITIONS / NOT READY

Use concise Markdown tables.
Reference source wording where available.
Mark unknown information as "Requires clarification".
```

---

## 2. Quality Check

Use this independent audit before approving the revised scope.

```text
QUALITY CHECK

Act as an independent Senior QA and Commercial Assurance Manager.

Review the Scope Gap Analysis against the original document.

Verify:

1. Accuracy: Every finding is traceable to source wording
   or clearly identified as a potential omission.
2. Requirements: Ambiguous, contradictory, and untestable
   statements are identified.
3. Completeness: Relevant functional, technical,
   security, data, and operational areas are covered.
4. Responsibilities: Customer, Supplier, and third-party
   ownership gaps are visible.
5. Acceptance: Proposed criteria are measurable,
   feasible, and require stakeholder agreement.
6. Commercial Risk: Exposure is assessed fairly
   for both Customer and Supplier.
7. Prioritization: Severity reflects actual project
   context, not generic assumptions.
8. Actionability: Each material gap has a practical
   clarification or correction.
9. Governance: Critical approval blockers and
   required decision authorities are identified.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent missing requirements, contract terms,
acceptance thresholds, or approved scope decisions.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Pre-Contract Scope Review

**Scenario:** A company is preparing to engage a software supplier to implement a CRM system. The draft Statement of Work describes required integrations, data migration, reporting, and training, but several commitments are too general to establish reliable delivery and commercial boundaries.

The Project Manager must identify gaps before contract signature.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM Implementation |
| Phase | Procurement / Contracting |
| Document | Draft Statement of Work |
| Delivery approach | Hybrid |
| Supplier model | External vendor |
| Commercial model | Fixed price |
| Main concern | Ambiguous scope and acceptance conditions |
| Management objective | Reduce change disputes and delivery uncertainty |

### Example Input

```text
Project: CRM Implementation

Document: Draft Statement of Work
Contract model: Fixed Price
Supplier: External CRM Implementation Vendor

Scope extract:

"The Supplier shall implement a CRM solution
integrated with the ERP and other relevant systems.

The solution shall provide fast customer searches
and flexible reporting capabilities.

The Supplier shall migrate all necessary
customer data from the legacy system.

The solution must comply with applicable
security requirements.

The Supplier shall provide user training
and technical documentation.

The implementation must be completed
by 30 September 2027."

Known information:
- ERP integration required.
- Other interfaces not yet listed.
- Legacy data quality not assessed.
- Business acceptance criteria not finalized.
- Support arrangements not defined.
```

### Example Output — Scope Gap Analysis

#### 1. Executive Scope Assessment

| Area | Assessment |
|---|---|
| Overall completeness | Insufficient for fixed-price commitment |
| Critical gaps | Integration scope, migration boundaries, acceptance criteria |
| Commercial exposure | High |
| Approval readiness | Not Ready |
| Main recommendation | Clarify deliverables, responsibilities, and measurable acceptance conditions before signature |

#### 2. Scope Gap Register

| ID | Gap / Ambiguity | Customer Risk | Supplier Risk | Priority | Recommended Fix |
|---|---|---|---|---|---|
| G-01 | "Other relevant systems" undefined | Required integrations may be excluded | Open-ended integration expectations | High | List systems and interfaces |
| G-02 | "Fast customer searches" unmeasured | Performance may not meet business needs | Disputes over acceptable response time | High | Agree performance criteria |
| G-03 | "Flexible reporting" undefined | Required reports may be missing | Uncontrolled report requests | High | Define reporting scope |
| G-04 | "All necessary customer data" undefined | Incomplete migration | Unexpected cleansing and migration effort | Critical | Define datasets and responsibilities |
| G-05 | Security requirements unspecified | Security expectations may be unmet | Undefined compliance effort | High | Reference approved security baseline |
| G-06 | Training and documentation undefined | Inadequate business readiness | Unclear delivery quantities | Medium | Specify required outputs |
| G-07 | No operational support scope | Unclear post-launch ownership | Unplanned support expectations | High | Define handover and support model |
| G-08 | Acceptance criteria missing | Disputes over completion | Payment / approval uncertainty | Critical | Establish acceptance matrix |

Priorities are illustrative and must be confirmed against the project's actual risk criteria.

#### 3. Requirements Quality Review

| Requirement | Quality Issue | Suggested Clarification |
|---|---|---|
| Fast customer searches | Not measurable | Define agreed response time, test load, and data volume |
| Flexible reporting | Unbounded functionality | List required reports and configuration options |
| All necessary customer data | Undefined scope | Identify entities, history, records, and exclusions |
| Applicable security requirements | Missing reference baseline | Specify approved security controls and review process |
| Technical documentation | Undefined deliverables | List documents, required content, and approval criteria |

Any proposed technical threshold must be agreed by the appropriate stakeholders rather than generated as an assumed requirement.

#### 4. Interface and Responsibility Matrix

| Interface / Dependency | Customer | Supplier | Third Party | Missing Decision |
|---|---|---|---|---|
| ERP integration | Responsibilities TBD | Responsibilities TBD | ERP provider, if applicable | API ownership and test access |
| Additional enterprise systems | Define candidate systems | Assess integration feasibility | TBD | Confirm scope and interface count |
| Legacy data migration | Responsibilities TBD | Responsibilities TBD | Legacy provider, if applicable | Extraction, cleansing, and reconciliation ownership |
| Security integration | Define security requirements | Confirm implementation responsibilities | Identity provider, if applicable | Authentication and approval responsibilities |

These are clarification areas, not confirmed contractual allocations.

#### 5. Acceptance Criteria Review

| Deliverable | Current Criterion | Gap | Required Clarification |
|---|---|---|---|
| ERP integration | Not defined | No agreed success test | Specify integration scenarios and evidence |
| Customer search | "Fast" | No performance threshold | Define measurable acceptance target |
| Data migration | "All necessary data" | No completeness or accuracy criteria | Agree reconciliation measures |
| Reporting | "Flexible reporting" | No report catalogue | Define report inventory and acceptance |
| Security | "Applicable requirements" | No approval standard | Confirm applicable security checks |
| User training | Training provided | No measurable delivery scope | Define audience, sessions, and materials |

Acceptance owners and criteria remain to be agreed.

#### 6. Assumptions and Exclusions

| Item | Type | Current Position | Risk if Incorrect |
|---|---|---|---|
| Legacy source data is usable | Assumption | Not validated | Unexpected cleansing and rework |
| ERP API is available | Assumption | Not confirmed | Integration delay |
| Additional integrations | Scope boundary | Undefined | Commercial scope expansion |
| Historical data cleansing | Exclusion candidate | Not specified | Responsibility dispute |
| Post-go-live support | Scope boundary | Not defined | Unplanned service commitments |

#### 7. Technical and Operational Gaps

| Area | Gap | Potential Impact | Required Clarification |
|---|---|---|---|
| Performance | No load conditions | Acceptance uncertainty | Agree performance test profile |
| Data | No migration inventory | Incomplete scope estimates | Define data sources and quality ownership |
| Security | No security baseline | Approval and compliance risk | Confirm security requirements |
| Environments | No environment responsibilities | Testing delays | Define provisioning and access |
| Operations | No support model | Handover failure | Agree service ownership |
| Documentation | No deliverables inventory | Incomplete knowledge transfer | Define mandatory documents |

#### 8. Recommended Scope Corrections

| Priority | Action | Proposed Owner | Evidence Required |
|---|---|---|---|
| Critical | Confirm complete migration scope and data ownership | Business / Data Lead | Approved data inventory |
| Critical | Define measurable acceptance criteria | Business Analyst / QA Lead | Acceptance matrix |
| High | Finalize integration catalogue | Solution Architect | Approved interface list |
| High | Approve non-functional requirements | Architecture / Security | Requirements baseline |
| High | Define operational handover | Service Owner | Support and transition plan |
| Medium | Specify training and documentation | Business Owner | Deliverables checklist |

### Management Decisions

1. **Scope approval:** Do not finalize the fixed-price scope until critical ambiguities are resolved or formally addressed.
2. **Commercial boundaries:** Confirm integration quantities, migration responsibilities, support obligations, and explicit exclusions.
3. **Acceptance:** Establish measurable criteria and authorized acceptance owners for key deliverables.
4. **Change control:** Ensure that requirements introduced after the agreed baseline follow the appropriate contractual change process.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The analysis identifies material ambiguity in integration scope, migration obligations, performance requirements, acceptance criteria, and operations. The recommendations are actionable, but technical and commercial boundaries remain undefined.

**Required corrections:** Confirm interface inventory, data migration scope, measurable acceptance criteria, customer–supplier responsibilities, exclusions, and support obligations.

**Approval blockers:** Undefined critical deliverables, missing acceptance criteria, and unresolved fixed-price commercial boundaries.

**Recommended scope status: NOT READY**

**Governance:** Supports PMI-aligned scope management, requirements analysis, procurement governance, quality planning, risk management, and change control.

AI-assisted analysis identifies potential scope gaps but does not establish contractual meaning or approve requirements. Final scope, commercial boundaries, and acceptance criteria require validation by authorized business, technical, commercial, and legal stakeholders. Protect confidential architecture, pricing, security requirements, and customer information.
