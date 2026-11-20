# User Change Notification

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** STAKE-003 | **Category:** Stakeholder Management

---


## 1. Ready-to-Use Prompt

**Purpose:** Communicate upcoming IT changes in clear, actionable language so affected users understand the timing, impact, required actions, and available support.

**Use case:** Prepare notifications for system launches, platform migrations, planned downtime, login changes, process updates, feature retirement, and other user-facing technology changes.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Change Communications
Specialist experienced in software deployment, organizational
change, service transition, and stakeholder communication.

CONTEXT

Project: [PROJECT NAME]
Change type: [GO-LIVE / MIGRATION / DOWNTIME / PROCESS CHANGE]
Target audience: [USER GROUPS]
Change description: [WHAT IS CHANGING]
Business reason: [WHY THE CHANGE IS REQUIRED]

SCHEDULE

Change date: [EXACT DATE]
Start time: [TIME / TIME ZONE]
Expected completion: [TIME / TIME ZONE]
Preparation deadline: [IF APPLICABLE]
Confirmed timing: [YES / NO]

USER IMPACT

Affected services: [LIST]
Expected disruption: [DETAILS]
New functionality / process: [DETAILS]
Known limitations: [DETAILS]
Data or access implications: [DETAILS]

USER ACTIONS

Required before change: [LIST / NONE]
Required during change: [LIST / NONE]
Required after change: [LIST / NONE]

SUPPORT AND GOVERNANCE

Support contact / channel: [DETAILS]
Support availability: [HOURS]
Training / guide / FAQ: [VERIFIED LINK / REFERENCE]
Communication owner: [ROLE]
Approval status: [APPROVED / PENDING]
Audience languages / locations: [IF RELEVANT]

TASK

Create a concise, user-friendly change notification
that clearly explains what is happening and what
affected users need to do.

STEP 1 — IDENTIFY ESSENTIAL INFORMATION

1. State what is changing and why.
2. Explain the exact change date, time,
   duration, and relevant time zone.
3. Identify affected users, services, and workflows.
4. Distinguish confirmed impact from potential disruption.
5. Include known limitations without minimizing their effect.

STEP 2 — DEFINE USER ACTIONS

6. Specify required actions before, during,
   and after the change.
7. Highlight preparation deadlines.
8. State "No action required" when appropriate.
9. Explain what users should expect after the change.
10. Provide verified support and training information.

STEP 3 — ADAPT COMMUNICATION

11. Use plain language suitable for the audience.
12. Remove unnecessary technical jargon.
13. Prioritize practical user impact over project background.
14. Where appropriate, prepare separate versions for:
    - End users
    - Business managers
    - System administrators
    - Support teams
    - External customers or partners
15. Adjust communication detail to the level of impact:
    - Low: Short notification
    - Medium: Notification and instructions
    - High: Notification, training, manager engagement,
      and coordinated support

STEP 4 — PLAN COMMUNICATION AND FOLLOW-UP

16. Recommend a proportionate notification cadence:
    - Early awareness
    - Detailed preparation
    - Final reminder
    - Go-live confirmation
    - Post-change update
17. Confirm support readiness before distribution.
18. Identify how user questions and concerns are handled.
19. Recommend accessible formats and validated translations
    where required.
20. Identify unresolved information that must be confirmed
    before publication.

RULES

- Do not invent dates, service availability, contacts,
  migration guarantees, or support commitments.
- Do not promise a disruption-free implementation.
- Do not describe unapproved dates as confirmed.
- Do not minimize known downtime or user impact.
- Use exact dates and time zones where appropriate.
- Keep language professional, direct, and accessible.
- Exclude unnecessary internal or confidential information.

OUTPUT FORMAT

1. USER NOTIFICATION — READY TO SEND

Subject: [SPECIFIC CHANGE AND DATE]

Hello [AUDIENCE],

[What is changing and why]

[When the change will happen]

[What this means for users]

[Actions required and deadlines]

[Known limitations and what to expect]

[Support and contact information]

Kind regards,
[AUTHORIZED PROJECT TEAM]

2. USER ACTION CHECKLIST

Timing | Required Action |
Deadline | Affected Group

3. COMMUNICATION PLAN

Audience | Message Purpose |
Channel | Proposed Timing |
Responsible Role

4. SUPPORT AND READINESS CHECK

Requirement | Current Status |
Owner | Action Required

5. USER QUESTIONS AND CONCERNS

Likely Question | Approved Answer /
Information Required | Support Route

6. PUBLICATION QUALITY CHECK

Information Gap | User Impact |
Required Validation | Approval Owner

MANAGEMENT SUMMARY

- Main user impact
- Critical preparation actions
- Communication timing
- Known limitations
- Support readiness
- Approval blockers

Use concise Markdown tables.
Separate the user-facing message from internal planning.
Mark unconfirmed information as "Requires verification".
```

---

## 2. Quality Check

Use this independent review before distributing the notification.

```text
QUALITY CHECK

Act as a Senior IT Communications and PMO Quality Reviewer.

Review the draft notification against the approved
change details and intended audience.

Verify:

1. Clarity: Users immediately understand what is changing.
2. Timing: Dates, time zones, deadlines, and
   expected duration are accurate.
3. Impact: Service disruption, workflow changes,
   and known limitations are explained honestly.
4. Actions: Users know exactly what they must do
   and when.
5. Accuracy: No unverified commitments or
   unsupported guarantees are included.
6. Audience: Content and detail match the
   intended recipients.
7. Support: Contact routes, training,
   and support availability are confirmed.
8. Accessibility: Wording, formatting,
   translations, and channels are appropriate.
9. Governance: Relevant communication,
   business, and service approvals are identified.
10. Usability: The message is concise,
    easy to scan, and free from unnecessary jargon.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Unverified Information: [GAPS]
Publication blockers: [CRITICAL ITEMS]

Do not invent organizational commitments,
confirmed dates, system guarantees, or support details.
```

---

## 3. Practical IT Use Case

### CRM Replacement — Go-Live and User Preparation

**Scenario:** A company is replacing its legacy CRM system. Customer Service employees must complete open customer-record updates before the existing application becomes read-only for weekend data migration.

The Project Manager must communicate the transition, expected limitations, and support arrangements in clear language before go-live.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Replacement |
| Phase | Deployment / Cutover |
| Audience | Customer Service Employees |
| Go-live | 23 November 2026, 07:00 CET |
| Legacy CRM read-only | 20 November 2026, 18:00 CET |
| User preparation deadline | 20 November 2026, 17:00 CET |
| Change | New CRM replaces existing application |
| Main concern | Business continuity and user readiness |
| Support | Dedicated hypercare channel from go-live |

### Example Input

```text
Project: CRM System Replacement

Audience:
Customer Service employees

Change:
New CRM replaces the current application.

Go-live:
Monday, 23 November 2026 at 07:00 CET.

Legacy system:
Read-only from Friday, 20 November
at 18:00 CET.

Data migration:
Scheduled during the weekend.

Required user action:
Complete and save all open customer-record
updates before Friday, 20 November at 17:00 CET.

Do not enter further updates after the deadline.

Training:
Mandatory employee training has been scheduled.

Support:
Dedicated hypercare channel available from Monday.

Known limitation:
Historical attachments older than five years
will be migrated during the first week after launch.

Exact support contact:
Not provided.

Communication approval:
Pending.
```

### Example Output — User Change Notification

#### 1. User Notification — Ready to Send

**Subject: New CRM Goes Live on 23 November — Action Required Before Friday**

Hello,

The new CRM system is scheduled to go live on **Monday, 23 November 2026, at 07:00 CET**, replacing the current application.

The transition will take place over the weekend, when customer data will be migrated to the new system.

**What is changing?**

The current CRM will become read-only from **Friday, 20 November, at 18:00 CET**. From that point, you will no longer be able to update customer records in the existing application.

**What do you need to do?**

Please complete and save all open customer-record updates by **17:00 CET on Friday, 20 November**.

Do not attempt to enter further updates after this deadline.

**What should you expect after go-live?**

From Monday morning, you will use the new CRM for your customer-service activities.

Historical attachments older than five years will not all be available immediately at launch. Their migration is scheduled to continue during the first week.

Mandatory training has already been scheduled to help you prepare for the new system.

**Support**

A dedicated hypercare support channel will be available from Monday to assist with questions or technical issues.

The exact support contact will be confirmed before this notification is distributed.

Thank you for your cooperation during the transition.

Kind regards,  
[CRM Project Team]

*Draft status: Pending communication approval and confirmation of the support contact.*

#### 2. User Action Checklist

| Timing | Required Action | Affected Group |
|---|---|---|
| Before 20 Nov, 17:00 CET | Complete and save open customer updates | Customer Service |
| After 20 Nov, 17:00 CET | Do not enter further updates | Customer Service |
| From 20 Nov, 18:00 CET | Legacy CRM becomes read-only | All CRM users |
| Weekend, 21–22 Nov | Data migration | Project / Technical Teams |
| 23 Nov, 07:00 CET | Begin using new CRM | Customer Service |
| After go-live | Use hypercare support for issues | All affected users |

#### 3. Communication Plan

| Audience | Message Purpose | Recommended Timing | Proposed Owner |
|---|---|---|---|
| Customer Service Employees | Change awareness and preparation | Before cutover | Change Lead |
| Team Managers | Confirm team readiness | Before preparation deadline | Business Owner |
| IT Service Desk | Prepare support procedures | Before go-live | Service Manager |
| Employees | Final action reminder | Before 20 November | Change Lead |
| All CRM Users | Go-live confirmation | After verified availability | Project Team |
| Affected Users | Known issues and support update | After go-live | Service Manager |

The exact communication cadence should be agreed with the business and communications teams.

#### 4. Support and Readiness Check

| Requirement | Current Status | Required Action |
|---|---|---|
| Go-live schedule | Provided | Confirm approved release schedule |
| User action deadline | Provided | Verify against cutover plan |
| Training | Scheduled | Confirm attendance and material availability |
| Hypercare support | Planned | Confirm channel, staffing, and hours |
| Historical attachments | Delayed migration planned | Confirm user-facing limitation |
| Service Desk readiness | Not provided | Brief support personnel |
| Notification approval | Pending | Obtain authorized sign-off |

#### 5. User Questions and Concerns

| Likely Question | Response / Required Information |
|---|---|
| When will the new CRM be available? | Scheduled for 23 November at 07:00 CET |
| Can I update the old CRM during the weekend? | No. It will be read-only from 20 November at 18:00 CET |
| What happens to unfinished customer updates? | Complete and save them by 20 November at 17:00 CET; handling of unfinished changes requires confirmation |
| Will all old attachments be available immediately? | No. Attachments older than five years are scheduled to migrate during the first week |
| Where can I report an issue? | Dedicated hypercare channel; exact contact must be confirmed |
| What if the migration takes longer? | Contingency communication and revised access timing must be confirmed by the project team |

#### 6. Publication Quality Check

| Item | Assessment | Required Correction |
|---|---|---|
| Change description | Clear | None |
| User actions | Clear | None |
| Key dates | Provided | Confirm release approval |
| Service limitations | Explicit | Validate migration commitment |
| Support contact | Missing | Add verified channel |
| Support availability | Not confirmed | Confirm operating hours |
| Communication approval | Pending | Obtain sign-off |
| Contingency messaging | Not provided | Confirm delay communication process |

### Management Decisions

1. **Cutover readiness:** Confirm that the release plan and user preparation deadlines are approved.
2. **Support readiness:** Validate the hypercare channel, staffing, availability, and escalation process before notification.
3. **Business communication:** Approve the user message and ensure managers understand their responsibilities.
4. **Contingency:** Prepare a communication approach if go-live timing or data availability changes.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The communication clearly explains the system change, cutover timeline, required user actions, and known attachment limitation. However, the support contact, service hours, notification approval, and contingency instructions remain unconfirmed.

**Required corrections:**
- Confirm the release schedule and cutover dates.
- Provide the verified support contact and availability.
- Validate the historical attachment migration statement.
- Confirm the contingency communication process.
- Obtain final communication approval.

**Publication blockers:** Missing support details and pending authorized approval.

**Governance:** Supports PMI-aligned stakeholder communication, organizational change, operational readiness, deployment planning, and project governance.

AI-assisted notifications should be reviewed by authorized project and business stakeholders. They must not introduce unsupported service guarantees, unapproved delivery commitments, or confidential information.
