# Project Meeting Minutes

## Purpose

Use this prompt to convert rough meeting notes into structured, professional project minutes.

The goal is to create a clear record of:

- what was discussed,
- what was decided,
- what actions were agreed,
- who owns each action,
- when actions are due,
- and what remains unresolved.

The objective is not to produce a transcript.

The objective is to create a concise, reliable project record.

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
After formal project meetings

---

# Prompt

```text id="minutes-01"
ROLE

You are an experienced IT Project Manager / Project Coordinator
converting rough meeting notes into formal project minutes.

TASK

Convert the notes below into clear, structured, professional
meeting minutes.

Do not invent decisions, owners, deadlines, or facts that are
not supported by the notes.

MEETING DETAILS

Meeting type:
[TYPE]

Project:
[PROJECT NAME]

Date:
[DATE]

Chair:
[NAME / ROLE]

Participants:
[LIST]

Apologies:
[IF APPLICABLE]

RAW NOTES

[PASTE ROUGH NOTES EXACTLY AS CAPTURED]

OUTPUT FORMAT

1. Meeting Details
2. Previous Actions Update
3. Agenda Items Discussed
4. Decisions Made
5. New Action Items
6. Risks / Issues / Dependencies Identified
7. Next Meeting Details
```

---

# 1. Meeting Details

Provide:

```text id="minutes-details"
Meeting:
Project:
Date:
Time:
Location / Platform:
Chair:
Participants:
Apologies:
Minutes prepared by:
```

Do not invent missing details.

Use:

> Not provided

where necessary.

---

# 2. Previous Actions Update

Provide:

| Action | Owner | Original Due Date | Status | Comment |
|---|---|---|---|---|

Suggested statuses:

```text id="minutes-action-status"
Open
In Progress
Complete
Overdue
Blocked
Deferred
```

Do not mark an action complete unless the notes support it.

---

# 3. Agenda Items Discussed

Summarise topics in numbered sections.

Example:

```text id="minutes-agenda-example"
1. Integration Status
2. Data Migration
3. Testing Readiness
4. Security Review
5. Vendor Dependencies
6. Release Planning
```

For each item capture:

- key facts,
- relevant discussion,
- impact,
- unresolved points.

Avoid writing every conversational detail.

---

# Discussion vs Decision

Keep these separate.

### Discussion

> The team reviewed the remaining integration defects and discussed the impact on the planned UAT start.

### Decision

> Decision: UAT will not start until both Severity 1 defects are resolved and retested.

A statement should only appear under **Decisions Made** if the notes clearly show that a decision was agreed.

---

# 4. Decisions Made

Provide a numbered list.

Example:

```text id="minutes-decisions"
D-01:
UAT entry criteria will require zero open Severity 1 defects.

D-02:
The project will continue using the mock authentication service
until production certification is completed.
```

Where useful include:

| Decision ID | Decision | Decision Owner | Effective Date |
|---|---|---|---|

---

# Decision Recording Rule

A strong decision record should capture:

```text id="minutes-decision-rule"
What was decided
Who had authority
When it applies
Any conditions
```

Avoid vague wording:

```text id="minutes-decision-weak"
The team discussed release timing.
```

Prefer:

```text id="minutes-decision-good"
Decision:
The release remains scheduled for 30 September, subject to security
approval being completed by 20 September.
```

---

# 5. New Action Items

Provide:

| Action ID | Action | Owner | Due Date | Priority | Status |
|---|---|---|---|---|---|

Use specific action wording.

### Weak

```text id="minutes-action-weak"
Follow up on testing.
```

### Better

```text id="minutes-action-good"
QA Lead to confirm retest completion for both Severity 1 defects
by 16 June.
```

---

# Action Quality Rule

Each action should ideally contain:

```text id="minutes-action-rule"
Action
Owner
Deadline
Expected Output
```

If the notes do not contain an owner or date, flag:

```text id="minutes-action-gap"
Owner:
To be confirmed

Due Date:
To be confirmed
```

Do not guess.

---

# 6. Risks / Issues / Dependencies Identified

Capture material items raised during the meeting.

Provide:

| Type | Description | Impact | Owner | Next Action |
|---|---|---|---|---|

Type may be:

```text id="minutes-type"
Risk
Issue
Dependency
Blocker
Decision Dependency
```

This helps connect meeting discussion to the RAID process.

---

# 7. Next Meeting Details

Provide:

```text id="minutes-next"
Next Meeting:
Date:
Time:
Purpose:
Required Inputs:
```

If not known, state:

> To be confirmed.

---

# Example Input

```text id="minutes-example-input"
Meeting:
Integration Coordination

Project:
Customer Portal

Chair:
Project Manager

attendees - PM, integration lead, QA lead, vendor lead, product owner

previous action - vendor recovery plan done, API certification still open

integration - mock service working, identity certification expected Friday

QA - 2 sev1 defects last week, one fixed and retested, one still open

PO - business wants UAT to start Monday if possible

QA says cannot recommend UAT while sev1 defect still open

agreed - no UAT start until sev1 closed and retested

vendor lead to confirm certification Friday by 2pm

QA lead to retest defect by Monday 10am if fix delivered Friday

PM to update sponsor if either item slips

next meeting Monday 11am
```

---

# Example Output

## Meeting Details

**Meeting:** Integration Coordination  
**Project:** Customer Portal  
**Chair:** Project Manager  
**Participants:** Project Manager, Integration Lead, QA Lead, Vendor Lead, Product Owner

---

## Previous Actions Update

| Action | Owner | Status |
|---|---|---|
| Submit vendor recovery plan | Vendor | Complete |
| Complete API certification | Vendor | Open |

---

## Agenda Items Discussed

### 1. Identity Certification

The mock authentication service is operational. Production certification remains outstanding and is currently expected on Friday.

### 2. Critical Defects

Of the two Severity 1 defects previously open, one has been fixed and successfully retested. One remains unresolved.

### 3. UAT Readiness

The Product Owner requested a Monday UAT start. QA advised that UAT should not begin while a Severity 1 defect remains open.

---

## Decisions Made

**D-01:** UAT will not start until the remaining Severity 1 defect has been resolved and successfully retested.

---

## New Actions

| Action | Owner | Due Date | Priority |
|---|---|---|---|
| Confirm API certification status | Vendor Lead | Friday 14:00 | High |
| Retest remaining Severity 1 defect, subject to fix delivery | QA Lead | Monday 10:00 | Critical |
| Escalate to Sponsor if either dependency slips | Project Manager | As required | High |

---

## Risks / Dependencies

| Type | Description | Impact |
|---|---|---|
| Dependency | API certification remains outstanding | Integration completion risk |
| Issue | One Severity 1 defect remains open | UAT cannot start |

---

## Next Meeting

**Monday, 11:00**

Purpose: Review UAT readiness and outstanding integration dependencies.

---

# Prompt 2 — Minutes Quality Review

```text id="minutes-review"
ROLE

You are a PMO Lead reviewing formal project meeting minutes.

TASK

Review the minutes below.

[PASTE MINUTES]

Check for:

- decisions hidden in discussion text,
- actions without owners,
- actions without deadlines,
- vague action wording,
- unsupported conclusions,
- inconsistent dates,
- unresolved dependencies,
- risks or issues that should be captured formally.

OUTPUT FORMAT

Finding
Why It Matters
Recommended Correction
Priority
```

---

# Prompt 3 — Extract Decisions and Actions

For long meetings:

```text id="minutes-extract"
ROLE

You are an IT Project Coordinator reviewing meeting notes.

TASK

Extract only decisions and actions from the notes below.

[PASTE NOTES]

OUTPUT FORMAT

DECISIONS

Decision ID
Decision
Decision Owner
Condition

ACTIONS

Action ID
Action
Owner
Due Date
Priority
```

Do not infer missing information.

---

# Prompt 4 — Action Follow-Up

Use meeting minutes to create an action follow-up list.

```text id="minutes-followup"
ROLE

You are a Project Manager reviewing open actions from recent
meeting minutes.

TASK

Identify:

- overdue actions,
- actions due in the next 7 days,
- blocked actions,
- actions without owners,
- actions without deadlines.

OUTPUT FORMAT

Action
Owner
Due Date
Status
Concern
Required Follow-Up
```

---

# Meeting Minutes Principles

Minutes should be:

```text id="minutes-principles"
Accurate
Concise
Neutral
Action-oriented
Traceable
Easy to review
```

Minutes should not be:

```text id="minutes-avoid"
A transcript
A personal opinion
A rewrite of every sentence spoken
A place to add decisions that were never agreed
```

---

# Formal vs Informal Meetings

Not every meeting requires detailed formal minutes.

## Formal Governance Meeting

Capture:

- decisions,
- approvals,
- risks,
- escalations,
- actions,
- deadlines.

## Delivery Coordination Meeting

Focus on:

- blockers,
- dependencies,
- decisions,
- actions.

## Working Session

A short action and decision summary may be sufficient.

Use documentation effort proportional to governance importance.

---

# Agile / Scrum Considerations

Do not create unnecessary formal minutes for every Scrum event.

For example, Daily Scrum normally does not need formal meeting minutes.

Formal capture may still be useful for:

- cross-team decisions,
- governance decisions,
- major dependencies,
- external vendor commitments,
- release decisions.

---

# Kanban Considerations

Where relevant, meeting output may capture:

- blocked items,
- ageing work,
- dependency actions,
- WIP policy decisions,
- service-delivery decisions.

The board remains the operational source of work status where applicable; minutes should capture important decisions and commitments rather than duplicate the board.

---

# Predictive Considerations

Formal minutes may be particularly important for:

- milestone reviews,
- change-control meetings,
- vendor reviews,
- risk reviews,
- steering committees.

---

# Hybrid Considerations

Keep formal governance records where required while allowing delivery teams to use lighter-weight documentation for routine coordination.

---

# Decision Log Integration

After the meeting, material decisions should be transferred to the project decision log.

Example:

| Decision ID | Meeting | Decision | Date | Owner |
|---|---|---|---|---|

This prevents important decisions from becoming difficult to find across multiple sets of meeting minutes.

---

# Action Log Integration

Likewise, project-critical actions should feed the central action tracker.

Use:

```text id="minutes-integration"
Meeting Minutes
↓
Decision Log
+
Action Log
+
Risk / Issue Register where relevant
```

Meeting minutes should not become an isolated information repository.

---

# Quality Checklist

Before distributing minutes, confirm:

- [ ] Meeting details are correct
- [ ] Participants are correct
- [ ] Previous actions are updated
- [ ] Discussion is concise
- [ ] Decisions are clearly separated
- [ ] Actions are specific
- [ ] Owners are assigned where known
- [ ] Deadlines are recorded where known
- [ ] Missing information is not invented
- [ ] Risks and issues are identified
- [ ] Dependencies are visible
- [ ] Next meeting information is included where known
- [ ] Important decisions are transferred to the decision log
- [ ] Critical actions are transferred to the action tracker

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- communication,
- stakeholder engagement,
- governance,
- action tracking,
- decision management,
- issue and risk management.

## PMBOK Relevance

This prompt supports:

- stakeholders,
- governance,
- delivery,
- team coordination,
- communication.

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

Before formal distribution, confirm:

- decisions accurately reflect what was agreed,
- actions have correct owners,
- deadlines are accurate,
- sensitive information is appropriate for the distribution list.

AI can structure rough notes.

It should not invent decisions or agreements that did not occur.

---

# Confidentiality

Meeting notes may contain sensitive information.

Protect:

- commercial discussions,
- vendor performance concerns,
- security issues,
- employee information,
- customer information,
- confidential decisions.

Use anonymised information in public AI tools where required.

---

# Prompt Metadata

```text id="minutes-metadata"
Prompt ID: REPORT-006
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager / Project Coordinator
Reviewer: Meeting Chair
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT meeting-minutes framework |
