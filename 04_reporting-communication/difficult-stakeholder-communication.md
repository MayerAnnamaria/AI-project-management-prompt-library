# Difficult Stakeholder Communication

## Purpose

Use this prompt to draft professional communication for difficult project situations where the message must be:

- factual,
- clear,
- firm,
- constructive,
- and relationship-aware.

Typical situations include:

- schedule delay,
- missed vendor commitments,
- unresolved dependencies,
- quality concerns,
- budget pressure,
- scope conflict,
- resource shortages,
- late decisions,
- security or compliance concerns.

The objective is to communicate the problem without becoming:

- defensive,
- emotional,
- accusatory,
- vague,
- or unnecessarily confrontational.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment / Hypercare

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / Programme Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
As required

---

# Prompt

```text id="stakeholder-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, stakeholder management, vendor governance,
executive communication, and difficult project conversations.

TASK

Draft a professional communication for the stakeholder situation below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Stakeholder:
[ROLE / ORGANISATION]

Relationship:
[COLLABORATIVE / FORMAL / TENSE / ESCALATED]

Situation:
[DESCRIBE WHAT HAS HAPPENED]

Known facts:
[FACTS]

Current impact:
[SCHEDULE / COST / SCOPE / QUALITY / RISK / BUSINESS]

Actions already taken:
[LIST]

Recovery measures:
[LIST]

Action required from stakeholder:
[LIST]

Required deadline:
[DATE]

Governance / contractual considerations:
[IF RELEVANT]

OUTPUT FORMAT

Structure the communication as:

1. Reference / Subject
2. Purpose
3. Factual Situation
4. Project Impact
5. Current Management / Recovery Action
6. Action Required from Recipient
7. Deadline / Consequence of Delay
8. Professional Close

TONE

Professional
Factual
Confident
Constructive
Non-defensive
Non-emotional
```

---

# Communication Principle

Use:

```text id="stakeholder-flow"
Facts
↓
Impact
↓
Action
↓
Decision / Response Required
↓
Deadline
```

Avoid:

```text id="stakeholder-avoid-flow"
Emotion
↓
Blame
↓
Long explanation
↓
Unclear request
```

---

# 1. Subject / Reference

The subject should make the purpose immediately clear.

### Weak

```text id="stakeholder-subject-weak"
Project Update
```

### Better

```text id="stakeholder-subject-better"
Customer Portal — Identity Integration Delay and Required Recovery Action
```

Or:

```text id="stakeholder-subject-example"
CRM Migration — Schedule Impact and Decision Required by 15 August
```

---

# 2. Opening

State the purpose directly.

Example:

```text id="stakeholder-opening"
I am writing to formally notify you of a delay affecting the
identity-integration workstream and to confirm the recovery actions
required to protect the planned UAT start.
```

Avoid overly apologetic openings unless an apology is genuinely appropriate.

---

# 3. Factual Description

Describe:

```text id="stakeholder-facts"
What happened
When
What was expected
What actually occurred
Current status
```

Use evidence.

Example:

> The API certification milestone was due on 5 June. As of 15 June, certification remains incomplete, resulting in a ten-working-day variance against the agreed plan.

Avoid:

> Your team keeps delaying everything.

---

# 4. Impact

Explain the project consequence.

Possible areas:

```text id="stakeholder-impact"
Schedule
Scope
Cost
Testing
Quality
Security
Operations
Business readiness
Customer impact
```

Example:

> The current delay prevents production-equivalent authentication testing and creates a direct dependency risk to the planned UAT start.

---

# Impact Without Exaggeration

Do not claim:

> The entire project will fail.

when the evidence only supports:

> The current delay may affect the UAT start unless recovery action is completed by 20 June.

Use proportionate language.

---

# 5. Recovery Measures

Explain what the project team is already doing.

Examples:

```text id="stakeholder-recovery"
Use temporary mock service
Re-sequence unaffected activities
Add technical review capacity
Accelerate defect resolution
Prepare parallel validation
Increase review cadence
```

This demonstrates management control rather than passive escalation.

---

# 6. Action Required

Be explicit.

### Weak

```text id="stakeholder-action-weak"
Please provide an update.
```

### Better

```text id="stakeholder-action-better"
Please provide by 17:00 CET on Thursday:

1. confirmed certification date,
2. recovery plan,
3. named action owners,
4. any additional support required from our team.
```

---

# 7. Deadline and Consequence of Delay

Use:

```text id="stakeholder-deadline"
Required by:
[DATE / TIME]

Reason:
[WHY THIS DATE MATTERS]

Impact if Delayed:
[PROJECT IMPACT]
```

Example:

> A confirmed recovery plan is required by Thursday because any further delay beyond Friday will reduce the available contingency before UAT.

---

# Tone Rules

The tone should be:

```text id="stakeholder-tone"
Firm without being aggressive
Confident without being dismissive
Factual without being cold
Constructive without hiding impact
```

---

# Avoid Emotional Language

Avoid:

```text id="stakeholder-emotional"
unacceptable
disappointing
frustrating
careless
your failure
your mistake
you always
you never
```

unless the organisational context genuinely requires stronger formal language.

Prefer:

```text id="stakeholder-factual-alternative"
The agreed milestone has not been met.

The current position creates a material schedule risk.

The recovery plan remains outstanding.

Management intervention is now required.
```

---

# Example Input

```text id="stakeholder-example-input"
Project:
Customer Portal

Stakeholder:
External identity provider

Relationship:
Professional but increasingly tense

Situation:
API certification is 10 working days late.

Expected Date:
5 June

Current Date:
15 June

Impact:
Production-equivalent authentication testing cannot complete.
UAT start may slip.

Actions Taken:
Mock service implemented.
Internal team re-sequenced testing.

Required from Vendor:
Confirmed certification date.
Recovery plan.
Named owners.

Deadline:
Thursday 17:00 CET.
```

---

# Example Output

## Subject

**Customer Portal — Identity Certification Delay and Recovery Action Required**

Dear [Name],

I am writing to formally confirm the current impact of the delayed identity-certification milestone and the recovery actions required to protect the planned UAT start.

The certification milestone was due on 5 June and remains incomplete as of 15 June, representing a ten-working-day variance against the agreed plan. As a result, production-equivalent authentication testing cannot yet be completed, creating a direct dependency risk to the UAT schedule.

To reduce the current impact, the project team has implemented the approved mock authentication service and re-sequenced eligible integration testing. These measures are protecting part of the test schedule but do not remove the need for completed certification.

Please provide by **17:00 CET on Thursday**:

1. confirmed certification completion date,
2. detailed recovery plan,
3. named owners for all outstanding actions,
4. any support required from our project team.

A further delay beyond the current recovery window may affect the planned UAT start and will require escalation through project governance.

Thank you for your prompt attention to this matter.

Kind regards,  
[Project Manager]

---

# Prompt 2 — Recipient Perspective Review

Before sending an important message:

```text id="stakeholder-review"
ROLE

You are the recipient of the project communication below.

TASK

Review the message from the recipient's perspective.

[PASTE MESSAGE]

Identify:

- questions I would ask,
- statements that lack evidence,
- unclear requests,
- unnecessary defensiveness,
- language that may damage the relationship,
- missing deadlines,
- missing project impact,
- possible misunderstandings.

OUTPUT FORMAT

Finding
Recipient Reaction
Why It Matters
Recommended Improvement
```

This second-pass review is especially useful for sensitive communications.

---

# Prompt 3 — Executive Escalation Version

```text id="stakeholder-exec"
ROLE

You are a senior Project Manager preparing an executive escalation.

TASK

Convert the communication below into a concise executive escalation.

[PASTE MESSAGE]

OUTPUT FORMAT

Issue
Current Impact
Actions Taken
Decision / Support Required
Owner
Deadline
Impact if Delayed

Maximum length:
150 words
```

---

# Prompt 4 — Vendor Escalation

```text id="stakeholder-vendor"
ROLE

You are a senior IT Project Manager escalating repeated vendor
delivery failure.

TASK

Draft a professional vendor escalation using the evidence below.

CONTEXT

Vendor:
[VENDOR]

Commitment:
[COMMITMENT]

Original due date:
[DATE]

Current status:
[STATUS]

Previous recovery commitments:
[DETAILS]

Impact:
[DETAILS]

Required recovery:
[DETAILS]

OUTPUT FORMAT

1. Current Position
2. Missed Commitment
3. Project Impact
4. Previous Recovery Actions
5. Required Recovery Plan
6. Escalation Requirement
7. Deadline
```

---

# Prompt 5 — Late Stakeholder Decision

```text id="stakeholder-late-decision"
ROLE

You are a senior Project Manager following up on an overdue
governance decision.

TASK

Draft a concise, professional escalation.

CONTEXT

Decision required:
[DECISION]

Decision owner:
[OWNER]

Original deadline:
[DATE]

Current impact:
[IMPACT]

Next dependency:
[DEPENDENCY]

OUTPUT FORMAT

State:

- decision required,
- why it is overdue,
- current impact,
- new final deadline,
- consequence if not received.
```

---

# Difficult Internal Stakeholder

The same principles apply internally.

Examples:

- business team does not provide UAT resources,
- architecture decision remains unresolved,
- security approval is delayed,
- sponsor decision is overdue,
- competing departments disagree on scope.

Use facts and governance rather than personal criticism.

---

# Example

Instead of:

> The business team is not cooperating.

Use:

> Six of the eight required UAT testers remain unconfirmed. Unless named resources are confirmed by 20 August, the current UAT plan will no longer be achievable.

---

# Communication Under Pressure

Before sending, check:

```text id="stakeholder-pressure"
Am I stating facts?

Am I separating facts from assumptions?

Have I explained impact?

Have I explained what we are doing?

Is the required action explicit?

Is the deadline explicit?

Is escalation proportionate?

Would I be comfortable seeing this message forwarded to senior management?
```

---

# Agile / Scrum Considerations

Do not escalate routine delivery disagreements unnecessarily.

Many issues should first be handled through:

- Product Owner discussion,
- team collaboration,
- backlog clarification,
- dependency resolution.

Escalate when:

- authority is insufficient,
- external commitments are threatened,
- decisions exceed team authority,
- material risk exists.

---

# Kanban Considerations

Evidence may include:

- ageing blocked work,
- repeated SLE breaches,
- growing WIP,
- persistent external dependencies.

Example:

> Three integration items have remained blocked for more than eight working days awaiting external approval, and the resulting work-item ageing now threatens the release forecast.

---

# Predictive Considerations

Communication may reference:

- milestone variance,
- baseline commitments,
- critical-path impact,
- formal change control,
- recovery plans.

---

# Hybrid Considerations

Combine formal governance with evidence from the actual delivery system.

Example:

```text id="stakeholder-hybrid"
Delivery evidence
↓
Project impact
↓
Required action
↓
Governance escalation
```

---

# Contractual / Legal Communications

If the communication has contractual or legal significance:

- verify contractual references,
- involve Legal or Procurement where appropriate,
- preserve required notice periods,
- avoid invented clause references,
- distinguish project-management communication from formal legal notice.

AI-generated wording should not be treated as legal advice.

---

# Quality Checklist

Before sending, confirm:

- [ ] Subject clearly states the purpose
- [ ] Facts are accurate
- [ ] Dates are accurate
- [ ] Impact is proportionate
- [ ] Tone is professional
- [ ] No unnecessary blame is included
- [ ] Recovery actions are visible
- [ ] Required action is explicit
- [ ] Owner is clear
- [ ] Deadline is clear
- [ ] Consequence of delay is clear
- [ ] Escalation is proportionate
- [ ] Contractual statements have been verified where relevant

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder engagement,
- communication,
- conflict management,
- governance,
- leadership,
- issue management,
- escalation.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- governance,
- delivery,
- risk,
- communication,
- leadership.

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

Sensitive stakeholder communication should be reviewed where appropriate by:

- Project Manager
- Programme Manager
- Sponsor
- Procurement
- Legal
- Vendor Management
- Security

The more contractual, financial, political, or reputational the communication becomes, the more important human review is.

---

# Confidentiality

Sensitive communications may contain:

- commercial positions,
- contractual information,
- vendor performance concerns,
- employee information,
- security issues,
- internal governance discussions.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text id="stakeholder-metadata"
Prompt ID: REPORT-005
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor / Legal where applicable
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
| 1.0 | YYYY-MM-DD | Initial difficult stakeholder communication framework |
