# Procurement Plan

## Purpose

Use this prompt to create a structured procurement plan for an IT, software, digital transformation, data, infrastructure, or technology-enabled project.

The procurement plan should clarify:

- what needs to be purchased,
- why external support is required,
- how suppliers will be selected,
- what approvals are needed,
- which commercial and delivery risks exist,
- and how vendor performance will be governed.

The objective is not simply to create a supplier list.

The objective is to ensure that external procurement supports project scope, delivery, quality, budget, and governance.

---

## Best Used For

**Project phase:**  
Planning / Procurement Preparation

**Project type:**  
Software implementation / Digital transformation / Cloud migration / Data / Infrastructure / ERP / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / PMO / Procurement Lead / Vendor Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
During project planning and whenever major external procurement is introduced or changed

---

# Prompt

```text id="procurement-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, vendor management, procurement coordination,
commercial governance, and third-party delivery.

TASK

Create a professional procurement plan for the project described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Project budget:
[BUDGET OR RANGE]

Target completion:
[DATE]

PROCUREMENT REQUIREMENTS

External services required:
[LIST]

Software / licences required:
[LIST]

Cloud / infrastructure services:
[LIST]

Implementation partners:
[LIST]

Specialist consultants:
[LIST]

Existing vendors:
[LIST]

Known contract constraints:
[LIST]

Known procurement policies:
[LIST]

Required approvals:
[LIST]

Security / compliance requirements:
[LIST]

Known vendor risks:
[LIST]

Local or organisational procurement requirements:
[LIST]

OUTPUT FORMAT

Create the procurement plan with:

1. Procurement Objectives
2. Procurement Strategy
3. Procurement Package List
4. Supplier Evaluation Criteria
5. Supplier Qualification Requirements
6. Procurement Timeline
7. Commercial and Contract Considerations
8. Governance and Approval Pathway
9. Vendor Performance Management
10. Key Procurement Risks and Mitigations
11. Recommended Next Actions
```

---

# Procurement Strategy

For each procurement area, determine the most appropriate approach.

Possible approaches may include:

```text id="procurement-methods"
Existing framework agreement
Competitive tender
Request for Proposal
Request for Quotation
Direct award where permitted
Extension of existing supplier agreement
Software subscription
Cloud consumption agreement
Professional services engagement
Staff augmentation
Managed service
Fixed-price implementation
Time and materials
Outcome-based engagement
```

Do not recommend a procurement method without considering organisational procurement rules.

---

# Procurement Package List

Provide:

| Package | Requirement | Procurement Method | Estimated Value | Required By | Owner | Approval Required |
|---|---|---|---:|---|---|---|

Possible IT procurement packages include:

- software licences,
- implementation partner,
- cloud services,
- infrastructure,
- data migration,
- integration development,
- cybersecurity testing,
- QA services,
- specialist consultants,
- training,
- change-management support,
- operational support.

---

# Supplier Evaluation Criteria

Define objective evaluation criteria.

Example:

| Criterion | Weight | Evidence Required |
|---|---:|---|
| Technical capability | 25% | Technical proposal |
| Relevant experience | 20% | Reference projects |
| Delivery approach | 15% | Delivery methodology |
| Commercial proposal | 20% | Pricing model |
| Security / compliance | 10% | Certifications / controls |
| Team capability | 10% | CVs / resource plan |

Use weights only where the organisation has approved or agreed them.

---

# Supplier Qualification Requirements

Consider:

- relevant delivery experience,
- technical capability,
- financial stability,
- security standards,
- data-protection capability,
- regulatory compliance,
- insurance where required,
- staffing capacity,
- geographic coverage,
- support capability,
- references,
- conflict-of-interest checks.

For software or cloud suppliers, also consider:

```text id="procurement-saas"
Data residency
Service availability
Disaster recovery
Security certification
Data portability
Exit arrangements
Integration capability
API availability
Support model
Product roadmap
```

---

# Procurement Timeline

Create a procurement timeline covering:

```text id="procurement-timeline"
Requirements confirmed
↓
Procurement strategy approved
↓
Supplier market engagement
↓
RFP / RFQ issued
↓
Supplier responses received
↓
Evaluation
↓
Clarifications
↓
Commercial negotiation
↓
Approval
↓
Contract signature
↓
Mobilisation
```

Provide:

| Procurement Stage | Planned Date | Dependency | Owner |
|---|---|---|---|

---

# Delivery Dependency Review

Procurement timelines should be linked to project delivery.

For every major procurement item identify:

| Procurement Item | Delivery Dependency | Required By | Impact if Late |
|---|---|---|---|

Example:

```text id="procurement-dependency-example"
Identity-management licence

Required before:
Integration testing

Impact if late:
Authentication integration cannot enter SIT.
```

---

# Commercial and Contract Considerations

Where relevant, assess:

- pricing model,
- payment milestones,
- acceptance criteria,
- service levels,
- delivery milestones,
- change-control mechanism,
- intellectual property,
- confidentiality,
- data ownership,
- termination rights,
- exit provisions,
- warranty,
- support period,
- liability,
- subcontracting,
- audit rights.

Do not generate or interpret contractual clauses as legal advice.

Contract terms should be reviewed by qualified legal and procurement professionals.

---

# Agile / Scrum Considerations

Where external vendors support iterative delivery, consider:

- capacity model,
- backlog flexibility,
- team continuity,
- release cadence,
- acceptance criteria,
- Definition of Done,
- commercial treatment of changing priorities.

Avoid creating a contract structure that requires detailed fixed scope while expecting unrestricted Agile change.

Explicitly identify this tension if it exists.

---

# Kanban Considerations

Where suppliers deliver through flow-based work, consider:

- service demand,
- WIP expectations,
- Service Level Expectations,
- throughput,
- blocked-item escalation,
- priority policies,
- support responsiveness.

Commercial measures should support flow rather than incentivise excessive work in progress.

---

# Predictive Considerations

Where scope and deliverables are defined upfront, procurement may focus more strongly on:

- fixed deliverables,
- milestone payments,
- formal acceptance,
- schedule commitments,
- contractual change control.

---

# Hybrid Considerations

Hybrid procurement may combine:

```text id="procurement-hybrid"
Fixed commercial boundaries
+
Flexible delivery prioritisation
+
Defined governance
+
Controlled change
```

Clarify which elements are fixed and which may adapt during delivery.

---

# Vendor Governance Model

For each strategic supplier, define:

| Governance Area | Owner | Cadence | Evidence |
|---|---|---|---|
| Delivery performance | Project Manager | Weekly | Delivery report |
| Commercial performance | Procurement / PM | Monthly | Cost report |
| Quality | QA Lead | Regular | Defect / quality metrics |
| Security | Security Lead | Milestone-based | Security review |
| Risks | PM / Vendor Lead | Weekly | Risk register |
| Executive escalation | Sponsor | As needed | Decision paper |

---

# Vendor Performance Indicators

Use metrics appropriate to the contract and delivery model.

Possible measures include:

- milestone achievement,
- deliverable acceptance,
- defect rate,
- SLA performance,
- response time,
- resolution time,
- cycle time,
- throughput,
- resource continuity,
- forecast accuracy,
- budget performance,
- change-request volume,
- security compliance.

Do not use metrics simply because they are easy to measure.

Each metric should support a management decision.

---

# Procurement Risk Review

Provide:

| Risk | Cause | Probability | Impact | Mitigation | Owner |
|---|---|---|---|---|---|

Typical IT procurement risks may include:

```text id="procurement-risks"
Long supplier lead time
Vendor capacity shortage
Supplier lock-in
Unclear requirements
Commercial model misalignment
Integration dependency
Security non-compliance
Data-residency issue
Licence-cost growth
Vendor financial instability
Single-source dependency
Key-person dependency
Contract approval delay
```

---

# Example Input

```text id="procurement-example-input"
Project:
CRM Replacement

Delivery Approach:
Hybrid

Budget:
€1.8 million

External Requirements:
CRM software licences
Implementation partner
Data migration specialist
Penetration testing provider

Existing Vendor:
Cloud hosting provider

Required Approvals:
Procurement
Finance
Information Security
Legal

Known Constraints:
Target implementation partner mobilisation in April.
Security approval required before contract signature.
Customer data must remain within the EU.

Known Risks:
Limited number of qualified migration suppliers.
CRM implementation partner availability may be constrained.
```

---

# Example Output Excerpt

## Procurement Strategy

The CRM replacement requires four major external procurement areas: software licensing, implementation services, data migration, and penetration testing.

The implementation partner and migration specialist represent the highest delivery dependency because late mobilisation could directly affect configuration, migration preparation, and the planned testing timeline.

Supplier selection should therefore balance commercial competitiveness with demonstrated CRM implementation capability, available delivery capacity, security compliance, and relevant migration experience.

---

## Example Package List

| Package | Method | Required By | Key Approval |
|---|---|---|---|
| CRM licences | Commercial negotiation | March | Procurement / Finance |
| Implementation partner | Competitive RFP | April | Steering Committee |
| Data migration specialist | RFQ / existing framework | May | Procurement |
| Penetration testing | Approved supplier panel | Before release | Security |

---

# Procurement Gap Review

After creating the plan, perform a second review.

```text id="procurement-gap"
ROLE

You are a senior IT Procurement and Project Governance specialist.

TASK

Review the procurement plan below and identify gaps that could
affect delivery, cost, quality, or governance.

[PASTE PROCUREMENT PLAN]

Check specifically for:

- missing procurement packages,
- unclear evaluation criteria,
- missing approvals,
- unrealistic lead times,
- vendor dependencies,
- unclear acceptance criteria,
- security gaps,
- data-protection gaps,
- contract / delivery model mismatch,
- missing exit arrangements,
- unclear supplier ownership.

OUTPUT FORMAT

Gap
Why It Matters
Potential Impact
Recommended Action
Owner
Priority
```

---

# Quality Checklist

Before approving the procurement plan, confirm:

- [ ] Procurement requirements are linked to project scope
- [ ] Major packages are identified
- [ ] Evaluation criteria are explicit
- [ ] Supplier qualification requirements are defined
- [ ] Procurement lead times are realistic
- [ ] Delivery dependencies are visible
- [ ] Required approvals are identified
- [ ] Security and compliance requirements are included
- [ ] Commercial model supports the delivery approach
- [ ] Vendor governance is defined
- [ ] Procurement risks have owners
- [ ] Exit and transition considerations are addressed where relevant

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- procurement management,
- planning,
- stakeholder management,
- risk,
- financial management,
- governance,
- vendor management.

## PMBOK Relevance

This prompt supports:

- procurement,
- finance,
- risk,
- governance,
- delivery,
- stakeholders.

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

Validate the procurement plan with:

- Project Manager
- Procurement
- Finance
- Legal
- Information Security
- Technical Lead
- Sponsor
- Vendor Manager where applicable

AI-generated procurement recommendations should not replace organisational procurement procedures, commercial approvals, or legal review.

---

# Confidentiality

Procurement information is often commercially sensitive.

Do not enter into public AI tools:

- confidential vendor pricing,
- tender responses,
- contract terms,
- negotiation positions,
- supplier financial information,
- proprietary solution information.

Anonymise supplier information where necessary.

---

# Prompt Metadata

```text id="procurement-metadata"
Prompt ID: PLAN-005
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Procurement / Finance / Legal
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT procurement planning framework |
