# Role Stacking — Author Then Reviewer

## Purpose

Use role stacking to improve important project-management outputs before they are sent to stakeholders.

The workflow uses the AI twice in the same conversation:

```text
Role 1
Author
↓
Draft
↓
Role 2
Reviewer / Recipient
↓
Challenge
↓
Improved Version
```

The first role creates the document.

The second role reviews it from the perspective of the person who will receive, approve, challenge, or act on it.

The objective is to expose weaknesses **before the real stakeholder does**.

---

## Best Used For

Role stacking is especially useful for:

- status reports,
- Steering Committee papers,
- executive updates,
- risk escalations,
- change requests,
- vendor communications,
- contractual correspondence,
- project proposals,
- decision papers,
- go-live recommendations.

---

# Core Principle

Do not ask:

```text
Is this document good?
```

Instead ask:

```text
Who will read this?

What will they care about?

What will they challenge?

What evidence will they expect?

What decision are they being asked to make?
```

Then instruct the AI to review from that perspective.

---

# Two-Role Workflow

```text
Author Role
↓
Create Draft
↓
Recipient Role
↓
Challenge Draft
↓
Identify Weaknesses
↓
Rewrite
```

---

# Step 1 — Draft as the Project Manager

```text
ROLE

You are a senior IT Project Manager.

TASK

Draft a concise weekly project status summary for the project below.

PROJECT CONTEXT

Project:
Enterprise CRM Replacement

Overall Status:
Amber

Current Situation:
UAT is forecast to start five working days late because external
identity-provider certification remains incomplete.

Actions Taken:
Mock authentication service implemented.
Unaffected testing has been resequenced.
Vendor escalation is active.

Business Impact:
Current production release date remains achievable but contingency
has reduced.

OUTPUT

Write:

1. Overall Status
2. Current Position
3. Main Risk
4. Recovery Actions
5. Decision / Support Required

Keep the summary suitable for senior stakeholders.
```

---

# Step 2 — Switch to the Recipient Role

After the first response:

```text
Now switch roles.

You are the Executive Sponsor receiving this status update.

You are experienced, time-constrained, and focused on:

- delivery confidence,
- business impact,
- decision requirements,
- evidence,
- accountability,
- whether the release commitment remains credible.

Review the status summary you just produced.

Identify:

1. The three weakest points
2. Any vague or unsupported statements
3. Questions you would immediately ask the Project Manager
4. Information missing for decision-making
5. A rewritten version addressing the weaknesses
```

---

# Why Role Stacking Works

A document can appear strong from the author's perspective while still leaving unanswered questions for the recipient.

Example:

```text
Project Manager thinks:
"The recovery plan is clear."

Sponsor thinks:
"How confident are we that the release date is still achievable?"
```

Role stacking forces the draft to survive a different perspective.

---

# Reviewer Perspectives

Choose a reviewer role that matches the actual audience.

---

# Executive Sponsor

Focus on:

```text
Business value
Schedule
Budget
Major risks
Decisions
Accountability
Confidence
```

Prompt:

```text
You are now the Executive Sponsor.

Review this document and identify anything that prevents you from
understanding project health or making the required decision.
```

---

# Steering Committee

Focus on:

```text
Governance
Options
Trade-offs
Recommendation
Decision required
Consequences
```

Prompt:

```text
You are now a Steering Committee member.

You have ten minutes to review this paper before the meeting.

Identify:

- what is unclear,
- what evidence is missing,
- whether options are balanced,
- whether the recommendation is justified,
- whether the decision required is explicit.
```

---

# CFO / Finance Reviewer

Focus on:

```text
Cost
Forecast
Commercial exposure
Assumptions
Contingency
Financial impact
```

Prompt:

```text
You are now the CFO reviewing this project update.

Challenge every financial statement.

Identify:

- unsupported cost claims,
- missing forecast information,
- unclear contingency,
- unexplained variance,
- financial risks requiring escalation.
```

---

# CIO / CTO

Focus on:

```text
Architecture
Technical risk
Security
Scalability
Technical debt
Operational readiness
```

Prompt:

```text
You are now the CTO reviewing this proposal.

Identify:

- technical assumptions,
- architecture risk,
- missing dependencies,
- operational concerns,
- technical evidence required before approval.
```

---

# CISO / Security Reviewer

Focus on:

```text
Security risk
Access
Data protection
Vulnerabilities
Controls
Approval evidence
```

Prompt:

```text
You are now the Information Security reviewer.

Challenge the document from a security and production-readiness
perspective.

Identify anything that would prevent you from approving the release.
```

---

# Product Owner

Focus on:

```text
Business value
Scope
Priorities
Acceptance
User outcomes
```

Prompt:

```text
You are now the Product Owner.

Review this output and identify whether:

- business value is clear,
- scope assumptions are correct,
- acceptance criteria are sufficient,
- priorities are aligned,
- any important user outcome is missing.
```

---

# Operations / Service Manager

Focus on:

```text
Supportability
Monitoring
Incidents
Runbooks
Ownership
Handover
```

Prompt:

```text
You are now the Service Manager who will operate this solution
after go-live.

Review the readiness assessment.

Identify every operational question you would ask before accepting
handover.
```

---

# Vendor Reviewer

When communicating with a supplier:

```text
You are now the Supplier Delivery Manager receiving this escalation.

Review it and identify:

- allegations you would challenge,
- evidence you would request,
- unclear responsibilities,
- statements that may be interpreted differently,
- opportunities to dispute the project position.
```

This can help strengthen commercial correspondence.

---

# Procurement / Commercial Reviewer

Focus on:

```text
Scope
Contract
Pricing
Assumptions
Obligations
Change control
```

Prompt:

```text
You are now the Commercial Manager.

Review this change request and identify:

- unclear scope,
- unsupported commercial assumptions,
- missing pricing evidence,
- contractual ambiguity,
- missing approvals.
```

---

# PMO Reviewer

Focus on:

```text
Governance
Consistency
Evidence
Ownership
Dates
Risk
Decision traceability
```

Prompt:

```text
You are now a PMO quality reviewer.

Check this document for:

- inconsistent dates,
- unclear owners,
- missing decisions,
- unsupported RAG status,
- missing risks,
- governance gaps.
```

---

# Business User Perspective

For user-facing communication:

```text
You are an employee who will receive this system-change
announcement.

You have no technical project knowledge.

Review it and answer:

1. Do I understand what is changing?
2. Do I understand when?
3. Do I understand how it affects me?
4. Do I know what I need to do?
5. Do I know where to get help?
```

---

# Multi-Role Stacking

For high-impact documents, use more than one reviewer.

Example:

```text
Project Manager
↓
Draft
↓
PMO Review
↓
Technical Review
↓
Executive Review
↓
Final Document
```

---

# Example — Go-Live Decision

Start with:

```text
ROLE

You are a senior IT Project Manager.

Create a Go / No-Go recommendation for the CRM production release.

CONTEXT

UAT:
Complete

Critical defects:
0

High defects:
2 with approved workarounds

Security:
Approved

Data migration rehearsal:
Passed

Operations:
Runbook approved

Vendor support:
Confirmed

Business readiness:
95% training completion

OUTPUT

Recommendation
Evidence
Open Risks
Conditions
Decision Required
```

Then role stack.

---

# Reviewer 1 — CISO

```text
Now act as the CISO.

Review the recommendation.

What evidence would you challenge before production approval?
```

---

# Reviewer 2 — Operations

```text
Now act as the Service Manager.

Identify anything that would prevent operational acceptance.
```

---

# Reviewer 3 — Sponsor

```text
Now act as the Executive Sponsor.

Is there enough information here to make the Go / No-Go decision?

Identify the three most important unanswered questions.

Then rewrite the final recommendation.
```

---

# Result

The document has now been challenged from:

```text
Security
+
Operations
+
Business Governance
```

This is stronger than asking the AI to simply “improve” the text.

---

# Adversarial Review

For important documents, explicitly ask the reviewer to challenge assumptions.

```text
Do not try to agree with the author.

Act as a rigorous reviewer.

Identify:

- weak evidence,
- unsupported assumptions,
- contradictions,
- vague claims,
- missing alternatives,
- risks being understated.
```

This helps reduce overly agreeable AI output.

---

# Evidence Challenge

Use:

```text
For every major claim in this document classify it as:

Confirmed Fact
Supported Analysis
Assumption
Opinion
Unsupported Claim
```

Then ask:

```text
Which claims require additional evidence before the document should
be issued?
```

---

# Question Prediction

A particularly useful role-stacking prompt is:

```text
You are the recipient of this document.

What are the five questions you are most likely to ask immediately
after reading it?
```

If the questions are predictable, the document can often answer them before being sent.

---

# Example

Draft states:

> The project remains on track for go-live.

Reviewer asks:

```text
What evidence supports this?

How much contingency remains?

What are the unresolved dependencies?

What would cause the date to move?

What is your confidence level?
```

The revised report should address these points.

---

# Decision-Maker Review

For decision papers:

```text
You are the person being asked to approve this recommendation.

Review the paper.

Tell me:

1. What decision am I being asked to make?
2. Do I have enough evidence?
3. Are alternatives clearly presented?
4. Are trade-offs visible?
5. What information would prevent me from approving this today?
```

---

# Role Stacking for Risk

```text
ROLE 1

You are the Project Manager.

Create a response plan for Risk R-004.
```

Then:

```text
ROLE 2

You are the Risk Owner.

Challenge whether the proposed actions are realistic and within
your control.
```

Then:

```text
ROLE 3

You are the PMO Risk Lead.

Review whether the residual risk rating is justified.
```

---

# Role Stacking for Vendor Evaluation

```text
ROLE 1
Procurement evaluator

↓
Supplier assessment

ROLE 2
Supplier

↓
Challenge the assessment

ROLE 3
Commercial reviewer

↓
Identify where evidence remains insufficient
```

This can help reduce one-sided vendor evaluations.

---

# Role Stacking for Requirements

```text
Business Analyst
↓
Draft requirement

Developer
↓
Identify technical ambiguity

Tester
↓
Identify testability gaps

Product Owner
↓
Confirm business intent
```

---

# Example Prompt

```text
ROLE 1

You are a senior Business Analyst.

Write acceptance criteria for the requirement below.

[REQUIREMENT]

After answering, wait.
```

Then:

```text
Now act as a QA Lead.

Review the acceptance criteria.

Identify anything that cannot be objectively tested.
```

Then:

```text
Now act as the Product Owner.

Check whether the revised criteria still represent the intended
business outcome.
```

---

# Role Stacking for Status Reports

Recommended reviewers:

```text
Project Manager
→ Creates

PMO
→ Checks governance

Sponsor
→ Checks decision usefulness
```

---

# Role Stacking for Technical Proposals

Recommended reviewers:

```text
Solution Architect
→ Creates

Security
→ Challenges risk

Operations
→ Challenges supportability

Project Manager
→ Reviews delivery impact
```

---

# Role Stacking for Commercial Changes

Recommended reviewers:

```text
Supplier
→ Provides proposal

Project Manager
→ Reviews scope / delivery

Commercial Manager
→ Reviews cost / contract

Business Owner
→ Reviews value
```

---

# Role Conflict

Different reviewers may disagree.

Example:

```text
Security:
Delay release until vulnerability is resolved.

Business:
Release is commercially urgent.

Operations:
Release is supportable with a workaround.
```

Do not ask AI to hide the conflict.

Instead:

```text
Summarise the competing stakeholder positions.

For each provide:

Objective
Concern
Risk
Preferred Outcome

Then identify realistic decision options and trade-offs.
```

---

# Role Stacking Is Not Consensus Generation

The objective is not:

```text
Make every reviewer agree.
```

It is:

```text
Expose different perspectives before the decision is made.
```

---

# Reviewer Selection

Choose reviewers based on the document.

| Document | Useful Reviewer |
|---|---|
| Status Report | Sponsor / PMO |
| Change Request | Commercial / Business Owner |
| Architecture Proposal | Architect / Security / Operations |
| Go-Live Paper | Business / Security / Operations |
| Vendor Escalation | Supplier / Procurement |
| Risk Response | Risk Owner / PMO |
| User Communication | End User / Change Lead |
| Contract Notice | Commercial / Legal |

---

# Don't Invent Authority

A simulated reviewer can identify likely concerns.

It cannot provide actual approval.

Example:

```text
AI acting as CISO
≠
Security approval
```

Similarly:

```text
AI acting as Legal Counsel
≠
Legal advice
```

Role stacking supports preparation.

It does not replace authorised review.

---

# Same-Conversation Workflow

Keep related author/reviewer steps in the same conversation where context matters.

```text
Draft
↓
Reviewer
↓
Revision
```

However, explicitly tell the model when the role changes.

Example:

```text
Stop acting as the Project Manager.

Now act as the Executive Sponsor.
```

This makes the review perspective clearer.

---

# Final Reconciliation

After multiple reviewers:

```text
Return to the Project Manager role.

Review all reviewer comments above.

Create a final version that:

- addresses material weaknesses,
- preserves verified facts,
- does not introduce unsupported claims,
- makes remaining disagreements explicit.
```

---

# Quality Gate

Before finalising an important document:

```text
Author Review
↓
Recipient Review
↓
Evidence Review
↓
Final Revision
```

This creates a simple AI-assisted quality gate.

---

# Role Stacking Quality Checklist

Before using the workflow, confirm:

- [ ] The author role is clearly defined
- [ ] The real audience is understood
- [ ] Reviewer role matches the audience
- [ ] Reviewer is instructed to challenge, not agree
- [ ] Weak evidence is identified
- [ ] Likely questions are predicted
- [ ] Missing information is highlighted
- [ ] Revision preserves verified facts
- [ ] Reviewer comments are not treated as actual stakeholder approval
- [ ] Human review still occurs for material decisions

---

# Key Principle

Role stacking is not:

```text
Ask AI to rewrite the same text twice.
```

It is:

```text
Draft from one professional perspective
↓
Challenge from another
↓
Strengthen the output before real-world review
```

This turns AI into both:

```text
Author
+
Critical Reviewer
```

while keeping the Project Manager accountable for the final output.

---

# Prompt Metadata

```text
Prompt ID: AIWF-002
Category: Advanced AI Workflows
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Project Manager
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
| 1.0 | YYYY-MM-DD | Initial role-stacking review workflow |
