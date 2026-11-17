# Supplier RFQ / RFP Response Review

## Purpose

Use this prompt to evaluate a supplier response against the requirements defined in an RFQ, RFP, tender, or vendor-selection process.

The review should identify:

- compliant requirements,
- partial responses,
- missing information,
- material deviations,
- commercial gaps,
- technical gaps,
- delivery risks,
- and clarification questions.

The objective is not simply to determine whether a supplier submitted a response.

The objective is to assess whether the response provides enough evidence to support an informed procurement decision.

---

## Best Used For

**Project phase:**  
Procurement / Vendor Selection / Contracting

**Project type:**  
Software implementation / SaaS / Cloud / ERP / Infrastructure / Data / Outsourcing / Consulting / Digital Transformation

**Primary user:**  
Project Manager / Procurement / Commercial Manager / Solution Architect / Vendor Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
For every material supplier evaluation

---

# Prompt

```text id="rfq-review-01"
ROLE

You are a senior IT Project Manager and Vendor Evaluation specialist
experienced in software procurement, supplier selection, technology
contracts, commercial evaluation, and project delivery.

TASK

Review the supplier response against the stated RFQ / RFP requirements.

Do not assume missing information is compliant.

Do not invent supplier capabilities or evidence.

PROCUREMENT CONTEXT

Project:
[PROJECT NAME]

Procurement type:
[RFQ / RFP / TENDER / VENDOR SELECTION]

Service / product:
[DESCRIPTION]

Evaluation stage:
[TECHNICAL / COMMERCIAL / FINAL]

WHAT WE REQUESTED

[PASTE REQUIREMENTS]

WHAT THE SUPPLIER PROVIDED

[PASTE RESPONSE]

OUTPUT FORMAT

Provide:

1. Executive Assessment
2. Compliance Gap Table
3. Technical Gaps
4. Commercial Gaps
5. Delivery / Resource Gaps
6. Security / Compliance Gaps
7. Clarification Questions
8. Top Risks
9. Recommendation

Recommendation options:

- Accept for next evaluation stage
- Accept with conditions
- Request clarification before progressing
- Reject
```

---

# 1. Executive Assessment

Summarise:

```text id="rfq-exec"
Overall compliance

Strongest areas

Most significant gaps

Whether missing information is material

Overall recommendation
```

Example:

> The supplier demonstrates relevant platform experience and has provided a commercially complete pricing proposal. However, the submission is incomplete in three material areas: resource availability, migration methodology, and security evidence. Clarification should be completed before commercial evaluation proceeds.

---

# 2. Compliance Gap Table

Use:

| Requirement | Requested | Supplier Response | Status | Gap / Concern | Clarification Required |
|---|---|---|---|---|---|

Suggested statuses:

```text id="rfq-status"
Compliant
Partially Compliant
Non-Compliant
Not Provided
Requires Clarification
```

Do not mark an item compliant where evidence is missing.

---

# Example

| Requirement | Requested | Supplier Response | Status |
|---|---|---|---|
| Relevant experience | 3 comparable implementations | 2 examples provided | Partially Compliant |
| Named PM | Required | CV provided | Compliant |
| Delivery plan | Required | Not submitted | Not Provided |
| Security certification | Required | Certificate expired | Non-Compliant |

---

# 3. Technical Review

Assess areas such as:

```text id="rfq-technical"
Solution architecture

Integration approach

API capability

Data migration

Performance

Scalability

Security architecture

Environments

Testing approach

Deployment

Monitoring

Support
```

Use:

| Technical Area | Requirement | Supplier Evidence | Assessment | Risk |
|---|---|---|---|---|

---

# Technical Evidence Rule

Do not accept statements such as:

```text id="rfq-technical-weak"
"Our solution is scalable."
```

without supporting detail where evidence was requested.

Ask:

```text id="rfq-technical-questions"
What scale has been demonstrated?

Under what load?

What architecture supports scalability?

What evidence is available?

What limits apply?
```

---

# 4. Commercial Review

Assess:

```text id="rfq-commercial"
Pricing model

Licence costs

Implementation cost

Recurring fees

Third-party costs

Cloud costs

Support costs

Rate cards

Change rates

Travel

Taxes

Assumptions

Exclusions
```

Provide:

| Commercial Item | Requirement | Supplier Position | Gap | Risk |
|---|---|---|---|---|

---

# Hidden Cost Review

Look for potential costs not clearly included.

Examples:

```text id="rfq-hidden-cost"
Additional environments

API usage fees

Data storage

Cloud consumption

Premium support

Training

Travel

Third-party licences

Migration tools

Post-go-live support

Additional users
```

Flag these as questions, not assumed costs.

---

# 5. Delivery / Resource Review

Assess:

```text id="rfq-delivery"
Delivery methodology

Mobilisation date

Project plan

Team structure

Named resources

Availability

Dependencies

Milestones

Governance

Escalation model
```

Example questions:

```text id="rfq-delivery-questions"
Are named resources committed or illustrative?

When are they available?

How many parallel projects are they supporting?

Who replaces key resources if unavailable?

Who owns delivery escalation?
```

---

# Resource Compliance Table

| Required Role | Supplier Proposal | Availability | Experience | Status |
|---|---|---|---|---|

Possible roles:

```text id="rfq-roles"
Project Manager
Solution Architect
Business Analyst
Technical Lead
Developers
Data Specialist
QA Lead
Security Specialist
Change Lead
Support Lead
```

---

# 6. Security / Compliance Review

Where relevant evaluate:

```text id="rfq-security"
Security certifications

Data protection

Data residency

Access controls

Encryption

Incident management

Vulnerability management

Subprocessors

Business continuity

Disaster recovery

Audit rights
```

Do not infer compliance from generic statements.

Example:

> “We follow industry-standard security” should not automatically be treated as evidence of a specific security requirement.

---

# 7. Clarification Questions

Clarification questions should be:

```text id="rfq-clarification-principles"
Specific
Evidence-oriented
Neutral
Linked to a stated requirement
```

### Weak

```text id="rfq-question-weak"
Can you provide more detail?
```

### Better

```text id="rfq-question-good"
Please confirm the named Solution Architect who would be allocated
to the project, their expected allocation percentage, and their
availability from the planned mobilisation date.
```

---

# Clarification Table

| ID | Requirement | Clarification Question | Why Required | Priority |
|---|---|---|---|---|

---

# 8. Top Procurement Risks

Identify the most material risks in the response.

Possible examples:

```text id="rfq-risks"
Unclear scope assumptions

Insufficient resource capacity

Unproven technical capability

Incomplete migration approach

Hidden recurring cost

Security non-compliance

Vendor lock-in

Unrealistic timeline

Weak support model

Excessive dependency on subcontractors
```

Provide:

| Risk | Evidence | Potential Impact | Clarification / Mitigation |
|---|---|---|---|

---

# Top 3 Commercial Traps

After the review, run:

```text id="rfq-commercial-traps"
ROLE

You are a senior IT Commercial Manager.

TASK

From the supplier response below, identify the three highest-risk
commercial gaps that could later create:

- change requests,
- cost escalation,
- delivery dispute,
- acceptance dispute,
- vendor lock-in.

For each provide:

Risk
Supplier Position
Why It Matters
Potential Future Dispute
Recommended Clarification Before Contract
```

---

# 9. Recommendation

Use one of:

```text id="rfq-recommendations"
Accept for next evaluation stage

Accept with conditions

Request clarification before progressing

Reject
```

Explain the recommendation.

Example:

```text id="rfq-recommendation-example"
Recommendation:
Request clarification before progressing.

Reason:
The supplier meets the core functional and commercial requirements,
but material gaps remain in migration planning, named resource
availability, and security evidence.

Progression should depend on satisfactory resolution of these items.
```

---

# Recommendation Rule

Do not recommend rejection merely because the response is imperfect.

Ask:

```text id="rfq-recommendation-test"
Is the gap material?

Can it be clarified?

Does it breach a mandatory requirement?

Does it create unacceptable risk?

Does procurement policy allow conditional progression?
```

---

# Example Input

```text id="rfq-example-input"
Project:
CRM Replacement

Requested:

- fixed implementation price
- detailed migration methodology
- 3 comparable CRM projects
- named PM and Solution Architect
- project plan
- EU data residency
- ISO 27001 certification
- 12 months post-go-live support
- detailed technical compliance matrix

Supplier response:

- fixed implementation price: €920,000
- migration approach: 2-page summary
- 2 CRM references
- PM CV provided
- no named Solution Architect
- high-level 8-month timeline
- EU hosting confirmed
- ISO 27001 certificate provided
- support proposal included for 6 months
- compliance matrix 80% complete
```

---

# Example Compliance Review

| Requirement | Supplier Response | Status | Gap |
|---|---|---|---|
| Fixed price | €920k | Compliant | None |
| Migration methodology | Brief summary | Partial | Detailed reconciliation / cutover approach missing |
| 3 references | 2 provided | Partial | One reference missing |
| Solution Architect | Not named | Not Provided | Resource risk |
| EU residency | Confirmed | Compliant | Verify contract wording |
| 12-month support | 6 months | Non-Compliant | Support period below requirement |
| Compliance matrix | 80% complete | Partial | Remaining items require clarification |

---

# Prompt 2 — Supplier Response Quality Review

```text id="rfq-quality-review"
ROLE

You are an independent Procurement and PMO reviewer.

TASK

Review the supplier evaluation below.

[PASTE EVALUATION]

Check for:

- requirements incorrectly marked compliant,
- missing evidence,
- inconsistent scoring,
- unsupported conclusions,
- supplier assumptions treated as commitments,
- commercially material gaps,
- bias in recommendation.

OUTPUT FORMAT

Finding
Evidence
Why It Matters
Recommended Correction
Priority
```

---

# Prompt 3 — Compare Multiple Suppliers

```text id="rfq-comparison"
ROLE

You are a senior IT Procurement Evaluation Lead.

TASK

Compare the supplier responses below against the same requirements.

SUPPLIER A
[PASTE]

SUPPLIER B
[PASTE]

SUPPLIER C
[PASTE]

OUTPUT FORMAT

Requirement
Supplier A
Supplier B
Supplier C
Evaluation Comment

Then provide:

1. Technical strengths
2. Commercial strengths
3. Key risks
4. Clarifications required
5. Recommended shortlist
```

Do not invent scoring weights unless they have been provided.

---

# Weighted Evaluation

Where approved weights exist:

| Criterion | Weight | Supplier Score | Weighted Score |
|---|---:|---:|---:|

Possible criteria:

```text id="rfq-weighting"
Technical fit
Relevant experience
Delivery capability
Commercial
Security
Support
Implementation team
```

Use only approved evaluation criteria and weights.

---

# Mandatory vs Desirable Requirements

Separate:

```text id="rfq-mandatory"
Mandatory
Failure may prevent progression.
```

from:

```text id="rfq-desirable"
Desirable
Contributes to comparative evaluation.
```

This avoids rejecting a supplier for a non-mandatory preference.

---

# Bid Assumption Review

Suppliers often include assumptions that materially affect price or delivery.

Extract:

| Supplier Assumption | Impact if Incorrect | Customer Action Required | Risk |
|---|---|---|---|

Examples:

```text id="rfq-assumptions"
Customer provides clean data

Customer supplies API access

Business SMEs available

No weekend work required

One migration cycle only

Existing licences sufficient
```

---

# Exclusion Review

Extract supplier exclusions separately.

Example:

```text id="rfq-exclusions"
Data cleansing excluded.

Third-party API changes excluded.

Penetration testing excluded.

Training beyond two sessions excluded.
```

Ask whether each exclusion is:

- acceptable,
- priced elsewhere,
- or a scope gap.

---

# Vendor Dependency Review

Identify:

```text id="rfq-vendor-dependencies"
Subcontractors

Cloud providers

Software manufacturers

Specialist resources

Offshore teams

Third-party licences
```

Ask:

> Which important deliverables depend on a third party not directly controlled by the bidder?

---

# Agile / Scrum Considerations

Where suppliers propose Agile delivery, review:

- team structure,
- Product Owner assumptions,
- backlog ownership,
- capacity model,
- release planning,
- Definition of Done,
- commercial treatment of changing priorities.

Do not accept “Agile” as a substitute for a delivery plan.

---

# Kanban / Managed Service Considerations

For service suppliers assess:

```text id="rfq-kanban"
Service classes

Capacity

WIP policy

SLA / SLE

Response times

Resolution times

Escalation

Reporting
```

---

# Predictive Considerations

Where delivery is milestone-driven, evaluate:

- detailed plan,
- dependencies,
- milestone acceptance,
- resource loading,
- critical path,
- change control.

---

# Hybrid Considerations

Assess whether governance and commercial structure actually support the proposed delivery model.

---

# Evaluation Traceability

Maintain a clear chain:

```text id="rfq-traceability"
RFQ Requirement
↓
Supplier Response
↓
Evidence
↓
Evaluator Assessment
↓
Clarification
↓
Final Decision
```

This improves defensibility of procurement decisions.

---

# Quality Checklist

Before finalising supplier evaluation, confirm:

- [ ] Every mandatory requirement is reviewed
- [ ] Partial responses are identified
- [ ] Missing evidence is visible
- [ ] Assumptions are extracted
- [ ] Exclusions are extracted
- [ ] Commercial gaps are identified
- [ ] Technical gaps are identified
- [ ] Security requirements are assessed
- [ ] Resource capability is reviewed
- [ ] Delivery plan is reviewed
- [ ] Clarification questions are specific
- [ ] Recommendation is evidence-based
- [ ] Evaluation criteria are applied consistently
- [ ] No unsupported supplier capability is assumed

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- procurement,
- supplier selection,
- risk,
- quality,
- cost,
- stakeholder management,
- governance.

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

Supplier evaluation should involve appropriate stakeholders such as:

- Procurement
- Project Manager
- Solution Architect
- Security
- Finance
- Business Owner
- Commercial / Legal
- Vendor Management

AI can help compare responses and identify gaps.

It should not make the final supplier-selection decision independently.

---

# Confidentiality

Supplier proposals are commercially sensitive.

Protect:

- pricing,
- technical architecture,
- rate cards,
- resource information,
- security evidence,
- negotiation positions,
- proprietary supplier information.

Do not upload confidential supplier submissions to public AI tools unless organisational policy permits it.

---

# Prompt Metadata

```text id="rfq-metadata"
Prompt ID: COMM-005
Category: Commercial & Project Governance
Version: 1.0
Status: Draft
Owner: Project Manager / Procurement
Reviewer: Commercial / Technical / Security
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
| 1.0 | YYYY-MM-DD | Initial IT supplier RFQ / RFP response-review framework |
