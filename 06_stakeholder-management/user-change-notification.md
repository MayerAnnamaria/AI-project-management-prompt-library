# User Change Notification

## Purpose

Use this prompt to create a clear, plain-language notification for users, employees, customers, or business teams who will be affected by an upcoming IT change.

Typical situations include:

- system go-live,
- platform migration,
- planned downtime,
- changed login process,
- new business process,
- new application rollout,
- data migration,
- service interruption,
- feature retirement,
- cutover activity.

The objective is to tell affected people:

- what is changing,
- why it is changing,
- when it will happen,
- how they will be affected,
- what they need to do,
- and where they can get help.

The communication should reduce uncertainty without creating unrealistic expectations.

---

## Best Used For

**Project phase:**  
Deployment / Release / Cutover / Change / Migration

**Project type:**  
Software implementation / SaaS / ERP / Cloud / Infrastructure / Digital Transformation

**Primary user:**  
Project Manager / Change Lead / Communications Lead / Product Owner

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Before any material user-facing change

---

# Prompt

```text id="user-notification-01"
ROLE

You are an experienced IT Project Manager and Change Communications
specialist preparing a user notification for an upcoming technology
change.

TASK

Write a clear, professional, plain-language notification for the
affected users described below.

CHANGE CONTEXT

Project:
[PROJECT NAME]

Audience:
[WHO WILL RECEIVE THE MESSAGE]

Change:
[WHAT IS CHANGING]

Reason:
[WHY]

Date / Time:
[WHEN]

Expected duration:
[IF APPLICABLE]

Expected user impact:
[DETAILS]

Actions users must take:
[DETAILS]

What users should expect:
[DETAILS]

Known limitations:
[DETAILS]

Support contact:
[CONTACT / SUPPORT CHANNEL]

Additional information:
[LINK / DOCUMENT / FAQ IF APPLICABLE]

OUTPUT REQUIREMENTS

The communication must:

- use plain language,
- avoid unnecessary technical jargon,
- explain the change clearly,
- explain expected impact honestly,
- avoid over-promising,
- clearly state user actions,
- provide support / contact information,
- remain concise.

OUTPUT FORMAT

1. Subject
2. Opening
3. What Is Changing
4. When It Will Happen
5. What This Means for You
6. What You Need to Do
7. Support / Questions
8. Professional Close
```

---

# Core Communication Principle

Use:

```text id="change-notification-flow"
What
↓
Why
↓
When
↓
Impact
↓
User Action
↓
Support
```

A user should not have to search through the message to understand what is expected.

---

# 1. Subject

The subject should tell users exactly what the communication concerns.

### Weak

```text id="notification-subject-weak"
Important Update
```

### Better

```text id="notification-subject-good"
CRM Upgrade — Planned Service Interruption on 18 November
```

Or:

```text id="notification-subject-example"
New Login Process Starts Monday — Action Required
```

---

# 2. Opening

State the change directly.

Example:

```text id="notification-opening"
We are upgrading the Customer Portal on Saturday, 18 November.
During the upgrade, the portal will be unavailable between
18:00 and 22:00 CET.
```

Avoid unnecessary project background before explaining the user impact.

---

# 3. Explain What Is Changing

Keep the explanation concise.

Example:

```text id="notification-change-example"
The current login process will be replaced with the organisation's
single sign-on service.

After the change, employees will use their normal corporate account
to access the application.
```

---

# Avoid Technical Jargon

Avoid:

```text id="notification-jargon"
The IdP federation will migrate from legacy SAML authentication to
the enterprise OIDC implementation.
```

unless the audience is technical.

For general users prefer:

```text id="notification-plain"
The way you sign in is changing.

From Monday, you will use your normal company login rather than a
separate application password.
```

---

# 4. Explain When

Be precise about:

```text id="notification-timing"
Date

Start time

Expected completion

Affected time zone

Any preparation deadline
```

Example:

> The upgrade will begin at 18:00 CET on Saturday, 18 November and is expected to finish by 22:00 CET.

---

# Timing Rule

Use absolute dates where possible.

Avoid:

```text id="notification-date-weak"
Next Friday
```

Prefer:

```text id="notification-date-good"
Friday, 20 November
```

This is especially important for international teams and forwarded messages.

---

# 5. Explain the User Impact

Tell users what they should realistically expect.

Possible impacts:

```text id="notification-impact"
Temporary service unavailability

Login change

Reduced functionality

Slower service

New workflow

Required password reset

Different screen or navigation

Delayed processing

Read-only period
```

---

# Example

```text id="notification-impact-example"
During the maintenance window you will not be able to create,
update, or view customer records.

Any work already saved before the maintenance window will remain
available after the service returns.
```

Only include the second statement if it has been confirmed.

---

# Be Honest About Disruption

Do not minimise a known impact.

### Weak

```text id="notification-minimise"
You may notice a very small interruption.
```

when the system will be unavailable for four hours.

### Better

```text id="notification-honest"
The application will be unavailable during the four-hour
maintenance window.
```

---

# 6. User Actions

State clearly whether action is required.

Use:

```text id="notification-user-action"
ACTION REQUIRED
```

where appropriate.

Example:

```text id="notification-action-example"
Before Friday:

1. Save any unfinished work.
2. Log out of the application before 18:00.
3. Do not schedule customer-data updates during the maintenance
   window.
```

---

# No Action Required

If users do not need to do anything, say so.

Example:

> No action is required before the upgrade.

This prevents unnecessary questions.

---

# 7. Support Information

Provide:

```text id="notification-support"
Support channel

Support hours

Contact method

Escalation route where appropriate

FAQ / guide
```

Example:

> If you experience problems after the upgrade, contact the IT Service Desk through [support channel].

---

# Support Readiness

Do not send a large-scale change notification before confirming that support teams know:

- what is changing,
- when,
- known issues,
- troubleshooting steps,
- escalation contacts.

---

# Example Input

```text id="notification-example-input"
Project:
CRM Replacement

Audience:
Customer Service employees

Change:
New CRM system will replace the existing application.

Go-live:
Monday, 23 November at 07:00 CET.

Impact:
Old system becomes read-only from Friday 20 November at 18:00.

Data migration:
Runs during the weekend.

User action:
Complete open customer updates before Friday 17:00.
Do not enter updates after this deadline.

Training:
Mandatory training has already been scheduled.

Support:
Hypercare support channel available from Monday.

Known limitation:
Historical attachments older than five years will be migrated during
the first week after launch.
```

---

# Example Output

## Subject

**CRM Go-Live on 23 November — Important Information and Action Required**

Hello,

The new CRM system will go live on **Monday, 23 November at 07:00 CET**.

As part of the transition, the current CRM will become read-only from **Friday, 20 November at 18:00 CET** while customer data is migrated to the new platform.

### What you need to do

Please complete and save any open customer-record updates by **17:00 CET on Friday, 20 November**.

After this deadline, please do not attempt to make further updates in the current CRM.

### What to expect

From Monday morning, you will use the new CRM for customer-service activities.

Historical attachments older than five years may not be immediately available at launch and will continue to be migrated during the first week.

### Support

A dedicated hypercare support channel will be available from Monday for questions or technical issues.

Thank you for your cooperation during the transition.

Kind regards,  
[Project Team]

---

# Prompt 2 — Plain-Language Review

```text id="notification-plain-review"
ROLE

You are a communications editor reviewing an IT project
notification for non-technical users.

TASK

Review the message below.

[PASTE MESSAGE]

Identify:

- technical jargon,
- unclear wording,
- missing user actions,
- unclear dates,
- vague impact statements,
- unnecessary project terminology,
- over-promising.

OUTPUT FORMAT

Original Wording
Issue
Recommended Plain-Language Version
```

---

# Prompt 3 — User Perspective Review

```text id="notification-user-review"
ROLE

You are an employee receiving the notification below without
detailed knowledge of the project.

TASK

Review the communication from the user's perspective.

[PASTE MESSAGE]

Answer:

1. Do I understand what is changing?
2. Do I understand when?
3. Do I understand how I am affected?
4. Do I know what I need to do?
5. Do I know where to get help?
6. What questions would I still have?
```

This is a useful final quality check before distribution.

---

# Prompt 4 — Executive / Manager Version

Managers may need additional context.

```text id="notification-manager"
ROLE

You are an IT Project Manager preparing a manager briefing for
an upcoming system change.

TASK

Convert the user notification below into a concise manager briefing.

[PASTE MESSAGE]

Include:

Change
Business impact
Timing
Team action required
Known risk
Support arrangements
Manager responsibilities
```

---

# Notification Timing

Where possible, communicate early enough for affected users to prepare.

Use a staged approach for major changes:

```text id="notification-timing-flow"
Early Awareness
↓
Detailed Preparation
↓
Final Reminder
↓
Go-Live Communication
↓
Post-Go-Live Update
```

Do not rely only on a last-minute notification.

---

# Example Communication Cadence

For a major system launch:

```text id="notification-cadence"
4 weeks before
→ Awareness

2 weeks before
→ Training / preparation

3–5 days before
→ Final instructions

Day before
→ Reminder

Go-live day
→ Launch confirmation

Post-go-live
→ Known issues / support update
```

The exact cadence should match project scale and organisational needs.

---

# Audience Segmentation

Different users may require different messages.

Examples:

```text id="notification-audience-segments"
End Users

Managers

System Administrators

Support Teams

External Customers

Vendors

Business Partners
```

Do not send the same technical detail to every audience automatically.

---

# Impact-Based Communication

A stakeholder whose work changes significantly needs more information than someone experiencing only a brief outage.

Use:

```text id="notification-impact-engagement"
Low Impact
→ Simple notification

Medium Impact
→ Notification + guide

High Impact
→ Notification + training + manager engagement + support
```

---

# Multilingual Communication

Where users work in multiple languages:

```text id="notification-language"
Define the official source version.

Translate approved content.

Validate technical terminology.

Keep dates and actions consistent across versions.

Provide the same support route.
```

Do not rely on automatic translation for high-impact communications without appropriate review.

---

# Accessibility

Consider:

- readable language,
- accessible document formats,
- descriptive links,
- captions for supporting videos,
- accessible training materials.

---

# User Concern Management

Users may reply with questions or concerns.

Define:

```text id="notification-concerns"
Where questions go

Who owns responses

How common questions become FAQs

How material concerns are escalated
```

---

# Avoid Over-Promising

Avoid:

```text id="notification-overpromise"
There will be no disruption.

The migration will be completely seamless.

You will not experience any issues.
```

unless this can genuinely be guaranteed.

Prefer:

```text id="notification-realistic"
We have planned the migration to minimise disruption.

Support will be available if you experience issues after go-live.
```

---

# Agile / Scrum Considerations

For frequent product releases:

- avoid excessive communication for minor internal changes,
- highlight user-impacting changes,
- use release notes where appropriate,
- communicate material changes separately.

---

# Kanban / Service Considerations

For service changes, notifications may relate to:

- maintenance,
- service interruption,
- new request processes,
- SLA changes,
- support-channel changes.

---

# Predictive Considerations

Large implementation programmes may require structured change communications linked to:

- milestones,
- training,
- cutover,
- operational readiness,
- go-live.

---

# Hybrid Considerations

Use lightweight release communication for routine delivery while maintaining formal communication for material business changes.

---

# Communication Quality Checklist

Before distribution, confirm:

- [ ] Audience is correct
- [ ] Subject is specific
- [ ] Change is clear
- [ ] Reason is understandable
- [ ] Date and time are precise
- [ ] Time zone is provided where required
- [ ] User impact is honest
- [ ] Required action is explicit
- [ ] Deadline is explicit
- [ ] Support route is provided
- [ ] Known limitations are included
- [ ] Technical jargon has been removed
- [ ] Claims are accurate
- [ ] No unrealistic promises are made
- [ ] Support team is prepared
- [ ] Translation is reviewed where required

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- stakeholder engagement,
- communication,
- organisational change,
- transition,
- governance.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- communication,
- delivery,
- value.

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

Material user communications should be reviewed by the appropriate:

- Project Manager
- Change Lead
- Business Owner
- Communications team
- Service Management
- Legal / Compliance where applicable

AI can help create clear and consistent wording.

It should not independently determine what commitments the organisation should make to users.

---

# Confidentiality

Do not include confidential internal project information in broad user communications.

Avoid unnecessarily exposing:

- internal disputes,
- security vulnerabilities,
- vendor problems,
- confidential commercial details,
- personal information.

Communicate what the audience needs to know.

---

# Prompt Metadata

```text id="notification-metadata"
Prompt ID: STAKE-003
Category: Stakeholder Management
Version: 1.0
Status: Draft
Owner: Project Manager / Change Lead
Reviewer: Business Owner / Communications
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
| 1.0 | YYYY-MM-DD | Initial IT user-change notification framework |
