# Contract Clause Analysis

## Purpose

Use this prompt to convert a complex contract clause into a structured, project-management-focused analysis.

The objective is to help the Project Manager understand:

- what the clause means,
- what each party is required to do,
- what delivery or commercial risks it creates,
- what deadlines or conditions matter,
- and where disputes or misunderstandings may arise.

This prompt is intended for **project and commercial awareness**, not legal interpretation or legal advice.

---

## Best Used For

**Project phase:**  
Procurement / Contracting / Delivery / Change / Escalation / Close-Out

**Project type:**  
Software implementation / SaaS / Cloud / ERP / Infrastructure / Outsourcing / Managed Service / Digital Transformation

**Primary user:**  
Project Manager / Delivery Manager / Vendor Manager / PMO / Commercial Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
When reviewing clauses that materially affect delivery, cost, scope, risk, or governance

---

# Prompt

```text id="contract-clause-01"
ROLE

You are a senior IT Commercial and Project Management specialist
experienced in software delivery, SaaS agreements, vendor contracts,
technology procurement, service management, and project governance.

TASK

Analyse the contract clause below for a Project Manager.

CONTRACT CONTEXT

Contract type:
[SOFTWARE IMPLEMENTATION / SAAS / CLOUD / OUTSOURCING / OTHER]

Customer / Client:
[ROLE]

Supplier / Vendor:
[ROLE]

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Relevant commercial context:
[DETAILS]

CLAUSE

[PASTE CLAUSE]

OUTPUT FORMAT

Provide:

1. Plain-English Summary
2. Customer / Client Obligations
3. Supplier / Vendor Obligations
4. Key Deadlines / Conditions / Triggers
5. Project Delivery Implications
6. Commercial Risks for the Customer
7. Commercial Risks for the Supplier
8. Common Areas of Dispute or Ambiguity
9. Questions the Project Manager Should Clarify
10. Recommended Project Controls

Use professional but accessible language.

Do not invent contractual rights or obligations that are not
supported by the clause.
```

---

# 1. Plain-English Summary

Explain the clause in 2–4 sentences.

The summary should answer:

```text id="clause-summary-questions"
What does this clause allow or require?

Who must do what?

Under what conditions?

What happens if the condition is not met?
```

Avoid simply rewriting the clause using different legal terminology.

---

# Example

### Clause Concept

Supplier must notify the customer within ten business days if a customer-caused dependency is likely to affect the agreed implementation schedule.

### Plain-English Summary

```text id="clause-summary-example"
The supplier must formally notify the customer within ten business
days when a customer-controlled dependency is likely to delay delivery.

If the supplier does not follow the required notification process,
its ability to rely on the delay for schedule relief may be affected,
depending on the wider contract terms.
```

Note:

Do not claim loss of entitlement unless the actual contract supports that conclusion.

---

# 2. Customer / Client Obligations

Identify obligations explicitly created by the clause.

Possible examples:

```text id="client-obligations"
Provide information

Provide system access

Approve deliverables

Make decisions

Provide resources

Review submissions

Pay invoices

Respond within defined periods

Provide environments

Maintain dependencies
```

Use:

| Obligation | Trigger | Deadline | Delivery Relevance |
|---|---|---|---|

---

# 3. Supplier / Vendor Obligations

Possible obligations include:

```text id="supplier-obligations"
Deliver agreed services

Meet milestones

Provide notification

Maintain service levels

Resolve defects

Provide documentation

Protect information

Support audits

Escalate incidents

Provide transition assistance
```

Use:

| Obligation | Trigger | Deadline | Evidence Required |
|---|---|---|---|

---

# 4. Key Deadlines, Conditions and Triggers

Extract any timing or procedural requirements.

Look for:

```text id="contract-triggers"
Notice periods

Approval periods

Response deadlines

Cure periods

Renewal dates

Termination windows

Payment deadlines

Escalation triggers

Acceptance periods

SLA measurement periods
```

Provide:

| Trigger | Required Action | Deadline | Responsible Party | Consequence if Missed |
|---|---|---|---|---|

Only state the consequence where the contract supports it.

---

# 5. Project Delivery Implications

Translate the clause into operational project-management meaning.

Ask:

```text id="delivery-implications"
Does this affect schedule?

Does this affect acceptance?

Does this affect scope?

Does this affect change control?

Does this affect vendor performance?

Does this affect release?

Does this affect payment?

Does this create a dependency?
```

Example:

> The ten-business-day notice requirement means dependency delays should be monitored through the RAID process so that potential contractual notifications are not identified too late.

---

# Contract-to-Project Translation

Use:

```text id="contract-project-flow"
Contract Requirement
↓
Project Trigger
↓
Project Control
↓
Evidence
↓
Escalation if Required
```

Example:

```text id="contract-project-example"
Contract:
Customer approval required within 5 business days.

Project Control:
Approval tracker.

Evidence:
Documented submission and approval timestamps.

Escalation:
Escalate unresolved approval on Day 4.
```

---

# 6. Customer Commercial Risks

Possible areas to consider:

```text id="customer-risks"
Unclear acceptance criteria

Unexpected licence costs

Vendor lock-in

Weak SLA remedies

Delayed approvals

Data portability

Exit costs

Change-control exposure

Minimum consumption commitments

Automatic renewal
```

Do not assume these exist unless supported by the clause or wider contract context.

---

# 7. Supplier Commercial Risks

Possible areas:

```text id="supplier-risks"
Unclear customer dependencies

Unlimited change expectation

Ambiguous acceptance

Uncontrolled scope

Delayed payment

Resource commitments

Service-credit exposure

Unclear responsibilities
```

Again, distinguish actual clause-derived risk from general possibilities.

---

# 8. Ambiguity / Dispute Analysis

Look for wording that may create different interpretations.

Examples:

```text id="contract-ambiguity"
Reasonable effort

Material delay

Promptly

Substantial compliance

Appropriate support

Acceptable performance

Customer-caused delay
```

For each:

| Ambiguous Term | Possible Interpretations | Project Risk | Clarification Needed |
|---|---|---|---|

---

# 9. Questions for the Project Manager

Generate clarification questions such as:

```text id="contract-pm-questions"
Who owns the notification process?

What evidence proves the trigger date?

Who is authorised to issue formal notices?

Which repository stores contractual correspondence?

Does the clause interact with another clause?

How is acceptance confirmed?

Who approves contractual changes?

What happens if the required response is late?
```

These questions should help the PM operationalise the clause.

---

# 10. Recommended Project Controls

Possible controls include:

```text id="contract-controls"
Contract obligations register

Notice tracker

Approval tracker

Decision log

Change log

SLA dashboard

Deliverable acceptance register

Vendor action tracker

Renewal calendar

Dependency register
```

Do not introduce controls that add bureaucracy without management value.

---

# Example Input

```text id="contract-example-input"
Contract Type:
Software Implementation Agreement

Clause:
The Customer shall review each Deliverable within five Business Days
of receipt and either approve it or provide written details of any
material non-conformance with the agreed Acceptance Criteria.

If no response is received within that period, the Deliverable shall
be deemed accepted.
```

---

# Example Analysis

## Plain-English Summary

The customer has five business days to review each submitted deliverable against the agreed acceptance criteria. If the customer does not approve or reject it within that period, the clause states that the deliverable is treated as accepted.

## Customer Obligation

The customer must complete the review within five business days and document any material non-conformance.

## Supplier Obligation

The supplier must submit a deliverable that can be assessed against the agreed acceptance criteria.

## Project Delivery Implication

The Project Manager should track submission and response dates because missed review deadlines may result in deemed acceptance.

## Project Control

Maintain a deliverable acceptance register containing:

```text id="acceptance-register"
Deliverable
Submission Date
Acceptance Deadline
Reviewer
Status
Comments
Final Decision
```

---

# Prompt 2 — Clause Risk Review

```text id="contract-risk-review"
ROLE

You are a senior IT Commercial Manager reviewing a contract clause
for delivery risk.

TASK

Review the clause and identify project-management risks.

[PASTE CLAUSE]

OUTPUT FORMAT

Clause Requirement
Potential Failure Scenario
Project Impact
Commercial Impact
Preventive Control
Owner
Evidence Required
```

---

# Prompt 3 — Clause Dependency Review

```text id="contract-dependency"
ROLE

You are an IT Project Manager mapping contractual obligations into
project dependencies.

TASK

Analyse the clause below and identify dependencies between the
customer and supplier.

[PASTE CLAUSE]

OUTPUT FORMAT

Dependency
Providing Party
Receiving Party
Required By
Impact if Late
Project Control
Escalation Trigger
```

---

# Prompt 4 — Clause Comparison

Where two contract versions exist:

```text id="contract-comparison"
ROLE

You are a senior IT Commercial Manager.

TASK

Compare the two versions of the clause below.

VERSION A

[PASTE]

VERSION B

[PASTE]

Identify:

1. Wording changes
2. Obligation changes
3. Deadline changes
4. Risk allocation changes
5. Commercial impact
6. Project-management impact

Do not assume legal significance beyond the text provided.
```

---

# Common IT Clauses Worth Reviewing

Examples include:

```text id="contract-clauses"
Scope and Deliverables
Acceptance
Change Control
Milestones
Payment
Service Levels
Availability
Incident Management
Data Protection
Security
Intellectual Property
Confidentiality
Subcontracting
Liability
Termination
Exit Assistance
Renewal
Audit Rights
Customer Dependencies
Force Majeure
```

The relevant clauses depend on the specific contract.

---

# SaaS Considerations

For SaaS agreements, pay particular attention to:

- availability,
- service credits,
- data ownership,
- data portability,
- retention,
- security,
- renewal,
- termination,
- usage limits,
- support.

---

# Cloud Considerations

Consider:

- consumption commitments,
- data region,
- service availability,
- shared-responsibility model,
- price changes,
- portability,
- exit costs.

---

# Implementation Contract Considerations

Consider:

- scope,
- milestones,
- dependencies,
- acceptance,
- change control,
- resource commitments,
- delay,
- payment.

---

# Agile / Scrum Considerations

Contract terms should support the intended delivery model.

Potential tension can arise where:

```text id="contract-agile-tension"
Contract:
Fixed detailed scope.

Delivery Model:
Adaptive backlog prioritisation.
```

Flag this tension where relevant.

Do not assume Agile delivery removes contractual obligations.

---

# Kanban / Managed Service Considerations

For ongoing service delivery, clauses may relate to:

- SLAs,
- service requests,
- prioritisation,
- response times,
- resolution times,
- service capacity,
- support windows.

Project and service-management responsibilities should be clearly distinguished.

---

# Predictive Considerations

Contractual milestones, deliverable acceptance, and formal change control may directly influence the project baseline.

---

# Hybrid Considerations

Clearly distinguish:

```text id="contract-hybrid"
Fixed commercial boundaries
+
Adaptive delivery mechanisms
```

The Project Manager should understand which elements can change operationally and which require contractual approval.

---

# Contract Obligations Register

For complex projects, maintain:

| ID | Clause | Obligation | Party | Trigger | Deadline | Owner | Evidence | Status |
|---|---|---|---|---|---|---|---|---|

This makes contract obligations visible within delivery governance.

---

# Important AI Rule

Never ask AI to assume that a clause creates:

- a legal entitlement,
- a waiver,
- a contractual breach,
- a right to terminate,
- liability,
- damages,

unless the contract text and professional legal review support that conclusion.

Use AI to support understanding and issue spotting.

Do not use it as the final legal authority.

---

# Recipient / Counterparty Challenge

After analysis, run:

```text id="contract-counterparty"
ROLE

You represent the counterparty to the contract clause below.

TASK

Challenge the interpretation provided.

CLAUSE

[PASTE]

INTERPRETATION

[PASTE]

Identify:

- unsupported assumptions,
- alternative interpretations,
- missing conditions,
- missing dependencies,
- wording that requires legal clarification.

Do not invent terms outside the clause.
```

This helps expose one-sided interpretations before formal communication.

---

# Quality Checklist

Before relying on the analysis, confirm:

- [ ] Original clause text is complete
- [ ] Plain-English summary matches the text
- [ ] Obligations are separated by party
- [ ] Deadlines are identified
- [ ] Conditions and triggers are visible
- [ ] Project implications are understood
- [ ] Actual requirements are separated from assumptions
- [ ] Ambiguities are highlighted
- [ ] Required project controls are identified
- [ ] Legal interpretation has not been invented
- [ ] Related clauses have been checked where necessary
- [ ] Legal / Procurement review is requested where appropriate

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- procurement,
- commercial management,
- stakeholder responsibilities,
- risk,
- governance,
- change management,
- vendor management.

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

Material contractual analysis should be reviewed with appropriate stakeholders such as:

- Legal
- Procurement
- Commercial Management
- Project Manager
- Vendor Manager
- Information Security
- Data Protection

AI can help explain wording and identify project-management implications.

It is not a substitute for qualified legal advice.

---

# Confidentiality

Contracts often contain highly sensitive commercial information.

Do not enter confidential contract text into public AI tools unless organisational policy permits it.

Protect:

- pricing,
- liability terms,
- negotiated concessions,
- security terms,
- vendor information,
- personal data,
- proprietary commercial terms.

Use redacted or anonymised text where appropriate.

---

# Prompt Metadata

```text id="contract-metadata"
Prompt ID: COMM-001
Category: Commercial & Project Governance
Version: 1.0
Status: Draft
Owner: Project Manager / Commercial Manager
Reviewer: Legal / Procurement
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
| 1.0 | YYYY-MM-DD | Initial IT contract-clause analysis framework |
