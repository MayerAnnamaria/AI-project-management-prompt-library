# Contract Close-Out

## Purpose

Use this prompt to prepare structured contract and supplier close-out documentation for an IT or digital project.

The close-out process should confirm:

- what was finally delivered,
- what was finally paid,
- whether outstanding commercial items remain,
- whether deliverables were accepted,
- whether documentation is complete,
- whether support and operational ownership have transferred,
- and whether the contract can be formally closed.

The objective is not simply to declare the project complete.

The objective is to ensure that **commercial, technical, operational, and governance obligations have actually been closed**.

---

## Best Used For

**Project phase:**  
Deployment / Handover / Hypercare Exit / Project Close

**Project type:**  
Software implementation / SaaS / ERP / Cloud / Infrastructure / Outsourcing / Digital Transformation

**Primary user:**  
Project Manager / Commercial Manager / Vendor Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Prepare progressively before handover and finalise at contract closure

---

# Prompt

```text id="closeout-01"
ROLE

You are a senior IT Project Manager and Commercial Manager
experienced in software delivery, vendor governance, project
handover, contract close-out, financial reconciliation, and
operational transition.

TASK

Prepare the contract close-out package for the project below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Contract:
[CONTRACT NAME / TYPE]

Customer:
[PARTY]

Supplier:
[PARTY]

Original contract value:
[VALUE]

Approved changes:
[VALUE / LIST]

Adjusted contract value:
[VALUE]

Supplier final account / final invoice:
[VALUE]

Agreed final commercial position:
[VALUE]

Contingency:
[DETAILS]

Outstanding commercial items:
[DETAILS]

Current delivery status:
[DETAILS]

Outstanding defects:
[DETAILS]

Documentation status:
[DETAILS]

Operational handover status:
[DETAILS]

Security / compliance status:
[DETAILS]

Support / warranty arrangements:
[DETAILS]

OUTPUT FORMAT

Produce two outputs:

1. FINAL COMMERCIAL NARRATIVE
2. CONTRACT CLOSE-OUT CHECKLIST
```

---

# Output 1 — Final Commercial Narrative

The narrative should explain:

```text id="closeout-commercial-structure"
Original commercial position

Approved changes

Adjusted contract value

Final supplier position

Agreed final position

Variance

Contingency usage

Outstanding liabilities / commitments

Overall commercial conclusion
```

---

# Example Structure

## Original Contract Position

State:

```text id="closeout-original"
Original contract value
Original commercial model
Initial approved scope
```

Example:

> The original implementation agreement was approved at €1.8M and covered CRM configuration, integration, migration, testing support, training, and implementation services.

---

# Approved Changes

Summarise:

| Change | Reason | Approved Value |
|---|---|---:|
| CR-04 | Additional SAP integration | €80,000 |
| CR-09 | Extended migration scope | €55,000 |
| CR-12 | Additional hypercare | €25,000 |

Then provide:

```text id="closeout-adjusted"
Original Contract
+
Approved Changes
=
Adjusted Contract Value
```

---

# Final Commercial Position

Provide:

| Measure | Value |
|---|---:|
| Original Contract | |
| Approved Changes | |
| Adjusted Contract | |
| Supplier Final Submission | |
| Agreed Final Position | |
| Variance | |

Explain the variance.

Do not simply reproduce the numbers.

---

# Commercial Commentary

Answer:

```text id="closeout-commercial-questions"
Why did the final cost differ?

Which changes drove the variance?

Was contingency used?

Were any claims rejected?

Were savings achieved?

Are any liabilities still open?
```

---

# Example

```text id="closeout-commercial-example"
The original contract value was €1.8M.

Approved changes totalling €160,000 increased the adjusted
contract value to €1.96M.

The Supplier submitted a final account of €2.04M.

Following commercial review and reconciliation of outstanding
change requests, the agreed final value was €1.985M.

The final commercial position therefore represents a €25,000
increase above the adjusted contract value, primarily associated
with approved extended hypercare and additional migration support.
```

---

# Contingency Review

Where contingency exists, report:

```text id="closeout-contingency"
Original contingency

Contingency used

Contingency remaining

Main drivers of use
```

Example:

| Contingency | Amount |
|---|---:|
| Approved | €200,000 |
| Used | €125,000 |
| Remaining | €75,000 |

---

# Outstanding Commercial Items

Before final closure, confirm whether any remain:

```text id="closeout-commercial-open"
Unpaid invoices

Pending credits

Unresolved claims

Open change requests

Service credits

Retentions where applicable

Outstanding purchase orders

Disputed charges

Tax / currency adjustments
```

Provide:

| Item | Value | Owner | Required Action | Status |
|---|---:|---|---|---|

---

# Output 2 — Contract Close-Out Checklist

Organise the checklist by:

```text id="closeout-checklist-categories"
Commercial
Technical
Documentation
Security / Compliance
Operational Handover
Stakeholder / Acceptance
Internal Governance
```

---

# 1. Commercial Close-Out

Confirm:

- [ ] Final invoices received
- [ ] Approved changes reconciled
- [ ] Unapproved changes resolved
- [ ] Credits applied
- [ ] Service credits reviewed
- [ ] Outstanding claims resolved
- [ ] Purchase orders closed
- [ ] Final contract value confirmed
- [ ] Financial forecast updated
- [ ] Finance confirms no unexplained commitment remains

---

# 2. Technical Close-Out

Confirm:

- [ ] Contracted deliverables complete
- [ ] Final solution deployed
- [ ] Acceptance criteria achieved
- [ ] Critical defects resolved
- [ ] Remaining defects formally accepted
- [ ] Data migration completed
- [ ] Data reconciliation approved
- [ ] Integrations validated
- [ ] Performance requirements validated
- [ ] Technical debt accepted or transferred
- [ ] Final configuration recorded
- [ ] Production environment confirmed

---

# Defect Close-Out

For remaining defects provide:

| Defect | Severity | Business Impact | Owner | Resolution / Acceptance | Target Date |
|---|---|---|---|---|---|

Do not close the contract merely because unresolved defects have moved to another tracker.

They should have:

- ownership,
- agreed disposition,
- and documented acceptance where required.

---

# 3. Documentation Close-Out

Confirm delivery of required documents such as:

```text id="closeout-documents"
Solution architecture
Configuration documentation
Interface specifications
Data mappings
Test evidence
Security documentation
Deployment procedures
Operations manual
Support procedures
Runbooks
User documentation
Training material
Licence information
Asset register
Known-error documentation
```

Use:

| Document | Required | Delivered | Approved | Owner |
|---|---|---|---|---|

---

# Documentation Quality Rule

Do not mark documentation complete simply because a file exists.

Check:

```text id="closeout-document-quality"
Is it current?

Does it reflect the production solution?

Has the correct owner approved it?

Can Operations actually use it?

Is it stored in the agreed repository?
```

---

# 4. Security / Compliance Close-Out

Where relevant confirm:

- [ ] Final security assessment completed
- [ ] Penetration-test findings resolved or accepted
- [ ] Production access reviewed
- [ ] Privileged access confirmed
- [ ] Data-protection requirements satisfied
- [ ] Logging / monitoring enabled
- [ ] Security exceptions documented
- [ ] Compliance evidence archived
- [ ] Temporary project access removed

---

# Access Review

At close-out check:

```text id="closeout-access"
Temporary vendor accounts

Administrative access

Development access

Test accounts

Shared credentials

Third-party access

Expired project permissions
```

Temporary project access should not remain active unintentionally after handover.

---

# 5. Operational Handover

Confirm:

- [ ] Operational owner identified
- [ ] Support model agreed
- [ ] Support contacts documented
- [ ] Incident process agreed
- [ ] Monitoring active
- [ ] Backup / recovery confirmed
- [ ] SLA arrangements active
- [ ] Knowledge transfer complete
- [ ] Support team trained
- [ ] Hypercare exit criteria achieved
- [ ] Warranty / support period confirmed

---

# Operational Readiness Test

Ask:

```text id="closeout-ops-test"
If the project team left tomorrow:

Who would operate the solution?

Who would handle an incident?

Where is the runbook?

Who owns vendor escalation?

How would the service be restored?

Who owns future enhancements?
```

If these cannot be answered, handover may not be complete.

---

# 6. Stakeholder / Acceptance Close-Out

Confirm:

- [ ] Business acceptance completed
- [ ] Product Owner / Business Owner sign-off obtained
- [ ] Technical acceptance completed
- [ ] Operational acceptance completed
- [ ] Security approval completed
- [ ] Open exceptions documented
- [ ] Final stakeholder communication issued
- [ ] Benefits owner confirmed

---

# Formal Acceptance

Use:

```text id="closeout-acceptance"
Deliverable
Acceptance Authority
Acceptance Date
Conditions
Evidence
```

Example:

| Deliverable | Authority | Status | Evidence |
|---|---|---|---|
| CRM Production Release | Business Owner | Accepted | Signed acceptance record |
| Data Migration | Data Owner | Accepted | Reconciliation report |
| Security | CISO delegate | Approved | Security approval record |

---

# Conditional Acceptance

Where items remain open:

```text id="closeout-conditional"
Accepted subject to:

1. closure of Medium defect D-142,
2. completion of reporting documentation,
3. vendor resolution by 15 November.
```

The conditions should have owners and deadlines.

---

# 7. Internal Governance Close-Out

Confirm:

- [ ] Final project status report issued
- [ ] Risk register reviewed
- [ ] Issues transferred or closed
- [ ] Decisions archived
- [ ] Change register reconciled
- [ ] Lessons learned completed
- [ ] Project documentation archived
- [ ] Budget closed
- [ ] Resources released
- [ ] PMO closure requirements satisfied
- [ ] Benefits ownership transferred

---

# Risk and Issue Transfer

Not every risk disappears when the project closes.

Classify open items as:

```text id="closeout-risk-transfer"
Closed

Accepted

Transferred to Operations

Transferred to Product

Transferred to Vendor Management

Transferred to another project
```

Record:

| Item | New Owner | Transfer Date | Evidence |
|---|---|---|---|

---

# Hypercare Exit

Where hypercare is used, define exit criteria.

Possible criteria:

```text id="closeout-hypercare"
No Critical incidents open

Incident rate within agreed level

Business operations stable

Support team operating independently

Monitoring stable

Known issues transferred

Vendor support active
```

Do not end hypercare only because the calendar date has arrived.

---

# Vendor Performance Review

At contract close:

Assess:

```text id="closeout-vendor-review"
Delivery

Quality

Schedule

Commercial management

Communication

Resource stability

Technical capability

Support

Change management
```

Provide:

| Area | Assessment | Evidence | Future Recommendation |
|---|---|---|---|

Possible recommendation:

```text id="closeout-vendor-recommendations"
Preferred supplier

Suitable with conditions

Use only for specific services

Performance improvement required

Do not recommend for future work
```

Follow organisational procurement policy.

---

# Knowledge Transfer

Confirm that knowledge has moved from the project team to the long-term owner.

Use:

```text id="closeout-knowledge"
Project Team
↓
Operations / Product / Support
```

Check:

- documentation,
- walkthroughs,
- training,
- recordings where appropriate,
- access,
- ownership.

---

# Example Input

```text id="closeout-example-input"
Project:
CRM Replacement

Original Contract:
€1.8M

Approved Changes:
€160k

Adjusted Contract:
€1.96M

Supplier Final Submission:
€2.04M

Agreed Final Position:
€1.985M

Current Status:
Production live.
Hypercare complete.

Outstanding:
2 Medium defects accepted for BAU resolution.

Security:
Final approval received.

Documentation:
Technical documentation complete.
Operations runbook approved.

Support:
12-month vendor support now active.
```

---

# Example Commercial Narrative

## Final Commercial Position

The original CRM implementation contract was approved at **€1.8M**. Approved scope changes totalling **€160k** increased the adjusted contract value to **€1.96M**.

The Supplier submitted a final commercial position of **€2.04M**. Following reconciliation of change requests and final commercial review, the agreed contract value was **€1.985M**.

The final position is therefore **€25k above the adjusted contract value**. The remaining variance primarily reflects approved extended migration and hypercare support. No material unresolved commercial claims remain at the point of closure.

---

# Prompt 2 — Close-Out Readiness Review

```text id="closeout-readiness"
ROLE

You are an independent PMO and Commercial reviewer assessing
whether an IT project is ready for formal contract close-out.

TASK

Review the close-out information below.

[PASTE CLOSE-OUT STATUS]

Identify:

- incomplete commercial items,
- unaccepted deliverables,
- unresolved defects,
- missing documentation,
- security gaps,
- operational handover gaps,
- unresolved risks / issues,
- missing stakeholder approvals.

OUTPUT FORMAT

Close-Out Area
Gap
Why It Matters
Owner
Required Action
Blocking Close-Out?
```

---

# Prompt 3 — Final Account Reconciliation Review

```text id="closeout-finance-review"
ROLE

You are a senior IT Commercial Manager reviewing the final
commercial position of a supplier contract.

TASK

Review the financial data below.

[PASTE DATA]

Reconcile:

Original Contract
Approved Changes
Adjusted Contract
Invoices
Credits
Claims
Contingency
Supplier Final Submission
Agreed Final Position

Flag:

- unexplained variance,
- duplicate charges,
- unresolved changes,
- unapproved costs,
- missing credits.

Do not invent financial values.
```

---

# Prompt 4 — Handover Gap Analysis

```text id="closeout-handover-gap"
ROLE

You are an IT Service Transition Manager.

TASK

Review the project handover package below.

[PASTE PACKAGE]

Check:

- operational ownership,
- documentation,
- monitoring,
- support,
- incident management,
- access,
- backup / recovery,
- known issues,
- vendor support,
- knowledge transfer.

OUTPUT FORMAT

Gap
Operational Risk
Required Action
Owner
Priority
```

---

# Agile / Scrum Considerations

Project or contract close-out may occur even when the product continues evolving.

Separate:

```text id="closeout-agile"
Project / Contract Closure
```

from:

```text id="closeout-product"
Ongoing Product Development
```

Transfer:

- backlog ownership,
- technical debt,
- known issues,
- product roadmap,
- benefits ownership.

---

# Kanban / Managed Service Considerations

For ongoing services confirm:

- service ownership,
- WIP policies,
- support queues,
- SLA / SLE,
- escalation,
- reporting,
- capacity ownership.

The project may close while the service continues.

---

# Predictive Considerations

Formal acceptance and baseline completion may play a larger role.

Confirm:

- deliverables,
- milestones,
- change reconciliation,
- final schedule position,
- final budget.

---

# Hybrid Considerations

Close the formal project governance while ensuring adaptive delivery and product ownership continue appropriately.

---

# Close-Out Timeline

Do not wait until the final week.

Recommended flow:

```text id="closeout-timeline"
Before Handover
↓
Identify closure requirements
↓
Track documentation / acceptance
↓
Resolve commercial items
↓
Complete operational readiness
↓
Formal acceptance
↓
Final reconciliation
↓
Project / Contract closure
```

For complex programmes, begin close-out planning well before the target handover.

---

# Closure Decision

Use:

```text id="closeout-decision"
Ready to Close

Ready to Close with Conditions

Not Ready to Close
```

Provide rationale.

---

# Quality Checklist

Before formal contract closure, confirm:

- [ ] Final commercial value reconciled
- [ ] All approved changes included
- [ ] Unapproved charges resolved
- [ ] Deliverables accepted
- [ ] Critical defects closed
- [ ] Remaining defects formally transferred
- [ ] Documentation complete
- [ ] Security approval complete
- [ ] Operational ownership established
- [ ] Support arrangements active
- [ ] Access reviewed
- [ ] Risks and issues closed or transferred
- [ ] Stakeholder acceptance documented
- [ ] Lessons learned captured
- [ ] Project records archived
- [ ] Financial commitments closed
- [ ] Contract closure approval obtained

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- project closure,
- procurement closure,
- financial management,
- quality,
- stakeholder acceptance,
- transition,
- lessons learned,
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

Contract close-out should involve appropriate stakeholders such as:

- Project Manager
- Commercial / Procurement
- Finance
- Business Owner
- Technical Lead
- Security
- Operations / Support
- Vendor Manager
- PMO
- Legal where required

AI can help identify missing closure activities and structure the final narrative.

It cannot formally accept deliverables, settle commercial claims, or close a contract on behalf of authorised stakeholders.

---

# Confidentiality

Close-out documentation may contain:

- final contract values,
- supplier performance,
- settlement information,
- security details,
- unresolved commercial matters,
- customer information.

Protect this information according to organisational policy.

---

# Prompt Metadata

```text id="closeout-metadata"
Prompt ID: COMM-006
Category: Commercial & Project Governance
Version: 1.0
Status: Draft
Owner: Project Manager / Commercial Manager
Reviewer: Finance / Procurement / Business Owner
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
| 1.0 | YYYY-MM-DD | Initial IT contract close-out framework |
