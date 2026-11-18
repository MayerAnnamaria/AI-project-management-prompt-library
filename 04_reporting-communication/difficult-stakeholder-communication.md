# Difficult Stakeholder Communication

**Prompt ID:** REPORT-005 | **Category:** Reporting & Communication | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Communicate difficult project situations clearly and assertively while protecting stakeholder relationships, maintaining accountability, and supporting timely decisions.

**Use case:** Draft professional emails or escalation messages when project delays, unresolved dependencies, vendor commitments, scope conflicts, or overdue decisions require stakeholder action.

Copy the prompt and replace the placeholders with your project information.

```text id="r5stake"
ROLE

You are a Senior IT Project Manager specializing in stakeholder
management, executive communication, conflict resolution,
vendor governance, and project escalation.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Recipient / stakeholder: [ROLE]
Relationship: [COLLABORATIVE / FORMAL / TENSE / ESCALATED]
Communication type: [EMAIL / VENDOR ESCALATION /
EXECUTIVE ESCALATION / DECISION FOLLOW-UP]
Situation: [WHAT HAS OCCURRED]
Known facts and dates: [DETAILS]
Original commitment: [IF APPLICABLE]
Current project impact: [SCHEDULE / COST / QUALITY / SCOPE]
Actions already taken: [LIST]
Recovery measures: [LIST]
Action or decision required: [DETAILS]
Decision owner: [ROLE]
Required deadline: [DATE / TIME / TIME ZONE]
Impact if delayed: [DETAILS]
Governance / contractual requirements: [IF RELEVANT]

TASK

Draft professional, factual, and action-oriented communication.

STEP 1 — STRUCTURE THE MESSAGE

1. Create a subject that clearly identifies the situation
   and required action.
2. State the purpose immediately.
3. Explain what was expected, what occurred, and the
   current status using verified facts.
4. Describe the actual or potential project impact
   without exaggeration or speculation.
5. Summarize actions already taken and recovery measures.
6. Specify the required decision, deliverable, or response.
7. State the deadline, why it matters, and the consequences
   of further delay.
8. Close constructively and reinforce accountability.

STEP 2 — ADAPT TO THE SITUATION

- Vendor escalation:
  Reference missed commitments, previous recovery actions,
  required deliverables, and contractual considerations.

- Overdue stakeholder decision:
  Explain the outstanding decision, affected dependency,
  required deadline, and escalation path.

- Executive escalation:
  Focus on business impact, mitigation, decision required,
  decision authority, and urgency. Maximum 150 words.

- Internal stakeholder conflict:
  Focus on shared objectives, facts, responsibilities,
  and required resolution rather than personal criticism.

STEP 3 — APPLY COMMUNICATION STANDARDS

9. Use the sequence:
   FACTS → IMPACT → ACTION → DECISION → DEADLINE.
10. Maintain a firm, professional, constructive tone.
11. Avoid blame, emotional language, and unnecessary
    defensiveness.
12. Separate confirmed facts from assumptions and forecasts.
13. Make requests specific and measurable.
14. Escalate proportionately to the project impact.
15. Verify contractual references and formal notice
    requirements before including them.

Do not invent facts, commitments, dates, contractual clauses,
approval authority, or consequences.

Do not present an ordinary project email as a formal legal notice.

OUTPUT FORMAT

1. READY-TO-SEND MESSAGE

Subject: [CLEAR SUBJECT]

[PROFESSIONAL GREETING]

[FACTUAL SITUATION AND IMPACT]

[MANAGEMENT / RECOVERY ACTIONS]

[EXPLICIT ACTION OR DECISION REQUIRED]

[DEADLINE AND CONSEQUENCE]

[PROFESSIONAL CLOSE]

2. EXECUTIVE ESCALATION SUMMARY

Issue | Current Impact | Actions Taken |
Decision / Support Required | Decision Owner |
Deadline | Impact if Delayed

Maximum 150 words.

3. COMMUNICATION REVIEW

Potential Misunderstanding | Recipient Concern |
Recommended Clarification

4. MANAGEMENT FOLLOW-UP

Action Required | Owner | Deadline |
Escalation Trigger | Next Follow-Up

Keep the ready-to-send message concise.
Use paragraphs rather than excessive bullet points.
Include only confirmed information.
```

---

## 2. Quality Check

Apply this independent review before sending the communication.

```text id="stakeqa5"
QUALITY CHECK

Act as a Senior QA Manager and Stakeholder Communication Reviewer.

Review the message from both the Project Manager's
and the recipient's perspectives.

Verify:

1. Accuracy: Facts, dates, commitments, and impacts
   are supported by the provided information.
2. Clarity: The situation and required response are
   immediately understandable.
3. Tone: Communication is firm, constructive,
   non-defensive, and free from unnecessary blame.
4. Accountability: Required actions, decision owners,
   and deadlines are explicit.
5. Proportionality: Project impacts and escalation
   consequences are not exaggerated.
6. Recipient Perspective: Likely questions,
   objections, or misunderstandings are addressed.
7. Governance: Escalation authority and contractual
   references are appropriate and verified.
8. Actionability: The recipient knows what to do next.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Recipient Concerns: [LIKELY QUESTIONS / OBJECTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

If needed, provide a revised ready-to-send message.

Do not invent facts, contractual obligations,
organizational authority, or stakeholder commitments.
```

---

## 3. Practical IT Use Case

### Software Development — Overdue Product Owner Decision

**Scenario:** A development team is implementing a reporting feature for an internal business application. The Product Owner has not confirmed the acceptance criteria for a key feature, preventing developers from finalizing implementation and QA from preparing reliable test cases.

The Project Manager must request a decision without creating unnecessary conflict.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Development |
| Delivery approach | Scrum |
| Stakeholder | Product Owner |
| Current issue | Outstanding acceptance criteria decision |
| Impact | Development clarification and test preparation delayed |
| Communication type | Internal stakeholder follow-up |
| Management objective | Obtain an actionable decision and protect the delivery plan |

### Example Input

```text id="stakeex5"
Project: Web Application Reporting Enhancement

Project phase: Development
Delivery approach: Scrum

Stakeholder:
Product Owner

Relationship:
Collaborative

Situation:
Acceptance criteria for the Excel export feature
have not been finalized.

Original decision deadline:
12 May 2027

Current date:
17 May 2027

Outstanding decision:
Confirm whether exports must support
up to 5,000 rows or 20,000 rows.

Known impact:
- Developers cannot finalize the export implementation.
- QA cannot approve the final test scenarios.
- The unresolved requirement may affect the sprint goal.

Actions already taken:
- Developers documented both implementation options.
- QA identified test coverage implications.
- The Project Manager recorded the dependency in Jira.

Required from Product Owner:
Confirm the required export limit
or authorize a short decision meeting.

Required deadline:
18 May 2027, 12:00 CEST.

Impact if delayed:
The team may need to re-plan affected Sprint work.
```

### Example Output — Stakeholder Communication

#### 1. Ready-to-Send Message

**Subject:** Reporting Enhancement — Excel Export Requirements Decision Needed by 18 May

Dear Product Owner,

I am following up on the outstanding acceptance criteria for the Excel export feature, originally scheduled for confirmation on 12 May.

The development and QA teams require a decision on whether the export must support up to 5,000 or 20,000 rows. Without this clarification, the implementation cannot be finalized and the corresponding test scenarios remain incomplete, potentially affecting the current Sprint Goal.

The team has documented both implementation options and their testing implications, and the dependency is tracked in Jira.

Could you please confirm the required export limit by **18 May at 12:00 CEST**? Alternatively, we can arrange a short decision meeting to review the options and agree on the appropriate requirement.

If the decision remains outstanding, we will need to reassess the affected Sprint work and communicate any resulting delivery impact.

Thank you for your support in resolving this dependency.

Kind regards,  
Project Manager

#### 2. Executive Escalation Summary

*Use only if the decision remains unresolved and material project impact is confirmed.*

| Field | Summary |
|---|---|
| Issue | Acceptance criteria for Excel export remain unconfirmed |
| Current impact | Implementation and QA preparation cannot be finalized |
| Actions taken | Technical options documented; dependency recorded in Jira |
| Decision required | Confirm the required export capacity |
| Decision owner | Product Owner |
| Deadline | 18 May 2027, 12:00 CEST |
| Impact if delayed | Potential Sprint replanning and delivery impact |

**Escalation recommendation:** First seek resolution through normal Product Owner and Scrum Team collaboration. Escalate only if the unresolved decision threatens a material commitment or requires authority beyond the team.

#### 3. Communication Review

| Potential Misunderstanding | Recipient Concern | Recommended Clarification |
|---|---|---|
| Why is the decision urgent? | Deadline appears arbitrary | Explain the dependency on implementation and testing |
| What decision is required? | Technical options may be unclear | Present both supported export limits |
| Is the Product Owner being blamed? | Message may feel accusatory | Focus on the unresolved requirement, not individual responsibility |
| What happens if no decision is made? | Consequences may be unclear | Explain that affected Sprint work may require replanning |

#### 4. Management Follow-Up

| Action | Proposed Owner | Deadline | Escalation Trigger |
|---|---|---|---|
| Confirm export acceptance criteria | Product Owner | 18 May, 12:00 | Decision remains outstanding |
| Update Jira requirements | Product Owner / BA | After confirmation | Accepted criteria unavailable |
| Finalize technical implementation | Development Lead | TBD | Clarification not received |
| Finalize test scenarios | QA Lead | TBD | Acceptance criteria remain unclear |
| Assess Sprint impact | Scrum Team | At next coordination point | Sprint Goal becomes threatened |

### Management Decisions

1. **Requirement clarification:** Confirm the expected export limit and acceptance criteria.
2. **Delivery coordination:** Update the backlog and testing documentation once the decision is available.
3. **Schedule management:** Assess whether the outstanding dependency affects the Sprint Goal or release forecast.
4. **Escalation:** Involve higher-level governance only if the decision cannot be resolved within the team's authority and a material commitment is at risk.

### Applied Quality Review

**Quality verdict: PASS**

**Findings:** The message identifies the outstanding decision, its delivery impact, supporting actions, and response deadline. The tone remains constructive and avoids personal criticism. Escalation is conditional rather than unnecessarily immediate.

**Required corrections:** None identified for the illustrative scenario. Before sending, verify the dates, technical options, intended recipient, and response deadline against the actual project records.

**Recipient concerns:** The Product Owner may need a concise explanation of the technical and business differences between the two export limits.

**Approval blockers:** None established from the supplied example.

**Governance:** This framework supports PMI-aligned stakeholder engagement, communication management, issue resolution, leadership, and project governance.

Sensitive communications involving contractual obligations, financial exposure, security incidents, or formal disputes require appropriate human review. AI-generated drafts do not replace authorized contractual notices or legal advice. Protect confidential project, vendor, employee, and security-sensitive information.
