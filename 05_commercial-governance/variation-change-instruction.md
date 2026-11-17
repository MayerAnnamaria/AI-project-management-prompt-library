# Variation / Change Instruction

## Purpose

Use this prompt to draft a formal project change or variation instruction when additional or modified work needs to be introduced after the original scope or contract has been agreed.

Typical IT examples include:

- new functionality,
- additional integrations,
- increased data-migration scope,
- additional environments,
- security requirements,
- reporting changes,
- additional user groups,
- new regulatory requirements,
- changed infrastructure,
- extended vendor support.

The objective is to ensure the change is:

- clearly described,
- commercially traceable,
- assessed for impact,
- priced appropriately,
- approved through governance,
- and incorporated into delivery in a controlled way.

---

## Best Used For

**Project phase:**  
Delivery / Change / Contract Management

**Project type:**  
Software implementation / ERP / SaaS / Cloud / Infrastructure / Outsourcing / Digital Transformation

**Primary user:**  
Project Manager / Commercial Manager / Vendor Manager / Change Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Whenever material work is added, removed, or changed outside the agreed baseline or commercial scope

---

# Prompt

```text id="change-instruction-01"
ROLE

You are a senior IT Project Manager and Commercial Manager
experienced in software delivery, change control, vendor management,
technology contracts, and project governance.

TASK

Draft a formal Change / Variation Instruction for the project
change described below.

Do not invent contractual rights, clause references, approval
authority, pricing rules, or deadlines.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Contract:
[CONTRACT NAME / TYPE]

Customer:
[PARTY]

Supplier:
[PARTY]

Relevant clause:
[VERIFIED CLAUSE IF APPLICABLE]

Change type:
[INSTRUCTED CHANGE / PROPOSED CHANGE / SCOPE ADDITION /
SCOPE REDUCTION / TECHNICAL CHANGE]

CHANGE DETAILS

Description:
[DETAILED DESCRIPTION]

Reason:
[WHY CHANGE IS REQUIRED]

Original scope:
[RELEVANT ORIGINAL SCOPE]

New / changed scope:
[DETAILS]

Known schedule impact:
[DETAILS / TO BE ASSESSED]

Known cost impact:
[DETAILS / TO BE ASSESSED]

Known resource impact:
[DETAILS]

Known technical impact:
[DETAILS]

Known risk:
[DETAILS]

Pricing response required:
[YES / NO]

Pricing deadline:
[VERIFIED DEADLINE]

Schedule-impact assessment required:
[YES / NO]

Approval authority:
[ROLE]

OUTPUT FORMAT

Draft a formal instruction containing:

1. Reference and Subject
2. Change Authority / Contract Reference
3. Purpose
4. Background
5. Detailed Scope of Change
6. Exclusions / Boundaries
7. Supplier Impact Assessment Required
8. Pricing Requirements
9. Schedule / Resource Impact Requirements
10. Assumptions and Dependencies
11. Required Response Date
12. Approval / Governance Process
13. Next Steps
```

---

# Core Change Principle

Use:

```text id="change-flow"
Business Need
↓
Defined Change
↓
Impact Assessment
↓
Cost / Schedule / Risk
↓
Approval
↓
Baseline Update
↓
Implementation
```

Do not use:

```text id="change-bad-flow"
Informal Request
↓
Work Begins
↓
Impact Discovered Later
↓
Commercial Dispute
```

---

# 1. Reference and Subject

Use a precise title.

### Weak

```text id="change-subject-weak"
Change Request
```

### Better

```text id="change-subject-good"
Change Instruction CR-014 — Additional Salesforce-to-SAP Integration
```

Or:

```text id="change-subject-example"
Formal Scope Change — Additional Regulatory Reporting Requirements
```

---

# 2. Change Authority / Contract Reference

Where applicable state:

```text id="change-authority"
Contract:
[CONTRACT]

Clause:
[VERIFIED CLAUSE]

Authority Issuing Instruction:
[ROLE]

Change ID:
[ID]
```

Do not invent contractual authority.

If the change is still under assessment, describe it as a proposal rather than an approved instruction.

---

# 3. Purpose

State exactly what is being changed.

Example:

> This instruction requests the Supplier to assess and implement an additional integration between the CRM platform and the organisation’s SAP ERP system.

Avoid:

> Please make the necessary changes.

---

# 4. Background

Explain:

```text id="change-background"
Original requirement
New business need
Reason change arose
Decision / event triggering change
```

Example:

> Following completion of the original solution design, Finance confirmed that customer-credit data must also be synchronised with SAP. This integration was not included in the approved implementation scope.

---

# 5. Detailed Scope of Change

Describe exactly what is being added, removed, or modified.

For software changes consider:

```text id="change-scope-it"
Functional requirements

Interfaces

Data fields

User roles

Business rules

Reports

Environments

Security

Testing

Documentation

Training

Support
```

---

# Scope Description Rule

### Weak

```text id="change-scope-weak"
Add SAP integration.
```

### Better

```text id="change-scope-good"
Design, configure, test, and deploy an outbound integration from
the CRM platform to SAP to transmit approved customer-credit status.

The change includes:

- interface design,
- field mapping,
- API development,
- authentication configuration,
- SIT support,
- UAT support,
- technical documentation.
```

---

# 6. Exclusions / Boundaries

Clarify what the change does **not** include.

Example:

```text id="change-exclusions"
Not included:

- changes to SAP credit-calculation logic,
- historical data migration,
- additional CRM user licences,
- production support beyond the existing agreement.
```

This reduces future ambiguity.

---

# 7. Supplier Impact Assessment

Require the supplier to evaluate:

```text id="change-impact-assessment"
Solution impact
Architecture
Development
Testing
Data
Security
Resources
Schedule
Dependencies
Operational support
Documentation
Training
```

Use:

| Impact Area | Supplier Assessment Required |
|---|---|
| Scope | Yes |
| Cost | Yes |
| Schedule | Yes |
| Resources | Yes |
| Technical | Yes |
| Risk | Yes |
| Support | If relevant |

---

# 8. Pricing Requirements

Where pricing is required, request clear cost breakdown.

Possible structure:

```text id="change-pricing"
Labour

Licences

Infrastructure

Cloud consumption

Third-party costs

Testing

Travel

Support

Contingency where permitted

Taxes where applicable
```

Require assumptions to be explicit.

---

# Pricing Table

| Cost Element | Quantity / Effort | Rate | Total | Assumption |
|---|---:|---:|---:|---|

Do not accept a single lump-sum figure without sufficient supporting information where detailed review is required.

---

# 9. Schedule Impact

Request:

```text id="change-schedule-impact"
Affected milestones

New activities

Dependencies

Critical path impact

Delivery date impact

Recovery options

Required decision date
```

Example:

> The Supplier shall confirm whether the change can be incorporated without affecting the planned production release and identify any assumptions supporting that conclusion.

---

# 10. Resource Impact

Assess whether the change requires:

- additional developers,
- architects,
- testers,
- security specialists,
- business analysts,
- data specialists,
- vendor resources.

Example:

> The Supplier shall identify whether the existing delivery team can absorb the change or whether additional capacity is required.

---

# 11. Risk Assessment

Each significant change should assess risk.

Provide:

| Risk | Impact | Mitigation | Owner |
|---|---|---|---|

Potential IT change risks include:

```text id="change-risks"
Regression risk

Integration failure

Schedule compression

Resource overload

Security impact

Testing reduction

Vendor dependency

Operational readiness

Technical debt
```

---

# 12. Required Response

Be explicit.

Example:

```text id="change-response"
Please submit by 17:00 CET on 15 September:

1. technical impact assessment,
2. detailed cost proposal,
3. resource estimate,
4. schedule impact,
5. identified dependencies,
6. key assumptions,
7. delivery risks.
```

---

# 13. Approval Process

A proposed change should not automatically become authorised work.

Example flow:

```text id="change-approval-flow"
Change Raised
↓
Impact Assessment
↓
Technical Review
↓
Commercial Review
↓
Business Approval
↓
Change Approved
↓
Baseline Updated
↓
Implementation
```

---

# Change Status

Suggested statuses:

```text id="change-status"
Draft

Under Assessment

Awaiting Approval

Approved

Rejected

Deferred

Implemented

Closed
```

---

# Example Input

```text id="change-example-input"
Project:
CRM Implementation

Contract:
Software Implementation Agreement

Change:
Additional integration between CRM and SAP.

Original Scope:
CRM integration included only billing platform and customer portal.

Reason:
Finance requires customer credit status to be synchronised with SAP.

Known Cost:
Not yet known.

Known Schedule Impact:
Not yet known.

Required Supplier Response:
Technical assessment, price, resource requirement, and delivery
impact.

Response Deadline:
15 September.
```

---

# Example Output

## Subject

**Change Instruction CR-014 — Additional CRM-to-SAP Integration**

Dear [Supplier],

This instruction requests assessment of an additional integration between the CRM platform and SAP ERP.

The approved implementation scope currently includes integrations with the billing platform and customer portal. Following further business review, Finance has confirmed that approved customer-credit status must also be transferred from CRM to SAP.

The requested change includes interface design, field mapping, development, security configuration, testing support, and technical documentation.

Please provide by **15 September**:

1. detailed technical impact assessment,
2. commercial proposal,
3. resource requirement,
4. schedule impact,
5. key assumptions and dependencies,
6. delivery risks.

No implementation should commence until the change has completed the agreed approval process unless separately authorised in writing.

Kind regards,  
[Project Manager]

---

# Prompt 2 — Change Impact Review

```text id="change-impact-review"
ROLE

You are a senior IT Project Manager reviewing a proposed change.

TASK

Assess the proposed change below.

[PASTE CHANGE]

Analyse:

1. Scope impact
2. Technical impact
3. Schedule impact
4. Cost impact
5. Resource impact
6. Testing impact
7. Security impact
8. Operational impact
9. Dependencies
10. Risks

OUTPUT FORMAT

Impact Area
Assessment
Evidence / Assumption
Severity
Required Action
```

---

# Prompt 3 — Change Proposal Challenge

```text id="change-challenge"
ROLE

You are an independent PMO and Commercial reviewer.

TASK

Challenge the change proposal below.

[PASTE CHANGE]

Check for:

- unclear scope,
- missing exclusions,
- unsupported cost,
- hidden dependencies,
- missing acceptance criteria,
- incomplete test impact,
- missing security impact,
- unrealistic schedule,
- unapproved assumptions.

OUTPUT FORMAT

Gap
Why It Matters
Potential Impact
Recommended Correction
```

---

# Prompt 4 — Supplier Change Proposal Review

```text id="change-supplier-review"
ROLE

You are a senior IT Project Manager reviewing a supplier's
commercial change proposal.

TASK

Review the proposal below.

[PASTE PROPOSAL]

Check:

- scope matches instruction,
- exclusions are reasonable,
- effort assumptions,
- duplicated work,
- schedule impact,
- rates,
- dependencies,
- acceptance criteria,
- testing effort,
- commercial risk.

OUTPUT FORMAT

Finding
Supplier Position
Project Assessment
Clarification Required
Recommendation
```

---

# Change Control vs Backlog Change

Not every backlog change should become a commercial change.

Ask:

```text id="change-commercial-test"
Is the work inside the agreed scope?

Is the commercial model designed to absorb reprioritisation?

Does the change affect cost?

Does it affect committed dates?

Does it introduce new deliverables?

Does it change acceptance criteria?

Does it change contractual obligations?
```

If the answer is no to all material commercial questions, normal delivery reprioritisation may be sufficient.

---

# Agile / Scrum Considerations

In Agile delivery, distinguish between:

```text id="change-agile"
Backlog reprioritisation
```

and:

```text id="change-agile-commercial"
Commercial scope change
```

A Product Owner may reprioritise work within agreed commercial boundaries.

They should not automatically authorise new contractual scope.

---

# Kanban / Managed Service Considerations

In service environments, change may involve:

- new service classes,
- additional capacity,
- revised SLA,
- new request types,
- additional support hours.

Evaluate whether the proposed change alters the commercial service model.

---

# Predictive Considerations

Formal variation control may directly affect:

- scope baseline,
- cost baseline,
- schedule baseline,
- contract value.

Approved changes should be reflected in the relevant baselines.

---

# Hybrid Considerations

Use:

```text id="change-hybrid"
Delivery Flexibility
+
Commercial Control
```

Example:

> Teams may reprioritise features within the approved delivery envelope, while new integrations or material scope additions follow formal change control.

---

# Change Register

Maintain:

| Change ID | Description | Raised By | Date | Cost Impact | Schedule Impact | Status | Approver |
|---|---|---|---|---:|---|---|---|

For larger projects also capture:

```text id="change-register-extra"
Related Requirement
Contract Clause
Risk
Decision Date
Implementation Date
Baseline Updated
```

---

# Baseline Update

After approval, confirm whether the following need updating:

```text id="change-baseline"
Scope baseline

Budget

Schedule

Requirements

Architecture

Risk register

Test plan

Release plan

Vendor agreement

Documentation
```

An approved change is not fully controlled until affected project artefacts are updated.

---

# Acceptance Criteria

Define how the new or changed deliverable will be accepted.

Example:

```text id="change-acceptance"
SAP receives customer-credit status successfully.

Data mapping matches approved specification.

Failed transactions are logged.

Security review passes.

SIT completed.

Business acceptance completed.
```

Avoid accepting vague change scope without measurable completion criteria.

---

# Quality Checklist

Before issuing or approving a change, confirm:

- [ ] Change description is clear
- [ ] Original scope is understood
- [ ] New scope is defined
- [ ] Exclusions are explicit
- [ ] Technical impact is assessed
- [ ] Cost impact is assessed
- [ ] Schedule impact is assessed
- [ ] Resource impact is assessed
- [ ] Testing impact is assessed
- [ ] Security impact is considered
- [ ] Dependencies are identified
- [ ] Risks are identified
- [ ] Acceptance criteria exist
- [ ] Approval authority is clear
- [ ] Required response date is clear
- [ ] Approved baselines will be updated
- [ ] Contractual references are verified where applicable

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- integrated change control,
- scope,
- schedule,
- cost,
- procurement,
- risk,
- governance,
- stakeholder management.

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

Material changes should be reviewed by the appropriate:

- Project Manager
- Business Owner
- Technical Lead
- Architecture
- Security
- Finance
- Procurement / Commercial
- Legal where applicable
- Sponsor / Change Authority

AI can help structure change information and identify gaps.

It cannot approve contractual or financial changes on behalf of authorised stakeholders.

---

# Confidentiality

Change proposals may contain:

- pricing,
- architecture,
- vendor rates,
- security information,
- commercial assumptions,
- contract terms.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text id="change-metadata"
Prompt ID: COMM-003
Category: Commercial & Project Governance
Version: 1.0
Status: Draft
Owner: Project Manager / Commercial Manager
Reviewer: Change Authority / Procurement
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
| 1.0 | YYYY-MM-DD | Initial IT variation / change-instruction framework |
