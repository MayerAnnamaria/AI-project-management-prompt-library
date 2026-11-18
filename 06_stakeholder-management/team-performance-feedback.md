# Team Performance Feedback

**Prompt ID:** STAKE-005 | **Category:** Stakeholder Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Prepare fair, specific, and constructive performance feedback that recognizes strengths, addresses observable concerns, and supports measurable improvement.

**Use case:** Provide feedback to IT project team members when communication, quality, ownership, collaboration, or delivery behavior requires recognition or improvement.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager experienced in leading
cross-functional and international technology teams,
performance coaching, stakeholder communication,
and delivery governance.

CONTEXT

Project: [PROJECT NAME]
Team member's role: [ROLE]
Experience level: [LEVEL]
Employment relationship: [EMPLOYEE / VENDOR / OTHER]
Project responsibilities: [LIST]
Feedback type: [DEVELOPMENT / RECOGNITION / MIXED]
Feedback context: [1:1 / WRITTEN REVIEW / PROJECT FOLLOW-UP]

STRENGTHS AND OBSERVATIONS

Demonstrated strengths: [SPECIFIC EXAMPLES]
Performance concern: [OBSERVABLE BEHAVIOR / NONE]
Evidence: [DATES / EVENTS / WORK PRODUCTS]
Project impact: [FACTUAL IMPACT]

RELEVANT CONTEXT

Role expectations: [AGREED RESPONSIBILITIES]
Workload / capacity: [KNOWN FACTS]
Process or tooling constraints: [KNOWN FACTS]
Previous feedback: [IF AVAILABLE]
Team member's perspective: [IF KNOWN]

FUTURE EXPECTATIONS

Required behavior: [SPECIFIC EXPECTATION]
Expected timing: [WHEN]
Communication / delivery process: [HOW]
Available support: [COACHING / TRAINING / RESOURCES]
Follow-up date: [DATE]
Formal management requirements: [IF APPLICABLE]

TASK

Prepare constructive, evidence-based performance feedback.

STEP 1 — ASSESS PERFORMANCE

1. Identify specific strengths and positive contributions.
2. Describe the concern using observable behavior.
3. Reference relevant dates, events, or deliverables.
4. Explain the demonstrated impact on:
   - Delivery and schedule
   - Quality
   - Collaboration
   - Stakeholder confidence
   - Decision-making
5. Separate facts from interpretation.
6. Consider whether the issue may involve:
   - Individual behavior
   - Unclear responsibilities
   - Ineffective processes
   - Workload or capacity
   - Skills or training gaps
   - Tooling or communication barriers
7. Identify missing information before assigning responsibility.

STEP 2 — PREPARE CONSTRUCTIVE FEEDBACK

8. Start with genuine, specific recognition.
9. Explain the concern using:
   Situation → Behavior → Impact.
10. State future expectations clearly:
    - What must change
    - When it must happen
    - Which process or channel applies
    - What successful performance looks like
11. Offer proportionate coaching, resources, or support.
12. Invite the team member to share their perspective.
13. Describe next steps if improvement is insufficient,
    without making unauthorized disciplinary commitments.

STEP 3 — DEFINE FOLLOW-UP

14. Recommend measurable, proportionate follow-up indicators.
15. Establish a reasonable review point.
16. Identify support and accountability arrangements.
17. Recognize improvement when demonstrated.
18. Escalate formal employment matters to the responsible
    Line Manager or HR team where appropriate.

STEP 4 — ADAPT TO CONTEXT

19. For junior members, emphasize clarity and coaching.
20. For senior members, address ownership, escalation,
    communication, and leadership responsibilities.
21. For vendor personnel, respect supplier governance
    and the relevant contractual management structure.
22. For remote or international teams, use clear language
    and verified expectations without cultural assumptions.

RULES

- Do not invent performance incidents or consequences.
- Do not make personality judgments.
- Do not infer motivation, intention, or attitude.
- Do not confuse missing process clarity with poor performance.
- Do not equate lower visibility with lower productivity.
- Avoid discriminatory or culturally stereotyped language.
- Use a firm, fair, respectful, and supportive tone.
- Protect confidential personnel information.
- Do not make formal HR, compensation, or termination decisions.

OUTPUT FORMAT

1. PERFORMANCE FEEDBACK — READY TO USE

Opening and Specific Strengths
Observed Concern and Supporting Example
Project Impact
Expected Behavior
Support and Development
Follow-Up Commitment
Professional Close

2. PERFORMANCE ASSESSMENT

Observation | Evidence | Project Impact |
Confirmed / Unverified | Context

3. ROOT CAUSE AND CONTEXT REVIEW

Potential Cause | Supporting Evidence |
Missing Information | Recommended Action

4. IMPROVEMENT AND SUPPORT PLAN

Expectation | Success Measure |
Support | Review Date | Responsible Role

5. FEEDBACK CONVERSATION GUIDE

Opening | Key Evidence |
Questions for Team Member |
Expected Agreement | Follow-Up

6. MANAGEMENT SUMMARY

- Main strengths
- Specific improvement area
- Project impact
- Support required
- Next review point
- Formal escalation requirements, if applicable

Use professional, direct, and natural language.
Keep feedback proportionate to the issue.
```

---

## 2. Quality Check

Run this independent review before sharing written performance feedback.

```text
QUALITY CHECK

Act as a Senior People Manager and PMO Quality Assurance Reviewer.

Review the performance feedback against the supplied evidence.

Verify:

1. Fairness:
   Recognition and concerns are specific and proportionate.

2. Evidence:
   Observations are supported by facts, examples,
   or documented project outcomes.

3. Objectivity:
   The feedback avoids personality judgments,
   unsupported assumptions, and cultural stereotypes.

4. Context:
   Process, workload, role clarity, and capability
   are considered before assigning responsibility.

5. Impact:
   The relationship between observed behavior
   and project consequences is supported.

6. Expectations:
   Required improvements are specific, achievable,
   and aligned with the person's responsibilities.

7. Support:
   Coaching, resources, and process improvements
   are included where appropriate.

8. Follow-Up:
   Success indicators, review timing, and accountability
   are clear and proportionate.

9. Governance:
   Feedback respects employment boundaries,
   confidentiality, and formal HR responsibilities.

10. Tone:
    The message is respectful, constructive,
    clear, and non-threatening.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Unverified Assumptions: [EVIDENCE GAPS]
Management / HR Review Required: [IF APPLICABLE]

Do not invent performance history, misconduct,
personal motivations, or disciplinary outcomes.
```

---

## 3. Practical IT Use Case

### Software Implementation — Business Analyst Requirement Communication

**Scenario:** During a software implementation project, a Business Analyst produces high-quality requirements documentation and maintains positive relationships with business stakeholders.

However, agreed requirement changes are not always communicated promptly to the development team, resulting in avoidable rework.

The Project Manager must give constructive feedback while checking whether process clarity also contributed to the problem.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Management System Enhancement |
| Phase | Development |
| Delivery approach | Hybrid |
| Team member | Business Analyst |
| Experience on project | Three months |
| Main strengths | Requirements analysis, documentation, stakeholder relationships |
| Performance concern | Delayed requirement-change communication |
| Project impact | Development rework and unclear requirements |
| Management objective | Improve change communication and delivery coordination |

### Example Input

```text
Project:
Customer Management System Enhancement

Role:
Business Analyst

Experience on project:
Three months

Strengths:
- Strong requirements analysis
- Clear, structured documentation
- Positive relationships with business users

Concern:
Important requirement changes are sometimes
discussed with business stakeholders but
communicated late to developers.

Specific evidence:
Two agreed changes last month were entered
into the backlog several days after the
business discussions.

Development had already started using
the previous requirements.

Project impact:
- Rework
- Confusion about current requirements
- Reduced delivery predictability

Expected behavior:
Requirement changes must be documented
and communicated through the agreed
project process on the same working day.

If approval is still pending, that status
must be clearly identified.

Available support:
Project Manager will review the change
process and escalation points with the BA.

Follow-up:
Regular 1:1 discussions over the next month.

Formal disciplinary action:
Not requested.
```

### Example Output — Team Performance Feedback

#### 1. Performance Feedback — Ready to Use

**Subject: Development Feedback — Requirement Change Communication**

Your contribution to requirements analysis and documentation has been valuable to the project. You consistently produce structured requirements and maintain positive working relationships with business stakeholders.

I would like to discuss one area where we need greater consistency: communicating requirement changes to the development team.

Last month, two changes discussed and agreed with business stakeholders were not reflected in the delivery backlog until several days later. Development had already started against the previous requirements, which resulted in rework and uncertainty about the current scope.

Going forward, I expect requirement changes to be documented and communicated through the agreed project process on the same working day. Where formal approval is still pending, that status should be clearly indicated so the development team does not interpret the change as authorized work.

I also want to understand whether any part of the current process makes timely communication difficult. Since you joined the project relatively recently, we can review the change workflow, responsibilities, and escalation points together.

Over the next month, we will review progress during our regular 1:1 meetings and check whether changes are being communicated consistently.

Your analytical and documentation skills are important strengths. Improving this coordination step will help the team reduce rework and maintain greater confidence in the requirements baseline.

#### 2. Performance Assessment

| Observation | Evidence | Project Impact | Assessment |
|---|---|---|---|
| Strong documentation | Reported quality of requirements | Supports delivery clarity | Positive |
| Effective business relationships | Reported stakeholder collaboration | Supports requirements gathering | Positive |
| Delayed change communication | Two changes entered late | Rework and scope confusion | Improvement required |
| Process familiarity | Three months on project | Possible learning need | Requires discussion |
| Communication expectations | Same-day update requested | Supports timely coordination | To be confirmed as agreed process |

**Management interpretation:** The concern is supported by specific observations, but the underlying cause should be discussed before concluding that individual performance is the sole issue.

#### 3. Root Cause and Context Review

| Potential Cause | Current Evidence | Required Clarification |
|---|---|---|
| Delayed individual communication | Two late backlog updates | What prevented timely updates? |
| Unclear change process | Not confirmed | Are approval and communication steps documented? |
| Role ambiguity | Not confirmed | Who owns backlog updates and developer notification? |
| Workload constraints | Not provided | Were competing priorities affecting response time? |
| Tooling or notifications | Not provided | Are developers informed when requirements change? |
| Experience on project | Three months | Is additional process onboarding needed? |

**Assessment:** Individual and process-related causes remain open for validation.

#### 4. Improvement and Support Plan

| Expectation | Success Measure | Support | Review Point |
|---|---|---|---|
| Communicate changes promptly | Changes recorded and communicated within agreed timeframe | Process walkthrough | Weekly |
| Distinguish approved and pending changes | Clear approval status in backlog | Change-status guidance | Weekly |
| Escalate unclear requirements | Questions raised before development proceeds | PM / BA check-in | As needed |
| Improve developer coordination | Fewer delays caused by unclear change communication | Joint BA–Development review | After one month |

The measures should be confirmed with the team member and relevant line manager.

#### 5. Feedback Conversation Guide

**Opening:** Recognize the Business Analyst's contribution to documentation quality and stakeholder collaboration.

**Concern:** Explain the two delayed requirement-change updates and their observed impact on development.

**Questions to ask:**
- How do you see these situations?
- Were the responsibilities and approval steps clear?
- Were there obstacles to updating the backlog promptly?
- What support would make this easier to manage?

**Expected agreement:** Clarify the change process, communication timing, and ownership of backlog updates.

**Support:** Review the workflow and escalation rules together.

**Follow-up:** Check progress during regular 1:1 discussions over the next month.

#### 6. Management Summary

| Area | Management Assessment |
|---|---|
| Strengths | Requirements quality, documentation, business communication |
| Improvement area | Timely change communication |
| Delivery impact | Rework and unclear requirements |
| Potential contributing factors | Role, process, workload, or tooling |
| Support | Change-process coaching |
| Review | Weekly check-ins for one month |
| Escalation | Not currently indicated |

### Management Decisions

1. **Clarify accountability:** Confirm who owns documentation, approval status, and communication of requirement changes.
2. **Improve process:** Ensure the change-control workflow clearly identifies approval and developer notification steps.
3. **Provide support:** Offer focused coaching rather than treating the issue as purely individual performance.
4. **Monitor improvement:** Review timely change communication and recognize sustained progress.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The feedback is specific, respectful, and supported by two reported examples. It acknowledges strengths and proposes practical support. However, the exact change-process expectations and potential contributing factors need confirmation.

**Required corrections:**
- Validate the specific incidents and resulting rework.
- Confirm whether same-day communication is an agreed requirement.
- Discuss the team member's perspective.
- Clarify backlog and change-approval ownership.
- Agree realistic improvement measures and follow-up.

**Unverified assumptions:** Whether the delay resulted from individual behavior, unclear responsibilities, workload, or tooling.

**Management / HR review:** Routine coaching may be appropriate without formal HR involvement. Any formal performance action must follow organizational policy and the responsible line manager's authority.

**Governance:** Supports PMI-aligned team leadership, communication, performance development, issue management, and project delivery.

AI can assist with feedback structure and communication quality, but it cannot determine employee performance ratings, disciplinary outcomes, or employment decisions. Protect confidential personnel information and share feedback only with authorized participants.
