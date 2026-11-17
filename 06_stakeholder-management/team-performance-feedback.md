# Team Performance Feedback

## Purpose

Use this prompt to prepare clear, fair, and constructive performance feedback for a project-team member.

The objective is to:

- recognise strengths,
- address a specific performance concern,
- explain its project impact,
- establish clear expectations,
- offer appropriate support,
- and create an opportunity for improvement.

The purpose is not to create unnecessarily harsh criticism.

The purpose is to help the team member understand **what is working, what needs to change, why it matters, and what good performance looks like going forward**.

---

## Best Used For

**Project phase:**  
Any delivery phase

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / Team Lead / Programme Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
When specific performance feedback is required

---

# Prompt

```text
ROLE

You are a senior IT Project Manager experienced in leading
international and cross-functional technology teams.

TASK

Prepare structured written performance feedback for the team member
described below.

TEAM MEMBER

Role:
[ROLE]

Experience level:
[LEVEL]

Project responsibilities:
[RESPONSIBILITIES]

STRENGTHS

[LIST SPECIFIC STRENGTHS]

PERFORMANCE CONCERN

[DESCRIBE THE SPECIFIC ISSUE]

SPECIFIC EXAMPLES

[DATES / EVENTS / OBSERVABLE BEHAVIOUR]

PROJECT IMPACT

[EXPLAIN IMPACT]

CONTEXT

[RELEVANT CONTEXT — TEAM STRUCTURE / REMOTE WORK / COMMUNICATION /
WORKLOAD / CULTURAL OR LANGUAGE CONSIDERATIONS]

EXPECTED BEHAVIOUR GOING FORWARD

[DEFINE EXPECTATION]

SUPPORT AVAILABLE

[DETAILS]

CONSEQUENCE IF PATTERN CONTINUES

[DETAILS IF APPROPRIATE]

OUTPUT REQUIREMENTS

Create structured feedback that:

1. acknowledges strengths specifically,
2. describes the issue using observable facts,
3. explains why the behaviour matters,
4. considers relevant context without making assumptions,
5. sets a clear future expectation,
6. offers practical support,
7. explains next steps if the issue continues.

Tone:
Firm
Fair
Supportive
Respectful
Specific
Professional
```

---

# Core Feedback Principle

Use:

```text
Strength
↓
Observed Behaviour
↓
Project Impact
↓
Expected Behaviour
↓
Support
↓
Follow-Up
```

Avoid:

```text
Personal Judgment
↓
Vague Criticism
↓
No Example
↓
No Clear Expectation
```

---

# 1. Start With Genuine Strengths

Acknowledge specific strengths relevant to the person's work.

### Weak

```text
You are doing a good job overall.
```

### Better

```text
Your defect analysis has been consistently detailed, and you have
identified several integration issues before they reached UAT.

Your technical preparation and attention to evidence are valuable
to the project.
```

Specific recognition makes the feedback more credible.

---

# 2. Describe Behaviour, Not Personality

Focus on observable behaviour.

Avoid:

```text
You are not proactive.
```

Prefer:

```text
During the last two dependency reviews, the API delivery risk was
already known within your workstream but was not raised during the
project meeting.

The risk was escalated only after it had begun affecting the test
schedule.
```

---

# Behaviour vs Interpretation

Separate:

```text
Observation:
The risk was not raised in the meeting.
```

from:

```text
Interpretation:
The person does not care about communication.
```

Do not present interpretation as fact.

---

# 3. Use Specific Examples

Strong feedback includes:

```text
When

Where

What happened

What should have happened

What impact occurred
```

Example:

> At the integration review on 10 September, the vendor dependency had already been identified by the technical team but was not raised during the meeting. The dependency became a schedule issue three days later and required escalation.

This is more actionable than:

> You need to communicate earlier.

---

# Specificity Principle

Use:

```text
Event
+
Behaviour
+
Impact
```

Example:

```text
During Tuesday's UAT readiness review,
the two unresolved Severity 1 defects were not highlighted
when readiness was discussed.

As a result, stakeholders initially left the meeting believing
that UAT could start as planned.
```

---

# 4. Explain Why It Matters

Connect behaviour to project outcomes.

Possible impacts:

```text
Schedule

Quality

Risk

Decision-making

Stakeholder trust

Team coordination

Customer impact

Vendor management

Delivery predictability
```

Example:

> Early visibility of delivery risks is essential because it gives the project team time to mitigate the issue before it affects committed milestones.

---

# 5. Consider Context

Relevant context may include:

```text
Remote working

New team membership

Different communication styles

Language

Experience level

Workload

Unclear role expectations

Organisational culture
```

However, context should not become unsupported speculation.

---

# Cultural Awareness

Use cultural awareness carefully.

Avoid:

```text
People from your culture tend not to challenge others in meetings.
```

Prefer:

```text
I recognise that communication styles can differ across teams and
working environments.

Regardless of communication style, the project requires material
delivery risks to be raised early so the wider team can act on them.
```

Respect the individual without stereotyping.

---

# 6. Define the Expected Behaviour

Be precise.

### Weak

```text
Please communicate better.
```

### Better

```text
Going forward, I expect any issue that could materially affect a
milestone, dependency, cost, scope, or quality target to be raised
during the relevant project meeting as soon as it is identified.

If you are uncertain whether something is significant enough to
escalate, raise it with me directly before the meeting.
```

---

# Expectation Framework

Define:

```text
What

When

Where

How

Threshold
```

Example:

```text
What:
Material schedule risks

When:
As soon as identified

Where:
Weekly delivery review / Jira / direct escalation

How:
Risk statement + impact + proposed action

Threshold:
Potential impact to milestone or committed dependency
```

---

# 7. Offer Support

Feedback should include a realistic path to improvement.

Possible support:

```text
1:1 preparation

Meeting coaching

Communication templates

Clarification of escalation thresholds

Mentoring

Training

Pairing with experienced team member

Regular check-ins
```

Example:

> For the next month, we can spend ten minutes before the weekly delivery meeting reviewing any risks you think may need escalation.

---

# 8. Explain Consequences Carefully

Where appropriate, clarify what happens if the issue continues.

Avoid threatening language.

### Weak

```text
If this happens again there will be consequences.
```

### Better

```text
I expect to see consistent improvement in early risk communication.

If material risks continue to remain unreported, we will need to
review whether the current responsibility model is appropriate and
agree a more formal improvement plan.
```

---

# Consequence Principle

Use:

```text
Expectation
↓
Opportunity to Improve
↓
Follow-Up
↓
Escalation if Necessary
```

Do not jump directly from feedback to punishment unless the situation requires formal HR action.

---

# Example Input

```text
Role:
Business Analyst

Strengths:
Strong requirements analysis.
Very good documentation.
Good relationship with business users.

Concern:
Important requirement changes are sometimes discussed directly with
business stakeholders but not communicated quickly enough to the
development team.

Example:
Two changes agreed last month were entered into the backlog several
days later after development had already started.

Impact:
Rework and confusion about approved requirements.

Expected Behaviour:
Any agreed requirement change must be documented and communicated
through the project process on the same working day.

Support:
PM will review change process together with BA.

Context:
BA joined project three months ago.
```

---

# Example Output

## Performance Feedback

You have made a strong contribution to the project through your requirements analysis and documentation. Your ability to work with business users and translate their needs into structured requirements has been particularly valuable.

I would like to address one area that needs improvement: the speed at which agreed requirement changes are communicated to the delivery team.

On two recent occasions, requirement changes were discussed and agreed with business stakeholders but were not reflected in the delivery backlog until several days later. In both cases, development had already started against the previous requirement, which resulted in avoidable rework and uncertainty about the approved scope.

Going forward, I expect any agreed requirement change to be documented and communicated through the project's agreed change process on the same working day. If a change has not yet been formally approved, that status should also be made explicit.

I recognise that you joined the project relatively recently and that the current change process involves several stakeholders. I would be happy to review the workflow with you and clarify the escalation and approval points so that the process is easier to apply consistently.

We will review progress during our regular 1:1s over the next month. If significant changes continue to reach the delivery team late, we will need to review the process and responsibilities more formally.

Your analytical strengths are valuable to the project, and improving this communication step will make your contribution even more effective.

---

# Prompt 2 — Feedback Quality Review

```text
ROLE

You are an experienced people manager reviewing performance feedback
written by a Project Manager.

TASK

Review the feedback below.

[PASTE FEEDBACK]

Check for:

- vague criticism,
- personality judgments,
- missing examples,
- unsupported assumptions,
- cultural stereotypes,
- unclear expectations,
- lack of support,
- disproportionate consequences,
- language likely to cause defensiveness.

OUTPUT FORMAT

Finding
Why It Matters
Recommended Improvement
```

---

# Prompt 3 — Prepare for the Conversation

Written feedback should usually support a conversation rather than replace one.

```text
ROLE

You are coaching an IT Project Manager before a performance-feedback
conversation.

TASK

Using the feedback below, prepare a discussion guide.

[PASTE FEEDBACK]

OUTPUT FORMAT

1. Opening
2. Strengths to acknowledge
3. Issue to discuss
4. Evidence / example
5. Questions to ask the team member
6. Expectation to set
7. Support to offer
8. Follow-up agreement
```

---

# Ask for the Team Member's Perspective

A feedback conversation should allow two-way discussion.

Questions may include:

```text
How do you see the situation?

Was there anything preventing you from raising the issue earlier?

Was the escalation expectation clear?

What would help you communicate these risks earlier?

Is there anything in the current process that makes this difficult?
```

This may reveal a process problem rather than an individual performance problem.

---

# Prompt 4 — Separate Performance From Process

```text
ROLE

You are a senior Delivery Manager reviewing a recurring team
performance issue.

TASK

Analyse whether the problem below is primarily:

- individual behaviour,
- unclear responsibility,
- poor process,
- insufficient capability,
- workload / capacity,
- or a combination.

SITUATION

[PASTE]

For each potential cause provide:

Evidence
Missing Information
Recommended Action

Do not assume the individual is the sole cause.
```

---

# Performance vs System Issue

Example:

```text
Symptom:
Tester repeatedly reports defects late.
```

Possible causes:

```text
Individual:
Defects not raised promptly.

Process:
No agreed defect-escalation threshold.

Tool:
Notifications not configured.

Capacity:
Tester covering three environments simultaneously.
```

Senior PM thinking requires distinguishing between these possibilities.

---

# Feedback Model

A practical structure is:

```text
Situation
↓
Behaviour
↓
Impact
↓
Expectation
↓
Support
```

---

# Situation

Describe the context.

```text
During the last two weekly delivery reviews...
```

---

# Behaviour

Describe observable action.

```text
...the known integration dependency was not raised.
```

---

# Impact

Describe why it matters.

```text
This reduced the time available to mitigate the schedule impact.
```

---

# Expectation

State what should happen.

```text
Material dependencies should be raised as soon as they are identified.
```

---

# Support

Explain how you can help.

```text
We can review your risk list together before the next three
delivery meetings.
```

---

# Positive Feedback

The same level of specificity should apply to positive feedback.

### Weak

```text
Great job.
```

### Better

```text
Your analysis of the production incident clearly separated the
technical cause from the process failure and helped the team agree
corrective actions within the same day.

That is exactly the level of structured problem-solving we need.
```

---

# Recognition Prompt

```text
ROLE

You are an IT Project Manager providing positive performance
feedback.

TASK

Write concise recognition based on the example below.

[PASTE EXAMPLE]

Include:

Specific behaviour
Positive impact
Capability demonstrated
Why it matters to the project
```

---

# Feedback for Vendor Team Members

Where the team member belongs to a supplier organisation, consider:

```text
Delivery expectation

Contractual responsibility

Supplier governance

Vendor PM involvement
```

Do not treat an external resource exactly like a direct employee where governance differs.

---

# Feedback for Junior Team Members

Provide additional clarity around:

- expected behaviour,
- examples,
- support,
- learning opportunities.

Avoid assuming experience they do not yet have.

---

# Feedback for Senior Team Members

Expect greater ownership around:

- escalation,
- decision-making,
- mentoring,
- dependency management,
- communication.

Keep feedback evidence-based regardless of seniority.

---

# Multicultural / International Teams

Good practices include:

```text
Use plain language

Avoid idioms

Be specific

Check understanding

Avoid stereotypes

Respect different communication styles

Keep project expectations consistent
```

Cultural awareness should improve communication, not lower clarity around project expectations.

---

# Remote-Team Considerations

Remote teams may need clearer explicit expectations around:

```text
Status updates

Availability

Escalation

Documentation

Meeting participation

Decision capture
```

Do not interpret lower visibility as lower performance without evidence.

---

# Agile / Scrum Considerations

Where teams use Scrum, feedback should respect role boundaries and team accountability.

Possible issues include:

- blockers not raised,
- poor collaboration,
- incomplete work,
- weak stakeholder communication.

Do not turn routine Sprint Retrospective observations automatically into formal performance issues.

---

# Kanban Considerations

Useful evidence may include:

- ageing items,
- repeatedly blocked work,
- handoff delays,
- missed service expectations.

Use metrics to understand patterns, not as the sole basis for personal judgment.

---

# Predictive Considerations

Feedback may relate to:

- schedule ownership,
- reporting,
- risk escalation,
- deliverable quality,
- milestone accountability.

---

# Hybrid Considerations

Evaluate both formal project responsibilities and day-to-day delivery behaviour.

---

# Follow-Up

Feedback should have a defined review point.

Use:

```text
Expectation agreed
↓
Support provided
↓
Observe
↓
Review
↓
Recognise improvement or address continued gap
```

---

# Improvement Follow-Up Table

| Expectation | Measure / Evidence | Review Date | Support | Status |
|---|---|---|---|---|

Do not create unnecessary bureaucracy for minor coaching feedback.

---

# Quality Checklist

Before giving feedback, confirm:

- [ ] Strengths are specific
- [ ] Concern is based on observable behaviour
- [ ] Specific example is included
- [ ] Project impact is explained
- [ ] Personal judgments are avoided
- [ ] Cultural stereotypes are avoided
- [ ] Context has been considered
- [ ] Expected behaviour is explicit
- [ ] Support is offered
- [ ] Consequences are proportionate
- [ ] Follow-up is defined
- [ ] Team member has an opportunity to respond

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- leadership,
- team development,
- communication,
- conflict management,
- emotional intelligence,
- performance management.

## PMBOK Relevance

This prompt supports:

- team,
- stakeholders,
- leadership,
- delivery.

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

Sensitive feedback may need input from:

- Line Manager
- People Manager
- HR
- Delivery Manager
- Vendor Manager where appropriate

AI can help structure feedback.

It should not make formal employment, disciplinary, compensation, or termination decisions.

---

# Confidentiality

Performance feedback may contain sensitive employee information.

Do not enter personally identifiable or confidential HR information into public AI tools unless organisational policy allows it.

Where possible, anonymise:

- names,
- personal details,
- HR history,
- performance records.

---

# Prompt Metadata

```text
Prompt ID: STAKE-005
Category: Stakeholder Management
Version: 1.0
Status: Draft
Owner: Project Manager / Team Lead
Reviewer: Line Manager / HR where appropriate
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
| 1.0 | YYYY-MM-DD | Initial IT team-performance feedback framework |
