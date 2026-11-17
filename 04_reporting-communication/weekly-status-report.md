# Weekly Project Status Report

## Purpose

Use this prompt to convert rough weekly project notes into a concise, structured, management-ready status report.

The report should help stakeholders understand:

- current overall status,
- what progressed this week,
- which risks and issues require attention,
- what is planned next,
- and which decisions or actions are required.

The objective is not to reproduce every project activity.

The objective is to communicate the information required for **management awareness, action, and decision-making**.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment / Hypercare

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Project Coordinator / Delivery Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Weekly

---

# Prompt

```text id="weekly-status-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, stakeholder communication, risk management,
project governance, and executive reporting.

TASK

Create a professional weekly project status report from the rough
project notes below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Reporting period:
[DATE RANGE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target milestone / release:
[MILESTONE / DATE]

Overall status:
[IF ALREADY ASSESSED]

ROUGH WEEKLY NOTES

[PASTE RAW NOTES HERE]

The notes may contain:

- progress,
- milestones,
- delivery metrics,
- blockers,
- risks,
- issues,
- defects,
- dependencies,
- vendor updates,
- budget information,
- decisions,
- stakeholder actions,
- next steps.

Do not invent missing information.

OUTPUT FORMAT

Create the report with:

1. Project Status Summary
2. This Week's Progress
3. Key Risks and Issues
4. Next Week's Priorities
5. Decisions / Actions Required
```

---

# 1. Project Status Summary

Provide:

```text id="weekly-rag"
Overall RAG Status:
GREEN / AMBER / RED

One-Sentence Rationale:
[WHY]
```

Then provide a concise management summary of no more than 3–4 sentences.

The summary should explain:

- current delivery position,
- most important progress,
- main concern,
- whether management action is required.

---

# RAG Principles

## Green

Use when:

```text id="weekly-green"
Key commitments remain achievable.

No material unresolved risk currently threatens the target.

Issues are being managed within agreed project tolerance.
```

## Amber

Use when:

```text id="weekly-amber"
A material risk or issue exists.

The target remains achievable but requires active management,
recovery action, or a timely decision.
```

## Red

Use when:

```text id="weekly-red"
A major commitment is no longer achievable under the current plan,
or material impact exceeds agreed project tolerance.
```

Do not assign RAG status based only on subjective tone.

Use available evidence.

---

# Evidence-Based RAG Check

Before assigning or validating the status, review:

```text id="weekly-rag-evidence"
Schedule
Scope
Budget
Quality
Risks
Issues
Dependencies
Vendor performance
Security / compliance
Release readiness
Business readiness
```

Where the available evidence conflicts with the stated status, flag it.

Example:

```text id="weekly-rag-conflict"
Reported Status:
Green

Evidence:
Critical integration dependency is already two weeks late.

Recommendation:
Review overall status — Amber may be more appropriate.
```

---

# 2. This Week's Progress

Use concise bullets focused on completed or materially advanced work.

Preferred style:

```text id="weekly-progress-good"
- CRM configuration reached 85% completion.
- Identity integration passed functional testing.
- UAT test scripts were approved by the Business Owner.
- Security pre-review completed with two actions remaining.
```

Avoid activity-only reporting such as:

```text id="weekly-progress-weak"
- Attended meetings.
- Discussed testing.
- Followed up with vendor.
```

Report outcomes rather than effort where possible.

---

# 3. Key Risks and Issues

Provide:

| Type | Risk / Issue | Impact | Current Action | Owner | Due |
|---|---|---|---|---|---|

Use:

```text id="weekly-risk-type"
Risk
Issue
Dependency
Blocker
```

Do not mix future uncertainty and already-materialised problems without identifying the type.

---

# Risk / Issue Reporting Rule

Each material item should answer:

```text id="weekly-risk-questions"
What is happening?

Why does it matter?

What is being done?

Who owns the action?

When is the next meaningful deadline?
```

---

# 4. Next Week's Priorities

Identify the most important planned outcomes for the next reporting period.

Examples:

```text id="weekly-next"
Complete identity-provider certification.

Close remaining Severity 1 integration defect.

Confirm named UAT testers.

Submit security evidence package.

Approve release-readiness checklist.
```

Prefer outcomes over generic activity.

---

# 5. Decisions / Actions Required

This section is especially important for governance.

Provide:

| Decision / Action | Required From | Why Required | Deadline | Impact if Delayed |
|---|---|---|---|---|

Examples:

```text id="weekly-decision-examples"
Approve additional vendor capacity.

Confirm release-scope reduction.

Approve budget contingency usage.

Confirm UAT business resources.

Accept residual security risk.

Approve revised milestone.
```

Do not hide management decisions inside narrative text.

---

# Decision Quality Rule

A decision request should contain:

```text id="weekly-decision-structure"
Decision required
+
Decision owner
+
Recommendation where appropriate
+
Decision deadline
+
Impact if delayed
```

### Weak

```text id="weekly-decision-weak"
Sponsor input required.
```

### Better

```text id="weekly-decision-good"
Decision Required:
Approve two additional vendor developers.

Decision Owner:
Project Sponsor.

Deadline:
Friday.

Impact if Delayed:
Current recovery plan will not protect the planned UAT start.
```

---

# Example Input

```text id="weekly-example-input"
Project:
Customer Portal

Reporting Period:
7–11 June

Delivery Approach:
Hybrid Agile

Overall:
Amber

Notes:
- portal frontend 90% done
- identity provider certification 10 days late
- mock authentication service now working
- 2 critical integration defects, one fixed today
- business confirmed 6 of 8 UAT testers
- security evidence 70% complete
- vendor recovery plan received, proposes certification next Friday
- budget still on plan
- next week: complete certification, close critical defects,
  confirm UAT testers, complete security package
- sponsor needs to decide whether to add two temporary vendor developers
```

---

# Example Output

## Project Status Summary

**Overall Status: Amber**

The project remains on track for the planned release, but the delayed identity-provider certification continues to create integration and UAT schedule risk. A working mock authentication service is allowing eligible testing to continue, and one of two critical defects has been resolved. The vendor has submitted a recovery plan, but additional capacity may be required to protect the UAT start.

---

## This Week's Progress

- Portal frontend reached approximately 90% completion.
- Mock authentication service was successfully enabled.
- One of two critical integration defects was resolved.
- Six of eight required UAT testers were confirmed.
- Security evidence package reached approximately 70% completion.
- Vendor recovery plan was received.

---

## Key Risks and Issues

| Type | Risk / Issue | Impact | Action | Owner |
|---|---|---|---|---|
| Issue | Identity certification 10 days late | UAT schedule risk | Execute vendor recovery plan | Vendor Lead |
| Issue | One critical defect remains open | Testing readiness | Prioritise fix and retest | QA Lead |
| Risk | Two UAT testers not yet confirmed | UAT capacity | Confirm backup resources | Business Owner |

---

## Next Week's Priorities

- Complete identity-provider certification.
- Resolve and retest remaining critical defect.
- Confirm all UAT resources.
- Complete security evidence package.

---

## Decision Required

**Decision:** Approve two temporary vendor developers  
**Owner:** Project Sponsor  
**Deadline:** Friday  
**Impact if delayed:** Recovery capacity may be insufficient to protect the planned UAT start.

---

# Delivery Metrics

Include metrics only when they help explain status.

Possible metrics include:

```text id="weekly-metrics"
Milestone completion
Requirements progress
Build / configuration progress
Defect trend
Test execution
Test pass rate
Release readiness
Budget variance
Vendor milestone performance
```

Do not add metrics purely to make the report look analytical.

---

# Agile / Scrum Considerations

Relevant weekly information may include:

- Sprint Goal progress,
- release progress,
- backlog risks,
- blocked work,
- defects,
- cross-team dependencies.

Avoid simply copying Sprint statistics into an executive report without explaining their project impact.

---

# Kanban Considerations

Where Kanban is used, relevant indicators may include:

```text id="weekly-kanban"
WIP
Blocked work
Work item age
Cycle time
Throughput
SLE performance
```

Example:

> Work item age increased in integration review this week because three items are waiting for external vendor approval, creating a growing release dependency.

Translate flow metrics into management meaning.

---

# Predictive Considerations

Relevant information may include:

- milestone status,
- schedule variance,
- critical-path exposure,
- budget variance,
- approved changes.

---

# Hybrid Considerations

Combine delivery-level evidence with governance-level reporting.

Example:

```text id="weekly-hybrid"
Delivery metrics
↓
Project impact
↓
Risk / issue
↓
Management action
↓
Decision
```

---

# Status Trend

Where useful, include:

```text id="weekly-trend"
Current Week:
Amber

Previous Week:
Green

Trend:
Deteriorating
```

Possible trends:

```text id="weekly-trends"
Improving
Stable
Deteriorating
```

Explain the reason for any material change.

---

# Prompt 2 — Status Report Quality Review

After generating the report:

```text id="weekly-review"
ROLE

You are a PMO Lead performing a quality review of an IT project
weekly status report.

TASK

Review the report below.

[PASTE REPORT]

Check for:

- unsupported RAG status,
- vague statements,
- missing owners,
- missing deadlines,
- hidden decisions,
- risks reported as issues or vice versa,
- excessive operational detail,
- contradictions,
- missing management impact,
- unsupported assumptions.

OUTPUT FORMAT

Finding
Why It Matters
Recommended Correction
Priority
```

---

# Executive Communication Rules

Use:

```text id="weekly-rules"
Professional
Factual
Concise
Evidence-based
Action-oriented
Non-emotional
```

Avoid:

```text id="weekly-avoid"
"We are doing our best."

"The vendor is terrible."

"Everything should probably be fine."

"We had many meetings."

"There are some concerns."
```

Replace opinion with evidence and impact.

---

# Quality Checklist

Before sending the report, confirm:

- [ ] Overall RAG status has a clear rationale
- [ ] Status is supported by project evidence
- [ ] Progress describes outcomes
- [ ] Material risks are visible
- [ ] Material issues are visible
- [ ] Owners are identified
- [ ] Due dates are included where relevant
- [ ] Next-week priorities are clear
- [ ] Decisions are explicit
- [ ] Decision deadlines are visible
- [ ] No unsupported information was invented
- [ ] Language is concise and professional

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- project monitoring,
- communication,
- stakeholder engagement,
- risk and issue management,
- governance,
- decision-making,
- delivery performance.

## PMBOK Relevance

This prompt supports:

- measurement,
- delivery,
- stakeholders,
- governance,
- risk,
- planning.

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

Before distribution, the Project Manager should validate:

- RAG status,
- delivery data,
- risk and issue status,
- financial information,
- decisions required,
- sensitive stakeholder messaging.

AI can turn rough notes into structured communication.

It should not determine official project status without sufficient evidence or accountable review.

---

# Confidentiality

Weekly reports may contain sensitive project information.

Protect:

- customer data,
- security incidents,
- confidential financial data,
- supplier-performance information,
- commercial negotiations,
- personal performance information.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text id="weekly-metadata"
Prompt ID: REPORT-001
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Delivery Lead
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
| 1.0 | YYYY-MM-DD | Initial IT weekly status reporting framework |
