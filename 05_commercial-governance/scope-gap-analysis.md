# Scope Gap Analysis

## Purpose

Use this prompt to review an IT scope, requirements document, Statement of Work, technical specification, or procurement package before approval or supplier commitment.

The analysis should identify:

- ambiguous requirements,
- missing requirements,
- unclear responsibilities,
- incomplete interfaces,
- missing acceptance criteria,
- assumptions that may later create disagreement,
- and areas likely to result in scope change or commercial dispute.

The objective is to identify scope problems **before they become delivery problems**.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Procurement / Contracting / Change Control

**Project type:**  
Software implementation / ERP / SaaS / Cloud / Infrastructure / Data / Outsourcing / Digital Transformation

**Primary user:**  
Project Manager / Business Analyst / Product Owner / Commercial Manager / Procurement / Solution Architect

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Before contract award, scope approval, major change approval, or vendor mobilisation

---

# Prompt

```text id="scope-gap-01"
ROLE

You are a senior IT Project Manager and Business / Commercial
Analyst experienced in software implementation, requirements
management, vendor delivery, contract governance, and scope control.

TASK

Review the project scope / requirements below and identify gaps
that could create delivery ambiguity, change requests, commercial
disputes, or acceptance problems.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Document type:
[SOW / REQUIREMENTS / RFP / CONTRACT SCOPE / TECHNICAL SPECIFICATION]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Supplier model:
[INTERNAL / EXTERNAL / MULTI-VENDOR]

Business objective:
[OBJECTIVE]

DOCUMENT TO REVIEW

[PASTE SCOPE / REQUIREMENTS]

CHECK FOR

1. Ambiguous statements
2. Missing requirements
3. Scope-change / variation risk
4. Unclear interface responsibilities
5. Missing measurable acceptance criteria
6. Undefined assumptions
7. Undefined exclusions
8. Missing dependencies
9. Missing security / compliance requirements
10. Missing operational / support requirements

OUTPUT FORMAT

Gap / Issue
Document Location
Why It Is Ambiguous / Missing
Risk to Customer
Risk to Supplier
Potential Delivery Impact
Recommended Fix
Priority
```

---

# Core Review Principle

Use:

```text id="scope-gap-flow"
Requirement
↓
Interpretation
↓
Ownership
↓
Acceptance
↓
Commercial Boundary
```

If any of these are unclear, scope risk increases.

---

# 1. Ambiguity Review

Look for wording that can be interpreted differently.

Examples:

```text id="scope-ambiguous-terms"
User-friendly

Modern

Best practice

High performance

Fast response

Appropriate security

Industry standard

Flexible reporting

Seamless integration

As required
```

These phrases may describe intent but often do not define a measurable requirement.

---

# Example

### Weak Requirement

```text id="scope-weak-requirement"
The system shall provide fast search.
```

### Better

```text id="scope-better-requirement"
For standard customer searches against the production dataset,
95% of requests shall return results within 2 seconds under the
agreed normal-load profile.
```

The exact target should come from stakeholder agreement, not AI invention.

---

# Ambiguity Questions

For every ambiguous statement ask:

```text id="scope-ambiguity-questions"
What does this mean?

How will compliance be measured?

Who decides whether it is acceptable?

Under what conditions?

What happens if the parties interpret it differently?
```

---

# 2. Missing Requirement Review

Check whether important requirement categories are absent.

Possible IT categories:

```text id="scope-missing-categories"
Business requirements
Functional requirements
Non-functional requirements
Data
Integrations
Security
Privacy
Performance
Availability
Accessibility
Environments
Testing
Migration
Training
Documentation
Deployment
Support
Operations
Monitoring
Disaster recovery
Compliance
```

Do not assume every category is required for every project.

---

# 3. Scope Change / Variation Risk

Identify wording that could produce future scope disputes.

Typical warning signs:

```text id="scope-change-risk"
"All necessary integrations"

"Any required reports"

"Complete migration"

"Full training"

"All applicable security requirements"

"Support as required"

"Any other functionality necessary"
```

These statements may leave commercial boundaries unclear.

---

# Example

### High-Risk Scope

```text id="scope-change-risk-example"
Supplier shall integrate the CRM with all relevant enterprise systems.
```

Questions:

```text id="scope-change-risk-questions"
Which systems?

How many interfaces?

What protocols?

Who owns each system?

Who provides API access?

Who pays for third-party changes?
```

---

# 4. Interface Responsibility Review

Interfaces are a common source of IT delivery risk.

For every interface identify:

| Interface | Customer Responsibility | Supplier Responsibility | Third Party | Acceptance Owner |
|---|---|---|---|---|

Consider:

```text id="scope-interface"
API specification
Authentication
Network connectivity
Test data
Firewall rules
Environment access
Source-system changes
Error handling
Monitoring
Support
```

---

# Responsibility Rule

Avoid:

```text id="scope-responsibility-weak"
Customer and supplier will coordinate integration.
```

Prefer clearly separated ownership.

Example:

```text id="scope-responsibility-good"
Supplier:
Develop CRM API client and error handling.

Customer:
Provide approved API specification and test endpoint.

Third Party:
Maintain availability of the billing API.

Customer Architecture:
Approve interface design.
```

---

# 5. Acceptance Criteria Review

Every important deliverable should have measurable acceptance criteria.

Ask:

```text id="scope-acceptance-questions"
What does complete mean?

Who accepts it?

What evidence is required?

What tolerance applies?

What happens when criteria are not met?
```

---

# Example

### Weak

```text id="scope-acceptance-weak"
Migration must be successful.
```

### Better

```text id="scope-acceptance-better"
Migration acceptance will be based on the agreed reconciliation
criteria, including completeness, accuracy, and exception handling.
```

Actual tolerances should be defined and approved by the project.

---

# Acceptance Matrix

| Deliverable | Acceptance Criterion | Evidence | Approver |
|---|---|---|---|

Examples:

```text id="scope-acceptance-examples"
Integration
→ Approved end-to-end test evidence

Data migration
→ Reconciliation results

Security
→ Required approval / test evidence

Training
→ Agreed materials delivered

Documentation
→ Required documents approved
```

---

# 6. Assumption Review

Identify hidden assumptions.

Examples:

```text id="scope-assumptions"
Customer data is clean.

APIs already exist.

Business users will be available.

Licences are already purchased.

Security approval will be straightforward.

Vendor resources are immediately available.
```

Convert important assumptions into explicit statements.

Use:

| Assumption | Owner | Validation Required | Impact if Wrong |
|---|---|---|---|

---

# 7. Exclusions Review

Scope should clearly state what is not included.

Possible exclusions:

```text id="scope-exclusions"
Historical data cleansing

Legacy-system remediation

Third-party licence fees

Changes to external systems

24/7 support

Post-go-live enhancement

Custom reporting beyond agreed reports

Additional environments
```

Exclusions should be explicit rather than assumed.

---

# 8. Dependency Review

Identify dependencies such as:

```text id="scope-dependencies"
Customer decisions

Vendor deliverables

Third-party APIs

Security approval

Data availability

Infrastructure

Environment readiness

Business resources

Procurement
```

Provide:

| Dependency | Owner | Required By | Impact if Late |
|---|---|---|---|

---

# 9. Security / Compliance Gap Review

Check whether the scope defines relevant requirements for:

```text id="scope-security"
Authentication

Authorisation

Encryption

Logging

Audit trail

Vulnerability management

Data residency

Retention

Privacy

Security testing

Access control
```

Do not invent standards or certifications.

Flag missing requirements for stakeholder confirmation.

---

# 10. Operational Readiness Gap Review

Scope often focuses on build but ignores operation.

Check:

```text id="scope-ops"
Monitoring

Incident management

Support ownership

Runbooks

Backup

Recovery

Service hours

SLA

Knowledge transfer

Hypercare

Handover
```

---

# Example Input

```text id="scope-gap-example-input"
Project:
Customer Portal

Scope Extract:

"The Supplier shall implement a modern customer portal integrated
with the CRM and other relevant enterprise systems.

The portal shall provide fast access to customer information.

The Supplier shall migrate all necessary customer data.

The solution shall comply with all applicable security standards.

The Supplier shall provide training and documentation.

The project shall be complete by 30 September."
```

---

# Example Gap Analysis

| Gap / Issue | Risk | Recommended Fix |
|---|---|---|
| "Other relevant enterprise systems" undefined | Number of integrations is commercially unclear | List all required integrations |
| "Fast access" not measurable | Performance acceptance dispute | Define measurable response-time criteria |
| "All necessary customer data" undefined | Migration scope may expand | Define entities, history, volume, and quality responsibilities |
| "Applicable security standards" undefined | Security obligations unclear | Identify approved security requirements |
| Training scope undefined | Number of sessions / users unclear | Define audience, format, duration, and materials |
| Documentation undefined | Acceptance disagreement | List required documents |

---

# Prompt 2 — Pre-Contract Scope Audit

```text id="scope-precontract"
ROLE

You are an independent IT Commercial Manager reviewing a scope
before contract signature.

TASK

Review the scope below specifically for commercial exposure.

[PASTE SCOPE]

Identify:

- open-ended obligations,
- undefined quantities,
- hidden assumptions,
- unclear ownership,
- customer dependencies,
- third-party dependencies,
- missing exclusions,
- missing acceptance criteria,
- language likely to create future change disputes.

OUTPUT FORMAT

Clause / Requirement
Commercial Risk
Customer Exposure
Supplier Exposure
Recommended Clarification
Priority
```

---

# Prompt 3 — Technical Scope Audit

```text id="scope-technical"
ROLE

You are a senior Solution Architect reviewing an IT project scope.

TASK

Review the scope below for technical completeness.

[PASTE SCOPE]

Check:

- architecture,
- integrations,
- environments,
- data,
- security,
- performance,
- resilience,
- monitoring,
- deployment,
- operational support.

OUTPUT FORMAT

Technical Gap
Why It Matters
Required Clarification
Owner
```

---

# Prompt 4 — Requirements Quality Audit

```text id="scope-requirements-quality"
ROLE

You are a senior Business Analyst.

TASK

Review the requirements below for quality.

[PASTE REQUIREMENTS]

Check whether each requirement is:

Clear
Testable
Unambiguous
Necessary
Traceable
Feasible
Measurable where relevant

OUTPUT FORMAT

Requirement
Quality Issue
Why It Matters
Suggested Clarification
```

---

# Scope Gap Severity

Possible classification:

```text id="scope-gap-severity"
Critical
Likely to cause major delivery, commercial, security, or acceptance failure.

High
Material ambiguity requiring resolution before commitment.

Medium
Important clarification but manageable.

Low
Minor improvement.
```

Use project context when assigning severity.

---

# Customer vs Supplier Perspective

A mature review should assess both sides.

Example:

```text id="scope-two-sided"
Ambiguous acceptance criteria

Customer Risk:
May receive a deliverable that does not meet expected outcomes.

Supplier Risk:
May face repeated rejection based on undocumented expectations.
```

Good scope definition protects both parties.

---

# Change-Risk Indicator

For each gap optionally assess:

```text id="scope-change-indicator"
Low
Medium
High
```

Ask:

> How likely is this ambiguity to create a future change request or commercial disagreement?

---

# Agile / Scrum Considerations

Agile projects may intentionally leave detailed feature requirements flexible.

However, commercial boundaries should still be clear.

Distinguish:

```text id="scope-agile"
Detailed backlog content
```

from:

```text id="scope-agile-commercial"
Contractual scope boundary
```

Examples of fixed boundaries may include:

- product area,
- team capacity,
- budget,
- duration,
- major interfaces,
- non-functional requirements,
- compliance obligations.

---

# Kanban / Managed Service Considerations

Review whether the scope defines:

- service boundaries,
- request types,
- service hours,
- priorities,
- SLAs / SLEs,
- support responsibilities,
- capacity assumptions.

Avoid ambiguous wording such as:

> Supplier will handle all support requests as required.

---

# Predictive Considerations

Detailed scope clarity is particularly important where:

- scope is baselined,
- price is fixed,
- milestone acceptance drives payment,
- formal change control applies.

---

# Hybrid Considerations

Keep enough definition for commercial and governance control while allowing delivery flexibility inside agreed boundaries.

---

# Scope-to-Change Prevention

Use:

```text id="scope-prevention"
Clear Scope
+
Clear Interfaces
+
Clear Assumptions
+
Clear Acceptance
+
Clear Exclusions
=
Lower Change / Dispute Risk
```

---

# Scope Gap Register

For significant reviews maintain:

| Gap ID | Requirement | Gap | Risk | Owner | Resolution | Status |
|---|---|---|---|---|---|---|

Suggested statuses:

```text id="scope-gap-status"
Open
Under Review
Clarified
Accepted Risk
Resolved
```

---

# Quality Checklist

Before approving the scope, confirm:

- [ ] Business objective is clear
- [ ] In-scope items are defined
- [ ] Out-of-scope items are defined
- [ ] Deliverables are defined
- [ ] Interfaces are identified
- [ ] Responsibilities are assigned
- [ ] Dependencies are identified
- [ ] Assumptions are explicit
- [ ] Acceptance criteria are measurable
- [ ] Security requirements are addressed
- [ ] Data requirements are addressed
- [ ] Testing responsibilities are clear
- [ ] Operational requirements are addressed
- [ ] Vendor responsibilities are clear
- [ ] Customer responsibilities are clear
- [ ] Commercial boundaries are understood
- [ ] High-risk ambiguities are resolved before commitment

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- scope management,
- requirements,
- procurement,
- risk,
- integrated change control,
- stakeholder alignment,
- quality.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

---

# Human Review Required

Scope reviews should involve relevant stakeholders such as:

- Project Manager
- Business Analyst
- Product Owner
- Solution Architect
- Security
- QA
- Procurement / Commercial
- Legal where applicable
- Vendor representatives

AI can identify potential ambiguity.

It cannot determine the final commercial interpretation of a contract.

---

# Confidentiality

Scope and contract documents may contain confidential information.

Protect:

- architecture,
- pricing,
- security requirements,
- commercial terms,
- customer information,
- proprietary solution details.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text id="scope-gap-metadata"
Prompt ID: COMM-004
Category: Commercial & Project Governance
Version: 1.0
Status: Draft
Owner: Project Manager / Business Analyst
Reviewer: Commercial / Architecture / Legal where applicable
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: High
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT scope-gap analysis framework |
