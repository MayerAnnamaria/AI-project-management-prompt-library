# Stakeholder Complaint Response

## Purpose

Use this prompt to prepare a professional response to a formal stakeholder complaint relating to an IT project, implementation, service transition, system change, or delivery issue.

Typical complaints may concern:

- service disruption,
- missed commitments,
- delayed delivery,
- poor communication,
- system defects,
- data issues,
- failed migration,
- user impact,
- vendor performance,
- inadequate support.

The objective is to respond in a way that is:

- honest,
- accountable,
- empathetic,
- factual,
- solution-oriented,
- and non-defensive.

The goal is not simply to defend the project team.

The goal is to **address the concern, rebuild confidence, and prevent unnecessary escalation**.

---

## Best Used For

**Project phase:**  
Delivery / Testing / Deployment / Hypercare / Operations Transition

**Project type:**  
Software implementation / SaaS / ERP / Cloud / Infrastructure / Data / Digital Transformation

**Primary user:**  
Project Manager / Delivery Manager / Programme Manager / Change Lead / Service Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
When a formal or material stakeholder complaint is received

---

# Prompt

```text id="complaint-response-01"
ROLE

You are a senior IT Project Manager experienced in stakeholder
management, service recovery, difficult communication, escalation,
and international technology delivery.

TASK

Draft a professional response to the stakeholder complaint below.

COMPLAINT RECEIVED

[PASTE COMPLAINT]

CONFIRMED FACTS

[LIST ONLY VERIFIED FACTS]

WHAT WENT WRONG

[DETAILS]

WHAT HAS ALREADY BEEN DONE

[CORRECTIVE ACTIONS]

WHAT IS STILL BEING INVESTIGATED

[DETAILS]

NEXT ACTIONS

[DETAILS]

EXPECTED RESOLUTION / UPDATE

[DATE / TIME]

CONTACT

[NAME / ROLE / CHANNEL]

OUTPUT REQUIREMENTS

The response must:

- acknowledge the concern,
- acknowledge confirmed failures honestly,
- distinguish confirmed facts from ongoing investigation,
- explain corrective actions,
- explain next steps,
- provide a clear update timeline,
- provide direct contact where appropriate,
- remain professional and empathetic,
- avoid defensive or dismissive language.

OUTPUT FORMAT

1. Subject
2. Acknowledgement
3. Confirmed Facts
4. Explanation
5. Corrective Actions
6. Next Steps
7. Update Commitment
8. Contact / Close
```

---

# Core Response Principle

Use:

```text id="complaint-flow"
Listen
↓
Acknowledge
↓
Verify
↓
Own Confirmed Failures
↓
Correct
↓
Follow Up
```

Avoid:

```text id="complaint-bad-flow"
Defend
↓
Blame
↓
Minimise
↓
Argue
```

---

# 1. Acknowledge the Complaint

Start by demonstrating that the concern has been understood.

Example:

```text id="complaint-acknowledgement"
Thank you for raising your concerns regarding the service
interruption and the lack of timely communication during yesterday's
deployment.

We recognise the impact this caused to your team.
```

This does not require accepting every allegation before investigation.

---

# Acknowledge Impact vs Admit Unsupported Fault

Distinguish:

```text id="complaint-distinction"
Acknowledging impact
```

from:

```text id="complaint-admission"
Admitting legal / contractual liability
```

Example:

> We recognise that the outage affected your team's ability to process customer requests.

This acknowledges impact without making unsupported legal conclusions.

---

# 2. Confirmed Facts

State only what has been verified.

Example:

```text id="complaint-confirmed"
Our review confirms that:

- the system became unavailable at 09:17,
- service was restored at 10:42,
- the planned stakeholder notification was not issued before the
  maintenance activity,
- the incident escalation reached the Service Manager later than
  required by the project process.
```

---

# Fact Discipline

Use:

```text id="complaint-fact-rule"
Confirmed Fact
Assumption
Unverified Claim
```

Keep them separate.

Do not present assumptions as conclusions.

---

# 3. Explain What Happened

Provide enough information to create understanding.

Avoid unnecessary technical detail unless the audience requires it.

### Too Technical

```text id="complaint-technical"
The Kubernetes ingress controller failed after a certificate
rotation created an invalid upstream TLS dependency.
```

### Stakeholder Appropriate

```text id="complaint-plain"
The interruption occurred after a configuration change affected
the application's connection to a supporting service.
```

Detailed technical analysis can be provided separately where appropriate.

---

# 4. Accept Confirmed Failures

Where the project genuinely failed to meet an agreed expectation, acknowledge it directly.

Example:

```text id="complaint-own-failure"
The planned communication should have been issued before the
maintenance activity.

That did not happen, and we have addressed this with the project
and service teams.
```

Avoid:

```text id="complaint-defensive"
Unfortunately, these things sometimes happen during complex IT
projects.
```

This can sound dismissive.

---

# 5. Corrective Actions

Explain what has already been done.

Examples:

```text id="complaint-corrective-actions"
Configuration corrected

Service restored

Vendor escalated

Deployment paused

Additional testing introduced

Change approval strengthened

Support coverage increased

Communication process updated

Monitoring enhanced
```

---

# Corrective Action Quality

### Weak

```text id="complaint-action-weak"
We will ensure this does not happen again.
```

### Better

```text id="complaint-action-good"
All production changes now require confirmation that the stakeholder
notification has been issued before the deployment is authorised.
```

Specific controls build more confidence than generic promises.

---

# 6. Next Steps

Explain what happens next.

Use:

```text id="complaint-next-steps"
Investigation

Root cause analysis

Corrective action

Validation

Stakeholder update

Closure
```

Example:

> A full root-cause review is currently in progress. We will validate the corrective actions with the service and infrastructure teams before formally closing the incident.

---

# 7. Provide an Update Commitment

Do not leave the stakeholder uncertain.

Example:

```text id="complaint-update"
We will provide the next written update by 15:00 CET on
18 November, including the confirmed root cause and any additional
preventive actions.
```

If resolution timing is uncertain, commit to the **next update**, not an unsupported resolution date.

---

# 8. Offer a Direct Contact

Where appropriate:

```text id="complaint-contact"
If you would like to discuss the impact directly, please contact
[ROLE / CONTACT].
```

For significant complaints, personal engagement can help de-escalate the issue.

---

# Example Input

```text id="complaint-example-input"
Complaint:

"The CRM was unavailable for more than an hour this morning without
warning. Our agents could not access customer records and we received
no update from the project team until after the service was restored.
This is the second communication problem during this rollout."

Confirmed facts:

- CRM unavailable 09:17–10:42.
- issue occurred after production configuration change.
- service restored.
- stakeholder notification was not sent.
- incident communication began at 10:15.
- root cause review still in progress.

Corrective actions:

- configuration reverted.
- production changes temporarily paused.
- deployment checklist updated.
- Service Manager added to approval process.

Next update:
Tomorrow at 15:00 CET.
```

---

# Example Output

## Subject

**Response to CRM Service Interruption and Communication Concern**

Dear [Name],

Thank you for raising your concerns regarding this morning's CRM service interruption and the communication provided during the incident.

We recognise that the outage affected your team's ability to access customer information and that the absence of an early project update made the situation more difficult to manage.

Our review confirms that the CRM was unavailable between **09:17 and 10:42 CET** following a production configuration change. The service has now been restored.

We have also confirmed that the planned stakeholder communication was not issued promptly. This did not meet the communication standard expected for the rollout.

The configuration change has been reverted, further production changes have temporarily been paused, and the deployment checklist has been updated to require communication confirmation before production approval. The Service Manager has also been added to the approval process.

A full root-cause review remains in progress. We will provide a further written update by **15:00 CET tomorrow**, including the confirmed cause and any additional preventive measures.

If you would like to discuss the operational impact directly, please contact [Project Manager / Service Manager].

Thank you for raising the issue and for your patience while we complete the review.

Kind regards,  
[Project Manager]

---

# Prompt 2 — De-Escalation Review

```text id="complaint-deescalation-review"
ROLE

You are an experienced stakeholder-relations lead reviewing a
response to a formal complaint.

TASK

Review the response below.

[PASTE RESPONSE]

Check for:

- defensive language,
- dismissive language,
- unnecessary blame,
- weak acknowledgement,
- vague corrective actions,
- unsupported promises,
- unclear next steps,
- missing update commitment,
- wording likely to escalate conflict.

OUTPUT FORMAT

Finding
Likely Stakeholder Reaction
Why It Matters
Recommended Revision
```

---

# Prompt 3 — Complaint Investigation Gap Review

```text id="complaint-investigation"
ROLE

You are a senior IT Project Manager reviewing a stakeholder
complaint before responding.

TASK

Compare the complaint with the confirmed facts below.

COMPLAINT

[PASTE]

CONFIRMED FACTS

[PASTE]

Identify:

1. Claims confirmed by evidence
2. Claims not yet confirmed
3. Missing facts
4. Information requiring investigation
5. Immediate corrective actions
6. Appropriate response commitments

Do not assume unverified allegations are true or false.
```

---

# Complaint vs Incident

A complaint may relate to a technical incident, but the two records serve different purposes.

```text id="complaint-vs-incident"
Incident Record
=
Technical / operational event

Complaint Record
=
Stakeholder concern and organisational response
```

Link them where appropriate, but do not treat them as identical.

---

# Complaint Categorisation

Possible categories:

```text id="complaint-categories"
Service disruption

Project delay

Quality

Communication

Data

Support

Scope / expectation

Vendor performance

User experience

Change impact
```

---

# Complaint Register

For significant projects maintain:

| Complaint ID | Stakeholder | Category | Date | Owner | Status | Resolution |
|---|---|---|---|---|---|---|

Suggested statuses:

```text id="complaint-status"
Received
Acknowledged
Investigating
Action in Progress
Responded
Closed
Escalated
```

---

# Response Timing

Do not leave serious complaints unanswered while the full investigation is completed.

Use:

```text id="complaint-response-timing"
Complaint received
↓
Acknowledge
↓
Investigate
↓
Interim update if needed
↓
Full response
↓
Close
```

Where organisational procedures specify response times, follow those requirements.

---

# Interim Response

When investigation will take time:

```text id="complaint-interim"
Thank you for raising this issue.

We are currently reviewing the incident and the communication
process surrounding it.

We will provide a full response by [DATE].

In the meantime, [IMMEDIATE ACTION] has already been implemented.
```

---

# Accountability Without Over-Promising

Use:

```text id="complaint-accountability"
We have confirmed that the notification process was not followed.
```

Avoid:

```text id="complaint-overpromise"
This will never happen again.
```

Prefer:

```text id="complaint-prevention"
We have implemented additional controls designed to reduce the
likelihood of recurrence.
```

---

# Root Cause vs Immediate Cause

Example:

```text id="complaint-root-cause"
Immediate Cause:
Incorrect configuration deployed.

Root Cause:
Change-control checklist did not require independent verification
of the affected configuration.

Corrective Action:
Independent verification added to the production-change process.
```

Where root cause analysis is not complete, say so.

---

# Stakeholder Recovery

For serious complaints, consider whether additional engagement is required.

Possible actions:

```text id="complaint-recovery"
1:1 discussion

Executive follow-up

Service review

Demonstration of corrective controls

Written closure confirmation

Operational readiness review
```

---

# Vendor-Caused Complaint

If a supplier caused the underlying event, do not automatically blame the vendor in the stakeholder response.

Externally:

> The issue has been escalated to the responsible delivery partner and corrective actions are being implemented.

Internally:

Track supplier responsibility through vendor governance and contractual processes.

---

# Sensitive Complaints

Escalate complaints involving:

```text id="complaint-sensitive"
Personal data

Security incidents

Legal allegations

Regulatory concerns

Discrimination

Employee misconduct

Financial loss

Media enquiries
```

to the appropriate specialist teams.

Do not rely solely on AI-generated wording for these cases.

---

# Agile / Scrum Considerations

Complaints may reveal:

- product misunderstanding,
- poor release communication,
- unmet user expectations,
- quality issues.

Feed legitimate lessons into:

- backlog refinement,
- retrospectives,
- release planning,
- stakeholder engagement.

---

# Kanban / Service Considerations

Track recurring complaints against:

- service demand,
- incident patterns,
- ageing work,
- SLA / SLE performance.

Repeated complaints may indicate systemic service-design issues rather than isolated incidents.

---

# Predictive Considerations

Complaints may relate to:

- missed milestones,
- acceptance,
- change impacts,
- stakeholder communication.

Formal governance may require complaint escalation or reporting.

---

# Hybrid Considerations

Use operational feedback from adaptive delivery while maintaining formal complaint and escalation controls where required.

---

# Quality Checklist

Before issuing the response, confirm:

- [ ] Complaint has been acknowledged
- [ ] Stakeholder impact is recognised
- [ ] Confirmed failures are acknowledged
- [ ] Facts are verified
- [ ] Unverified claims are not presented as facts
- [ ] Explanation is understandable
- [ ] Corrective actions are specific
- [ ] Next steps are clear
- [ ] Next update is dated
- [ ] Tone is professional and empathetic
- [ ] Language is not defensive
- [ ] Language is not dismissive
- [ ] Unsupported promises are avoided
- [ ] Appropriate escalation has occurred
- [ ] Direct contact is provided where appropriate

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder engagement,
- communication,
- conflict management,
- issue management,
- leadership,
- governance.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- team,
- communication,
- delivery,
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

Material complaints should be reviewed by appropriate stakeholders such as:

- Project Manager
- Service Manager
- Business Owner
- Communications
- Legal / Compliance where applicable
- Information Security where applicable
- Senior management for escalated matters

AI can help structure a calm, clear response.

It should not determine legal liability, regulatory response, or disciplinary action.

---

# Confidentiality

Complaints may contain:

- personal information,
- security information,
- customer data,
- employee information,
- commercial disputes,
- sensitive operational details.

Share complaint records only with appropriate stakeholders.

---

# Prompt Metadata

```text id="complaint-metadata"
Prompt ID: STAKE-004
Category: Stakeholder Management
Version: 1.0
Status: Draft
Owner: Project Manager / Service Manager
Reviewer: Business Owner / Communications
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Medium / High depending on complaint
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT stakeholder complaint-response framework |
