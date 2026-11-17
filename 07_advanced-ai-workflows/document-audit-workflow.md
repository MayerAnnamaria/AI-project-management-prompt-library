# Document Audit Workflow

## Purpose

Use this workflow to audit a project-management document before it is submitted, approved, circulated, or used for decision-making.

The AI acts as a critical quality reviewer and looks for:

- missing information,
- vague wording,
- weak actions,
- unsupported claims,
- inconsistent data,
- unclear ownership,
- missing risks,
- and gaps that a real stakeholder or reviewer may challenge.

The objective is simple:

> Find weaknesses before your reviewer does.

---

## Best Used For

Document audit is especially useful for:

- risk registers,
- project briefs,
- project charters,
- scope documents,
- requirements,
- status reports,
- Steering Committee papers,
- change requests,
- RAID logs,
- vendor evaluations,
- project plans,
- close-out reports.

---

# Core Principle

Use:

```text
Draft
↓
Audit
↓
Find Gaps
↓
Correct
↓
Re-Audit
↓
Submit
```

Do not use:

```text
Draft
↓
Submit
↓
Reviewer Finds Problems
```

---

# Generic Document Audit Prompt

```text
ROLE

You are a senior IT Project Manager and PMO quality reviewer.

TASK

Audit the project document below before it is submitted to
stakeholders.

DOCUMENT TYPE

[PROJECT BRIEF / RISK REGISTER / STATUS REPORT / SCOPE /
CHANGE REQUEST / OTHER]

DOCUMENT

[PASTE DOCUMENT]

AUDIT FOR

1. Missing information
2. Vague or ambiguous wording
3. Unsupported claims
4. Missing owners
5. Missing deadlines
6. Weak actions
7. Missing risks or dependencies
8. Inconsistent dates or data
9. Missing decision requirements
10. Information that may be challenged by a reviewer

OUTPUT FORMAT

Audit Table:

Section / Item
Issue Found
Why It Matters
Specific Recommendation
Priority

Then provide:

Overall Quality Rating:
Poor / Acceptable / Good / Excellent

Justification:
Maximum 3 sentences.

Top 3 Improvements Required Before Submission.
```

---

# Why Audit Before Submission

A document may look complete because it contains many sections.

That does not mean it is decision-ready.

Common weaknesses include:

```text
Information exists
but
is too vague to act on
```

or:

```text
Risk identified
but
no meaningful response exists
```

or:

```text
Decision requested
but
options and consequences are unclear
```

---

# Audit Dimension 1 — Completeness

Ask:

```text
What information should normally be present in this document
but is currently missing?
```

Examples:

For a risk register:

- owner,
- trigger,
- response,
- review date,
- residual risk.

For a status report:

- RAG rationale,
- milestone status,
- risks,
- decisions required,
- forecast.

For a scope document:

- exclusions,
- interfaces,
- acceptance criteria,
- assumptions.

---

# Audit Dimension 2 — Specificity

Look for vague wording.

Examples:

```text
Monitor closely

Manage proactively

Follow up

Resolve quickly

Some delay

Potential issue

Significant risk

As required
```

These phrases often lack actionability.

---

# Example

### Weak

```text
Mitigation:
Monitor vendor closely.
```

### Better

```text
Mitigation:
Vendor Delivery Manager to provide a weekly certification recovery
plan until the dependency is closed.

Escalate to Vendor Director if the forecast date slips by more than
two working days.
```

---

# Audit Dimension 3 — Evidence

Check whether important claims are supported.

Example:

```text
Project remains Green.
```

Ask:

```text
What evidence supports Green?

Schedule?
Budget?
Quality?
Risk?
```

A status colour without rationale is weak governance information.

---

# Evidence Audit Prompt

```text
For every major claim in this document classify it as:

Confirmed Fact
Supported Analysis
Assumption
Opinion
Unsupported Claim

Identify which statements require additional evidence.
```

---

# Audit Dimension 4 — Action Quality

Every material action should ideally include:

```text
Action
Owner
Deadline
Expected Outcome
```

Example:

### Weak

```text
PM to follow up vendor.
```

### Better

```text
PM to obtain the vendor's confirmed certification completion date
and recovery plan by 17:00 CET on 20 November.
```

---

# Audit Dimension 5 — Ownership

Look for:

```text
Someone should...

The team will...

Business to...

Vendor to resolve...
```

Ask:

> Which named role is accountable?

Avoid ambiguous collective ownership where specific accountability is required.

---

# Audit Dimension 6 — Deadlines

Check whether time-sensitive actions have:

```text
Date
Time
Milestone
Trigger
```

Example:

### Weak

```text
Security review to be completed soon.
```

### Better

```text
Security review must be completed by 24 November to protect the
planned production approval.
```

---

# Audit Dimension 7 — Risk Coverage

For risk-related documents ask:

```text
What important risks are not represented?
```

Possible IT risk domains:

```text
Scope
Schedule
Cost
Architecture
Integration
Data
Security
Testing
Vendor
Resources
Operations
Compliance
Change adoption
```

Do not automatically add generic risks.

Flag missing domains for human validation.

---

# Audit Dimension 8 — Mitigation Quality

A mitigation should reduce:

```text
Likelihood
and/or
Impact
```

Weak mitigation:

```text
Track the risk.
```

Tracking is not mitigation.

Better:

```text
Complete an integration proof of concept before development starts
to validate API compatibility.
```

---

# Audit Dimension 9 — Decision Readiness

For decision papers ask:

```text
What decision is required?

Who makes it?

By when?

What options exist?

What happens if no decision is made?

Is there a recommendation?
```

If these are unclear, the paper is not decision-ready.

---

# Audit Dimension 10 — Internal Consistency

Check for:

```text
Different dates for the same milestone

Different owners for the same action

Different risk scores

Different budget figures

Conflicting status statements

Outdated project information
```

---

# Example — Risk Register Audit

## Input

```text
Risk 1:
Project delay
Likelihood: 3
Impact: 3
Mitigation: Monitor schedule.

Risk 2:
Cost overrun
Likelihood: 2
Impact: 4
Mitigation: Review budget monthly.

Risk 3:
Vendor performance
Likelihood: 3
Impact: 4
Mitigation: Manage vendor carefully.
```

---

# Example Audit

| Risk | Issue Found | Specific Recommendation |
|---|---|---|
| R1 | Risk is too generic | Identify cause, event, and specific milestone impact |
| R1 | Mitigation is not actionable | Define preventive schedule action, owner, trigger, and deadline |
| R2 | No cause identified | Identify cost driver rather than generic cost overrun |
| R2 | Monthly review is monitoring, not mitigation | Define cost-control action |
| R3 | Vendor risk is too broad | Identify specific vendor deliverable or dependency |
| R3 | No escalation threshold | Define escalation trigger and owner |

---

# Overall Rating Example

```text
Overall Quality:
Poor

Reason:
The register identifies broad risk themes but does not provide
sufficient specificity to support active risk management.

Most mitigations describe monitoring rather than actions that reduce
likelihood or impact.
```

---

# Prompt 2 — Critical Reviewer Audit

```text
ROLE

You are the most critical but fair reviewer of this document.

You are looking for weaknesses that could cause:

- rejection,
- governance challenge,
- project delay,
- commercial disagreement,
- poor management decisions.

TASK

Review the document below.

[PASTE DOCUMENT]

Identify the five issues most likely to be challenged by an
experienced reviewer.

For each provide:

Weakness
Likely Reviewer Question
Why It Matters
Recommended Fix
```

---

# Prompt 3 — Executive Audit

```text
ROLE

You are an Executive Sponsor reviewing this document.

TASK

Audit it for decision usefulness.

Identify:

- unnecessary detail,
- missing evidence,
- unclear business impact,
- missing decisions,
- unclear accountability,
- unresolved risks.

Then answer:

Would you approve or accept this document as it stands?

Yes / No / With Conditions

Explain why.
```

---

# Prompt 4 — PMO Audit

```text
ROLE

You are a PMO quality reviewer.

TASK

Audit the document against basic project-governance quality.

Check:

- version information,
- ownership,
- dates,
- status,
- traceability,
- decisions,
- risks,
- actions,
- approvals.

OUTPUT

Finding
Governance Impact
Required Correction
Priority
```

---

# Prompt 5 — Technical Reviewer Audit

```text
ROLE

You are a senior Solution Architect reviewing this document.

TASK

Audit only the technical aspects.

Check for:

- technical assumptions,
- undefined interfaces,
- missing architecture decisions,
- missing non-functional requirements,
- security gaps,
- operational gaps,
- unsupported technical claims.

Do not review commercial matters unless they directly affect the
technical solution.
```

---

# Prompt 6 — Commercial Audit

```text
ROLE

You are a senior IT Commercial Manager.

TASK

Audit the document for commercial risk.

Check:

- unclear scope,
- missing exclusions,
- hidden assumptions,
- unapproved changes,
- pricing ambiguity,
- unclear responsibilities,
- vendor dependency,
- acceptance risk.

OUTPUT

Commercial Gap
Potential Exposure
Evidence Required
Recommended Action
```

---

# Prompt 7 — QA / Testing Audit

```text
ROLE

You are a senior QA Lead.

TASK

Audit the document for testability and quality assurance.

Check:

- measurable acceptance criteria,
- test ownership,
- environment assumptions,
- defect criteria,
- evidence,
- entry criteria,
- exit criteria.

Identify anything that cannot be objectively validated.
```

---

# Document-Specific Audit Patterns

## Project Brief

Check:

```text
Business objective
Scope
Deliverables
Constraints
Dependencies
Stakeholders
Risks
Success criteria
```

---

# Project Charter

Check:

```text
Purpose
Business justification
Objectives
Scope
Governance
Authority
Risks
Budget
Milestones
Approval
```

---

# Scope

Check:

```text
Ambiguity
Missing requirements
Interfaces
Exclusions
Acceptance
Dependencies
Assumptions
```

---

# Risk Register

Check:

```text
Cause-event-impact
Scoring
Owner
Mitigation
Trigger
Residual risk
Review date
```

---

# Status Report

Check:

```text
RAG rationale
Progress
Forecast
Risks
Issues
Actions
Decision required
```

---

# Steering Paper

Check:

```text
Decision
Options
Trade-offs
Evidence
Recommendation
Deadline
Consequence
```

---

# Change Request

Check:

```text
Original scope
Changed scope
Cost
Schedule
Resources
Risk
Acceptance
Approval
```

---

# Meeting Minutes

Check:

```text
Decisions
Actions
Owners
Deadlines
Risks
Unresolved items
```

---

# Supplier Evaluation

Check:

```text
Requirement
Evidence
Compliance
Gap
Risk
Clarification
Recommendation
```

---

# Quality Rating

Use:

```text
Poor
Material gaps prevent reliable use.

Acceptable
Usable but requires several improvements.

Good
Generally complete and decision-ready with minor gaps.

Excellent
Clear, evidence-based, actionable, and internally consistent.
```

The rating should always include reasoning.

---

# Do Not Optimise for the Rating

The goal is not:

```text
Get AI to say "Excellent."
```

The goal is:

```text
Find material weaknesses before real-world submission.
```

---

# Audit → Correction Workflow

Use:

```text
Document
↓
Audit
↓
Issues Identified
↓
Human Confirms
↓
Corrections
↓
Re-Audit
↓
Submit
```

---

# Re-Audit Prompt

```text
The document has now been revised.

Compare the new version with your previous audit.

Confirm:

1. Which findings are resolved
2. Which findings are partially resolved
3. Which findings remain open
4. Whether any new issue was introduced

Then provide an updated quality rating.
```

---

# Difference Audit

For major revisions:

```text
Compare Version 1 and Version 2.

Identify:

Added information
Removed information
Changed facts
Changed dates
Changed owners
Changed risk ratings
Changed decisions

Flag any unintended material change.
```

---

# Audit Priority

Use:

```text
Critical
Could lead to incorrect decision, major risk, or rejection.

High
Material weakness requiring correction before issue.

Medium
Should be improved but may not block issue.

Low
Formatting or minor clarity improvement.
```

---

# AI Audit Limitations

AI may identify plausible gaps that are not relevant to the actual project.

Therefore:

```text
AI Finding
↓
Human Validation
↓
Correction if Relevant
```

Do not automatically add every suggestion.

---

# Missing Information Rule

If information is absent, AI should say:

```text
Not provided.
```

Not invent it.

---

# False Precision Rule

Do not improve a document by fabricating:

- dates,
- percentages,
- budgets,
- owners,
- risk scores,
- milestones,
- contractual clauses.

A more detailed document is not automatically a more accurate document.

---

# Audit as a Quality Gate

For important artefacts:

```text
Author
↓
Document Audit
↓
Specialist Review
↓
Stakeholder Approval
```

AI audit can improve quality before expensive human review time is used.

---

# Agile / Scrum Considerations

Audit:

- release summaries,
- Product Owner decision papers,
- dependency reports,
- Sprint / release communications.

Avoid creating unnecessary documentation solely to satisfy an audit.

---

# Kanban Considerations

Audit:

- service-review commentary,
- flow reports,
- blocked-item analysis,
- operational risk summaries.

Check whether metrics lead to actions rather than simply describing flow.

---

# Predictive Considerations

Audit formal:

- baselines,
- milestone reports,
- change documents,
- risk registers,
- governance papers.

---

# Hybrid Considerations

Audit both:

```text
Delivery Evidence
+
Formal Governance
```

Check that they tell a consistent story.

---

# Quality Checklist

Before completing a document audit, confirm:

- [ ] Completeness reviewed
- [ ] Vague wording identified
- [ ] Unsupported claims identified
- [ ] Action quality reviewed
- [ ] Ownership reviewed
- [ ] Deadlines reviewed
- [ ] Risk coverage reviewed where relevant
- [ ] Decision clarity reviewed
- [ ] Internal consistency checked
- [ ] Recommendations are specific
- [ ] Overall rating is justified
- [ ] AI findings will receive human validation

---

# Key Principle

Document audit is not:

```text
Proofread this.
```

It is:

```text
Act as a critical professional reviewer.

Find the management, governance, evidence, and decision gaps
before the document reaches the real reviewer.
```

---

# Prompt Metadata

```text
Prompt ID: AIWF-004
Category: Advanced AI Workflows
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Project Manager
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low / Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial document-audit workflow |
