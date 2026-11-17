# Contractual Claim / Formal Notification

## Purpose

Use this prompt to prepare a structured contractual notification when an event may create:

- schedule impact,
- additional cost,
- scope impact,
- resource impact,
- or another contractual consequence.

Typical IT examples may include:

- customer-caused delay,
- delayed access or environment availability,
- late approval,
- scope expansion,
- dependency failure,
- delayed third-party integration,
- additional work outside the agreed scope,
- suspension or interruption,
- vendor-caused milestone delay.

The purpose is to create a **factual and traceable draft for commercial and legal review**.

It is not a substitute for legal advice.

---

## Best Used For

**Project phase:**  
Contracting / Delivery / Change / Escalation

**Project type:**  
Software implementation / SaaS / ERP / Cloud / Outsourcing / Managed Service / Digital Transformation

**Primary user:**  
Project Manager / Delivery Manager / Commercial Manager / Vendor Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
When a contract-relevant event occurs

---

# Prompt

```text id="claim-notice-01"
ROLE

You are a senior IT Commercial and Project Management specialist
experienced in software delivery, technology contracts, vendor
management, commercial governance, and formal project correspondence.

TASK

Draft a formal contractual notification based only on the facts
provided below.

Do not invent contractual rights, clause references, notice periods,
entitlements, or remedies.

CONTRACT CONTEXT

Project:
[PROJECT NAME]

Contract:
[CONTRACT NAME / TYPE]

Customer:
[PARTY]

Supplier:
[PARTY]

Relevant clause(s):
[PASTE VERIFIED CLAUSE REFERENCES]

Notice requirements:
[PASTE VERIFIED REQUIREMENTS]

Event:
[DESCRIBE EVENT]

Date event occurred:
[DATE]

Date project became aware:
[DATE]

Previous notice:
[DETAILS / NONE]

Schedule impact:
[DETAILS]

Cost impact:
[DETAILS]

Scope impact:
[DETAILS]

Evidence:
[LIST]

Mitigation / recovery actions:
[LIST]

Remedy / relief being requested:
[DETAILS]

OUTPUT FORMAT

Draft a formal notification with:

1. Reference and Subject
2. Purpose of Notice
3. Relevant Contractual Basis
4. Factual Description of Event
5. Chronology
6. Current Impact
7. Mitigation / Recovery Actions
8. Relief / Action Requested
9. Supporting Evidence
10. Reservation / Next Steps where appropriate
11. Professional Close

Tone:
Formal
Contractual
Factual
Non-adversarial
Precise
```

---

# Core Principle

Use:

```text id="claim-flow"
Contract Requirement
↓
Event
↓
Evidence
↓
Impact
↓
Mitigation
↓
Relief / Action Requested
```

Avoid:

```text id="claim-bad-flow"
Complaint
↓
Blame
↓
Unsupported entitlement
↓
Aggressive demand
```

---

# 1. Reference and Subject

Use a precise subject.

### Weak

```text id="claim-subject-weak"
Project Delay
```

### Better

```text id="claim-subject-good"
Formal Notice — Customer Access Delay Affecting System Integration Milestone
```

Or:

```text id="claim-subject-example"
Contractual Notice — Additional Scope and Associated Schedule / Cost Impact
```

Where a verified clause applies:

```text id="claim-subject-clause"
Formal Notice under Clause [X] — [EVENT]
```

Never invent the clause number.

---

# 2. Purpose of Notice

State why the communication is being issued.

Example:

```text id="claim-purpose"
This notice is issued to formally record the delay to the integration
workstream arising from the late provision of the required production-
equivalent test environment and to notify the Customer of the current
schedule impact.
```

Avoid unnecessary background in the opening.

---

# 3. Contractual Basis

Reference only verified clauses.

Use:

```text id="claim-basis"
Relevant Clause:
[CLAUSE]

Requirement:
[PLAIN-LANGUAGE SUMMARY BASED ON CLAUSE]

Notice Requirement:
[IF VERIFIED]
```

Do not state:

> We are automatically entitled to compensation.

unless qualified legal/commercial review confirms this.

Prefer:

> Based on the current contractual assessment, this event may give rise to relief under Clause [X], subject to the applicable contractual requirements and formal review.

---

# 4. Factual Description

State:

```text id="claim-facts"
What was required
Who was responsible
Required date
Actual position
Date discovered
Current status
```

Example:

> The Customer was due to provide access to the production-equivalent integration environment by 10 May. Access was provided on 24 May, creating a fourteen-calendar-day delay to the planned start of end-to-end integration testing.

Keep the language factual.

---

# 5. Chronology

Use a chronological table.

| Date | Event | Evidence / Reference |
|---|---|---|
| 10 May | Contractual / planned environment date | Approved project plan |
| 11 May | Delay raised in project meeting | Meeting minutes |
| 14 May | Formal follow-up issued | Email reference |
| 24 May | Access provided | Access confirmation |

This strengthens traceability.

---

# 6. Impact Assessment

Assess only supported impact.

Possible dimensions:

```text id="claim-impact"
Schedule
Cost
Resource
Scope
Testing
Release
Operations
Commercial
```

Provide:

| Impact Area | Current Assessment | Evidence |
|---|---|---|

---

# Schedule Impact

Explain:

```text id="claim-schedule"
Affected activity

Original date

Current / forecast date

Duration of impact

Downstream dependency

Recovery potential
```

Example:

> The delayed environment availability prevented end-to-end testing from starting for ten working days. The current forecast shows a five-working-day impact to the UAT start after partial recovery through resequencing.

---

# Cost Impact

Where relevant:

```text id="claim-cost"
Additional vendor effort

Extended resource mobilisation

Additional cloud / environment cost

Rework

Idle time

Acceleration cost
```

If cost is not yet known:

> Cost impact is currently under assessment and will be provided when supporting evidence is available.

Do not fabricate values.

---

# 7. Mitigation and Recovery

Demonstrate reasonable management action.

Examples:

```text id="claim-mitigation"
Re-sequenced unaffected work

Used mock services

Reallocated internal resources

Conducted parallel testing

Added recovery checkpoints

Requested accelerated approval
```

Example:

> The project team has resequenced eligible integration activities and continued testing through the approved mock environment to reduce the schedule impact.

---

# 8. Relief / Action Requested

Be explicit.

Possible requests include:

```text id="claim-request"
Confirm revised milestone

Approve schedule adjustment

Approve change request

Acknowledge event

Provide missing dependency

Approve additional cost

Confirm responsibility

Attend commercial review
```

Example:

```text id="claim-request-example"
The Supplier requests formal acknowledgement of the event and
agreement to review the resulting schedule impact through the
contractual change-control process.
```

---

# Specificity Rule

### Weak

```text id="claim-request-weak"
Please advise.
```

### Better

```text id="claim-request-good"
Please confirm by 18 June whether the Customer accepts the proposed
five-working-day revision to the UAT milestone so that the integrated
project schedule can be updated.
```

---

# 9. Evidence

Reference supporting records.

Possible evidence:

```text id="claim-evidence"
Approved schedule
Contract clause
Meeting minutes
Email correspondence
Decision log
Access records
System logs
Timesheets
Vendor quotations
Change request
Test records
```

Use:

| Evidence ID | Description | Date |
|---|---|---|

---

# Evidence Principle

A contractual position is stronger when supported by contemporaneous project records.

This makes disciplined project documentation commercially important.

---

# 10. Notice Period Check

Before issuing any formal notification, confirm:

```text id="claim-notice-check"
What event triggered the notice?

When did the event occur?

When did the project become aware?

What notice period applies?

Who must receive the notice?

What delivery method is contractually required?

Is acknowledgement required?

Is evidence of delivery retained?
```

Do not rely on AI to calculate a legal deadline unless the applicable clause and dates have been verified.

---

# Formal Notice Tracker

For complex contracts maintain:

| Notice ID | Event | Clause | Trigger Date | Notice Deadline | Date Issued | Recipient | Delivery Evidence | Status |
|---|---|---|---|---|---|---|---|---|

This reduces the risk of missing contractual procedures.

---

# Example Input

```text id="claim-example-input"
Project:
CRM Implementation

Contract:
Software Implementation Agreement

Event:
Customer production-equivalent integration environment was provided
late.

Required Date:
10 May

Actual Date:
24 May

Impact:
Integration testing started 10 working days late.

Recovery:
Team used mock services and resequenced unaffected tests.

Current Forecast:
5 working days impact to UAT.

Relevant Clause:
Clause 8.3 — Customer Dependencies

Notice Requirement:
Written notice within 10 business days of becoming aware of the
dependency delay.

Evidence:
Approved schedule
Environment request log
Meeting minutes
Access confirmation

Requested Action:
Acknowledge event and review schedule adjustment through formal
change control.
```

---

# Example Output

## Subject

**Formal Notice — Delay in Customer Integration Environment Availability**

Dear [Name],

This notice is issued in relation to the delayed availability of the production-equivalent integration environment required for the CRM implementation project.

Under Clause 8.3 of the Agreement, the Customer is responsible for providing the identified project dependencies in accordance with the agreed delivery schedule. The environment was required by 10 May and became available on 24 May.

The delay prevented the planned start of end-to-end integration testing. Following resequencing and use of the approved mock environment, the current forecast indicates a five-working-day impact to the planned UAT start.

The project team continues to implement recovery actions to minimise the schedule impact. We request formal acknowledgement of the event and confirmation that the resulting schedule impact will be reviewed through the contractual change-control process.

Supporting project records, including the approved schedule, environment request history, and access confirmation, are available for review.

Kind regards,  
[Project Manager]

---

# Prompt 2 — Claim / Notice Quality Review

```text id="claim-review"
ROLE

You are an independent IT Commercial Manager reviewing a draft
contractual notification.

TASK

Review the draft below.

[PASTE DRAFT]

Check for:

- unsupported entitlement statements,
- incorrect or unsupported clause references,
- missing notice dates,
- missing evidence,
- unclear chronology,
- unquantified impact,
- unsupported cost claims,
- emotional or adversarial language,
- unclear requested action,
- missing deadline.

OUTPUT FORMAT

Finding
Why It Matters
Required Correction
Reviewer
Priority
```

---

# Prompt 3 — Counterparty Challenge

```text id="claim-counterparty"
ROLE

You represent the contractual counterparty receiving the
notification below.

TASK

Challenge the notification.

[PASTE DRAFT]

Identify:

- facts that may be disputed,
- missing evidence,
- alternative causation,
- mitigation questions,
- chronology gaps,
- unsupported entitlement,
- unclear impact calculations.

Do not invent contract terms.

OUTPUT FORMAT

Challenge
Basis
Evidence Required
Potential Weakness
Recommended Response Preparation
```

This helps identify weaknesses before formal issue.

---

# Causation Review

For significant claims, distinguish:

```text id="claim-causation"
Event
↓
Affected Activity
↓
Actual Delay / Cost
↓
Downstream Impact
```

Do not assume:

```text id="claim-causation-bad"
Event occurred
=
Entire project delay
```

The impact should be supported by evidence.

---

# Concurrent Causes

Where more than one factor may have contributed:

```text id="claim-concurrency"
Customer dependency delay
+
Supplier defect
+
Resource shortage
```

flag this for commercial / legal review.

Do not present a single cause as definitive when evidence shows multiple contributing factors.

---

# Change-Control Integration

A formal notification does not automatically replace project change control.

Where applicable:

```text id="claim-change-flow"
Event
↓
Notice
↓
Impact Assessment
↓
Change Request
↓
Commercial Review
↓
Approval / Rejection
↓
Baseline Update
```

---

# Agile / Scrum Considerations

Adaptive delivery does not remove contractual requirements.

Potential contract-relevant events may include:

- customer dependencies,
- unavailable Product Owner decisions,
- agreed release commitments,
- supplier capacity commitments,
- scope outside agreed commercial boundaries.

Distinguish normal backlog reprioritisation from a contractual change.

---

# Kanban / Managed Service Considerations

Potential evidence may include:

- SLA breaches,
- work-item ageing,
- blocked service requests,
- response-time data,
- throughput history.

Use operational metrics as evidence only when contractually relevant.

---

# Predictive Considerations

Formal claims may link closely to:

- baseline milestones,
- critical path,
- contractual dates,
- change control,
- resource or cost impact.

---

# Hybrid Considerations

Separate:

```text id="claim-hybrid"
Adaptive delivery change
```

from:

```text id="claim-hybrid-contract"
Commercial / contractual change
```

Not every delivery adjustment requires a contractual claim.

---

# Writing Rules

Use:

```text id="claim-writing-rules"
Professional
Factual
Specific
Traceable
Non-adversarial
Evidence-based
```

Avoid:

```text id="claim-writing-avoid"
Clearly your fault

We demand

This is completely unacceptable

You have caused the entire project delay

As everyone knows
```

unless such wording has been intentionally approved by Legal / Commercial.

---

# Quality Checklist

Before issuing a formal notice, confirm:

- [ ] Contract version is correct
- [ ] Clause references are verified
- [ ] Event date is correct
- [ ] Awareness date is correct
- [ ] Notice deadline is verified
- [ ] Correct recipient is identified
- [ ] Required delivery method is verified
- [ ] Facts are evidence-based
- [ ] Chronology is clear
- [ ] Impact is supported
- [ ] Mitigation is recorded
- [ ] Relief requested is explicit
- [ ] No unsupported legal entitlement is claimed
- [ ] Commercial / Legal review completed where required
- [ ] Delivery evidence will be retained

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- procurement,
- change management,
- schedule,
- cost,
- risk,
- stakeholder communication,
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

Formal contractual notifications should normally be reviewed by the appropriate:

- Legal team,
- Commercial Manager,
- Procurement,
- Project Manager,
- Programme Manager,
- Vendor Manager.

AI can help structure the draft and identify missing information.

It should not determine legal entitlement, contractual liability, or final claim strategy.

---

# Confidentiality

Formal claims may contain highly sensitive information.

Protect:

- pricing,
- legal positions,
- contract clauses,
- commercial negotiations,
- dispute strategy,
- vendor performance information,
- customer information.

Do not paste confidential contract or dispute material into public AI tools unless organisational policy permits it.

---

# Prompt Metadata

```text id="claim-metadata"
Prompt ID: COMM-002
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
| 1.0 | YYYY-MM-DD | Initial IT contractual claim / formal notification framework |
