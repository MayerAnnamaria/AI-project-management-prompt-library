# Project Meeting Minutes

**Prompt ID:** REPORT-006 | **Category:** Reporting & Communication | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Convert unstructured project meeting notes into accurate, concise, and actionable records of discussions, decisions, responsibilities, and unresolved dependencies.

**Use case:** Document weekly IT delivery meetings, project status reviews, vendor coordination meetings, testing reviews, or steering committee discussions where decisions and follow-up actions require clear ownership.

Copy the prompt and replace the placeholders with your meeting information.

```text id="minutes01"
ROLE

You are a Senior IT Project Manager and Project Coordinator
experienced in software delivery, stakeholder communication,
meeting documentation, action tracking, and governance.

CONTEXT

Project: [PROJECT NAME]
Meeting type: [DELIVERY / TESTING / VENDOR / GOVERNANCE / OTHER]
Meeting date: [DATE]
Time / time zone: [IF KNOWN]
Location / platform: [IF KNOWN]
Chair: [NAME / ROLE]
Participants: [LIST]
Apologies: [IF APPLICABLE]
Minutes prepared by: [NAME / ROLE]
Previous actions: [PASTE IF AVAILABLE]
Raw meeting notes: [PASTE NOTES]
Next meeting: [IF KNOWN]
Reporting date: [DATE, FOR ACTION FOLLOW-UP]
Documentation level: [FORMAL / STANDARD / BRIEF]

TASK

Create structured Project Meeting Minutes from the supplied notes.

STEP 1 — STRUCTURE THE MEETING RECORD

1. Capture meeting details without inventing missing information.
2. Summarize previous actions, including status and outstanding work.
3. Organize discussion into concise, numbered agenda topics.
4. Distinguish factual updates, proposals, decisions,
   and unresolved questions.
5. Extract only decisions explicitly agreed during the meeting.
6. Record decision authority, conditions, and effective dates
   where supported by the notes.

STEP 2 — EXTRACT ACTIONS AND DEPENDENCIES

7. Identify specific follow-up actions and expected outputs.
8. Record Action Owner, Due Date, Priority, and Status
   only where supported by available information.
9. Flag missing owners or deadlines as "To be confirmed".
10. Capture new risks, existing issues, blockers,
    dependencies, and required decisions separately.
11. Identify actions that are overdue, blocked, or due
    within the next seven days where dates are available.

STEP 3 — SUPPORT PROJECT GOVERNANCE

12. Identify material decisions for the central Decision Log.
13. Identify actions for the project Action Tracker.
14. Identify risks, issues, and dependencies for the RAID register.
15. Highlight unresolved items requiring management attention.
16. Record the next meeting and required inputs where known.

Do not invent decisions, agreements, ownership, dates,
priorities, approvals, or action completion.

Keep discussion summaries factual, neutral, and concise.
Do not create a transcript.

Adapt documentation detail to meeting importance:
- Formal governance: decisions, approvals, risks, escalations.
- Delivery coordination: progress, blockers, dependencies, actions.
- Working sessions: concise decision and action summary.

For Agile teams, avoid duplicating Jira or Scrum event records
unless material decisions or cross-team commitments require capture.

OUTPUT FORMAT

1. MEETING DETAILS

Meeting | Project | Date | Time | Platform |
Chair | Participants | Apologies | Minutes Prepared By

2. PREVIOUS ACTIONS

Action ID | Action | Owner | Original Due Date |
Status | Comment

3. AGENDA ITEMS DISCUSSED

Topic | Key Discussion | Project Impact |
Unresolved Point

4. DECISIONS MADE

Decision ID | Decision | Decision Owner |
Effective Date | Conditions

5. NEW ACTION ITEMS

Action ID | Action | Expected Output |
Owner | Due Date | Priority | Status

6. RISKS, ISSUES, AND DEPENDENCIES

Type | Description | Project Impact |
Owner | Required Follow-Up

7. ACTION FOLLOW-UP

Action | Owner | Due Date | Status |
Concern | Required Follow-Up

8. NEXT MEETING

Date | Time | Purpose | Required Inputs

9. GOVERNANCE UPDATE

Record Type | Item | Target Register |
Required Update | Proposed Owner

MANAGEMENT SUMMARY

- Key decisions
- Critical actions and deadlines
- Open blockers and dependencies
- Items requiring escalation or confirmation

Use concise Markdown tables.
Mark unavailable details as "Not provided".
Do not infer agreement from discussion alone.
```

---

## 2. Quality Check

Apply this independent review before distributing the minutes.

```text id="minutesqa"
QUALITY CHECK

Act as a Senior PMO Quality Assurance Manager.

Review the meeting minutes against the original notes.

Verify:

1. Accuracy: Facts, dates, participants, and statuses
   match the available source information.
2. Decisions: Agreed decisions are distinguished from
   proposals, opinions, and discussion.
3. Actions: Follow-ups are specific, with supported owners,
   deadlines, and expected outputs.
4. Completeness: Material discussion points, unresolved
   questions, blockers, risks, and dependencies are captured.
5. Traceability: Decision IDs, Action IDs, and references
   support follow-up and central register updates.
6. Consistency: No conflicting deadlines, action statuses,
   or unsupported completion claims.
7. Governance: Important decisions and actions are identified
   for the relevant project registers.
8. Professionalism: Minutes are concise, neutral,
   and free from personal interpretation.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Confirmation Required: [MISSING OWNERS / DATES / DECISIONS]

Do not invent decisions, actions, deadlines, or approvals.
Flag ambiguous statements for meeting-chair confirmation.
```

---

## 3. Practical IT Use Case

### Software Development — Weekly Delivery Coordination Meeting

**Scenario:** A software team is preparing a reporting feature for production release. During the weekly coordination meeting, the Project Manager reviews development progress, open defects, integration dependencies, and testing readiness.

The objective is to convert rough notes into a structured record that supports Jira tracking, responsibility assignment, and release management.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Meeting type | Weekly Delivery Coordination |
| Delivery approach | Scrum |
| Phase | Development / Testing |
| Participants | Project Manager, Product Owner, Development Lead, QA Lead |
| Tools | Jira, Confluence, Microsoft Teams |
| Main concerns | API integration, open defects, testing readiness |
| Management objective | Confirm decisions, owners, and delivery dependencies |

### Example Input

```text id="minutesinput"
Project: Web Application Reporting Enhancement

Meeting: Weekly Delivery Coordination
Date: 7 June 2027
Time: 10:00–10:30
Platform: Microsoft Teams
Chair: Project Manager

Participants:
PM, Product Owner, Development Lead, QA Lead

Previous actions:
A-01 API specification review — Development Lead — complete
A-02 Regression test plan — QA Lead — still in progress

Rough notes:

- Reporting API integration mostly done.
- 2 defects open in Jira, one Severity 1.
- Development Lead expects fix by Wednesday 9 June.
- QA says regression testing can continue on unaffected features.
- PO wants UAT to start on 14 June.
- QA says UAT should not start with the Sev1 defect open.
- Team agreed: UAT start depends on Sev1 resolution and retest.
- Development Lead to provide fix by 9 June.
- QA Lead to retest by 11 June if fix available.
- PM to update release readiness status after retest.
- Next meeting Monday 14 June at 10:00.
```

### Example Output — Project Meeting Minutes

#### 1. Meeting Details

| Field | Details |
|---|---|
| Meeting | Weekly Delivery Coordination |
| Project | Web Application Reporting Enhancement |
| Date | 7 June 2027 |
| Time | 10:00–10:30 |
| Platform | Microsoft Teams |
| Chair | Project Manager |
| Participants | Project Manager, Product Owner, Development Lead, QA Lead |
| Minutes prepared by | Not provided |

#### 2. Previous Actions

| Action ID | Action | Owner | Due Date | Status |
|---|---|---|---|---|
| A-01 | Review API specification | Development Lead | Not provided | Complete |
| A-02 | Prepare regression test plan | QA Lead | Not provided | In Progress |

#### 3. Agenda Items Discussed

| Topic | Key Discussion | Project Impact | Unresolved Point |
|---|---|---|---|
| API integration | Integration substantially completed | Final readiness requires confirmation | Remaining integration work |
| Open defects | Two defects open, including one Severity 1 | Testing and UAT readiness affected | Critical defect resolution |
| Regression testing | Unaffected features can continue testing | Some test progress maintained | Final completion forecast |
| UAT readiness | Product Owner requested 14 June start | UAT depends on successful retesting | Critical defect closure |

#### 4. Decisions Made

| Decision ID | Decision | Decision Owner | Effective Date | Conditions |
|---|---|---|---|---|
| D-01 | UAT start is conditional on resolution and successful retesting of the Severity 1 defect | Not confirmed | Before UAT | Severity 1 fix and retest completed |

The notes establish that the team agreed on this condition; they do not establish formal UAT approval authority.

#### 5. New Action Items

| Action ID | Action | Expected Output | Owner | Due Date | Status |
|---|---|---|---|---|---|
| A-03 | Provide fix for Severity 1 defect | Corrected build | Development Lead | 9 June 2027 | Open |
| A-04 | Retest Severity 1 defect, subject to fix availability | Verified test result | QA Lead | 11 June 2027 | Open |
| A-05 | Update release readiness status after retest | Updated project status | Project Manager | After retest | Open |

Priorities were not explicitly assigned during the meeting.

#### 6. Risks, Issues, and Dependencies

| Type | Description | Project Impact | Proposed Owner | Required Follow-Up |
|---|---|---|---|---|
| Issue | One Severity 1 defect remains open | UAT readiness blocked | Development Lead | Fix and retest |
| Dependency | QA retesting depends on fix availability | Retest could be delayed | QA Lead | Confirm corrected build |
| Risk | UAT may not start on 14 June if retesting is unsuccessful | Release schedule exposure | Project Manager | Reassess UAT readiness |
| Dependency | Final release readiness depends on test outcome | Approval timing affected | Project Manager | Update status after retest |

#### 7. Action Follow-Up

| Action | Owner | Due Date | Status | Required Follow-Up |
|---|---|---|---|---|
| Complete regression plan | QA Lead | Not provided | In Progress | Confirm completion date |
| Deliver critical defect fix | Development Lead | 9 June | Open | Verify availability |
| Retest critical defect | QA Lead | 11 June | Open | Record results in Jira |
| Update readiness status | Project Manager | After retest | Open | Communicate outcome |

#### 8. Next Meeting

| Field | Details |
|---|---|
| Date | 14 June 2027 |
| Time | 10:00 |
| Purpose | Review defect resolution and UAT readiness |
| Required inputs | Defect fix status, QA retest evidence, updated readiness assessment |

The meeting purpose and required inputs are proposed based on the discussion; they were not explicitly agreed in the notes.

#### 9. Governance Update

| Record Type | Item | Target Register | Required Update | Proposed Owner |
|---|---|---|---|---|
| Decision | D-01 UAT entry condition | Decision Log | Record and validate decision authority | Project Manager |
| Action | A-03 Critical defect fix | Jira / Action Tracker | Track fix completion | Development Lead |
| Action | A-04 Defect retesting | Jira / Action Tracker | Record test outcome | QA Lead |
| Issue | Open Severity 1 defect | Issue Log / Jira | Maintain status and impact | Project Manager |
| Risk | Potential UAT delay | Risk Register | Assess likelihood and schedule impact | Project Manager |

### Management Decisions

1. **Defect resolution:** Confirm that the Severity 1 fix is delivered by 9 June and successfully retested by 11 June.
2. **UAT readiness:** Validate the agreed testing condition and obtain formal UAT start authorization where required.
3. **Release reporting:** Update project status based on verified defect and testing evidence.
4. **Governance:** Transfer material decisions, actions, issues, and risks into their authoritative project registers.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The minutes capture the main topics, confirmed UAT condition, and action ownership. However, decision authority, the regression-plan deadline, and some proposed next-meeting details require clarification.

**Required corrections:**
- Confirm who is authorized to approve UAT start.
- Obtain the missing regression test plan deadline.
- Validate proposed meeting purpose and preparation inputs.
- Confirm that the meeting chair agrees with the final decision record.

**Confirmation Required:** Formal UAT approval authority and outstanding action deadline.

**Governance:** This template supports PMI-aligned stakeholder communication, decision management, issue tracking, and project governance.

Meeting minutes are an official project record only after the appropriate review and distribution process. AI-generated minutes do not establish decisions or commitments beyond what participants actually agreed. Protect confidential project, employee, vendor, customer, and security-sensitive information.
