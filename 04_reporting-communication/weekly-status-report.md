# Weekly Project Status Report

**Prompt ID:** REPORT-001 | **Category:** Reporting & Communication | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Convert weekly project updates into concise, evidence-based reports that communicate delivery health, progress, risks, and required management actions.

**Use case:** Prepare weekly status reports for IT project sponsors, delivery managers, and stakeholders when project progress, blockers, dependencies, and upcoming decisions require visibility.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software
delivery, stakeholder communication, risk management,
performance monitoring, and project governance.

CONTEXT

Project: [PROJECT NAME]
Reporting period: [DATE RANGE]
Current phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target milestone / release: [DATE]
Reported overall RAG: [GREEN / AMBER / RED / UNKNOWN]
Previous-week status: [IF AVAILABLE]
Approved baselines / tolerances: [IF AVAILABLE]

ROUGH WEEKLY NOTES

[PASTE NOTES]

Notes may include:
- Completed deliverables and progress
- Milestones and delivery metrics
- Risks, issues, defects, and blockers
- Vendors and external dependencies
- Quality, security, and testing
- Budget and resource changes
- Management decisions
- Next-week priorities

TASK

Create a professional Weekly Project Status Report.

STEP 1 — ASSESS PROJECT HEALTH

1. Evaluate project health using available evidence:
   schedule, scope, cost, quality, risks, dependencies,
   security, and release readiness.
2. Validate the reported RAG status:
   - Green: Commitments remain achievable within tolerance.
   - Amber: Material exposure requires active management
     but commitments may remain achievable.
   - Red: Major commitments are not achievable under the
     current plan or agreed tolerance is exceeded.
3. Identify contradictions between RAG status and evidence.
4. Explain material changes from the previous reporting period.

STEP 2 — REPORT DELIVERY PERFORMANCE

5. Summarize completed or materially advanced work.
6. Focus on outcomes rather than meetings or routine activities.
7. Identify material risks, existing issues, blockers,
   and external dependencies.
8. Explain business or delivery impact, current actions,
   ownership, and relevant deadlines.
9. Highlight only metrics that support management decisions.

STEP 3 — DEFINE NEXT ACTIONS

10. Identify the most important outcomes for next week.
11. Separate decisions from operational follow-up actions.
12. Specify decisions required, responsible authority,
    deadline, recommendation, and impact if delayed.
13. Flag missing owners, dates, or evidence for confirmation.

Adapt reporting to the delivery approach:
- Agile / Scrum: Sprint Goals, release progress, blockers,
  quality, and cross-team dependencies.
- Kanban: WIP, work-item age, cycle time, throughput,
  blocked items, and SLE performance.
- Predictive: Milestone variance, critical path,
  budget, and approved changes.
- Hybrid: Combine delivery evidence with formal commitments.

Do not invent facts, owners, deadlines, or approvals.
Do not assume the project is on track without evidence.
Clearly distinguish risks from materialized issues.

OUTPUT FORMAT

1. PROJECT STATUS SUMMARY

Overall RAG | Previous RAG | Trend |
One-Sentence Rationale

Executive summary:
3–4 sentences covering delivery position, key progress,
main concern, and management attention required.

2. THIS WEEK'S PROGRESS

Deliverable / Workstream | Achievement |
Evidence / Metric | Management Significance

3. KEY RISKS, ISSUES, AND DEPENDENCIES

Type | Description | Impact |
Current Action | Owner | Due Date

4. NEXT WEEK'S PRIORITIES

Priority | Expected Outcome |
Owner | Target Date | Dependency

5. DECISIONS AND ACTIONS REQUIRED

Type | Decision / Action | Required From |
Recommendation | Deadline | Impact if Delayed

MANAGEMENT SUMMARY

- Current project health
- Main achievement
- Most critical exposure
- Immediate decisions and next steps

Use concise Markdown tables.
Mark missing information as "Not provided".
Label proposed actions and unconfirmed ownership.
```

---

## 2. Quality Check

Apply this independent review before distributing the weekly report.

```text
QUALITY CHECK

Act as a Senior PMO Quality Assurance Manager.

Review the Weekly Project Status Report against
the original project notes.

Verify:

1. Accuracy: Facts, metrics, dates, and status align
   with the provided evidence.
2. RAG: Overall status is justified and consistent
   with approved project tolerances.
3. Progress: Achievements describe measurable outcomes,
   not routine activity.
4. Risks and Issues: Uncertain risks are distinguished
   from existing problems and dependencies.
5. Accountability: Material actions have supported
   owners, deadlines, and expected outcomes.
6. Decisions: Governance requests are explicit,
   justified, and time-sensitive where appropriate.
7. Forecast: Next-week priorities are achievable
   or clearly marked as dependent on unresolved items.
8. Consistency: No unsupported optimism,
   contradictory statements, or invented commitments.
9. Readability: The report is concise,
   professional, and management-focused.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent status evidence, ownership,
delivery commitments, or approvals.
```

---

## 3. Practical IT Use Case

### Software Development — Weekly Integration and UAT Readiness

**Scenario:** A development team is implementing a customer self-service portal. The project is approaching UAT, but a delayed identity-provider certification and unresolved integration defects are affecting testing readiness.

The Project Manager must prepare a concise weekly report for delivery stakeholders and project leadership.

### Project Context

| Attribute | Details |
|---|---|
| Project | Customer Self-Service Portal |
| Phase | Integration Testing |
| Delivery approach | Hybrid |
| Reporting period | 7–11 June 2027 |
| Target milestone | UAT Preparation |
| Overall status | Amber |
| Main concern | Identity integration and critical defects |
| Management objective | Protect UAT readiness and clarify recovery decisions |

### Example Input

```text
Project: Customer Self-Service Portal

Reporting period: 7–11 June 2027
Delivery approach: Hybrid
Current phase: Integration Testing
Reported RAG: Amber

Weekly notes:
- Frontend development reached 90%.
- Identity-provider certification is
  10 working days behind plan.
- Mock authentication service is operational.
- Two critical integration defects were open.
- One critical defect has been fixed and retested.
- Six of eight UAT testers have been confirmed.
- Security evidence package is 70% complete.
- Vendor recovery plan received.
- Revised certification target: 18 June.
- Budget currently reported as on plan.

Next-week priorities:
- Complete identity certification.
- Resolve remaining critical defect.
- Confirm UAT resources.
- Complete security evidence.

Decision required:
Sponsor to consider two temporary vendor developers.

Decision deadline:
18 June 2027.

Previous-week RAG:
Not provided.
```

### Example Output — Weekly Project Status Report

#### 1. Project Status Summary

| Indicator | Assessment |
|---|---|
| Overall RAG | Amber |
| Previous RAG | Not provided |
| Trend | Cannot be assessed |
| Primary concern | Identity certification delay and UAT readiness |

**Executive Summary**

The Customer Self-Service Portal remains Amber due to a ten-working-day delay in identity-provider certification and one unresolved critical integration defect. Frontend development has reached 90%, and the operational mock authentication service allows eligible testing to continue. Six of eight UAT testers are confirmed, while security evidence remains incomplete. Management attention is required to validate vendor recovery and determine whether temporary development capacity is justified.

#### 2. This Week's Progress

| Workstream | Achievement | Management Significance |
|---|---|---|
| Frontend | 90% complete | Remaining development work requires confirmation |
| Integration | Mock authentication operational | Eligible testing can continue |
| Quality | One critical defect fixed and retested | One critical defect remains |
| Business Readiness | 6 of 8 testers confirmed | UAT capacity not fully secured |
| Security | Evidence package 70% complete | Final readiness remains outstanding |
| Vendor | Recovery plan received | Revised certification target is 18 June |

#### 3. Key Risks, Issues, and Dependencies

| Type | Description | Project Impact | Required Action | Proposed Owner |
|---|---|---|---|---|
| Issue | Identity certification 10 days late | Integration and UAT readiness | Validate recovery plan | Vendor Lead |
| Issue | One critical defect remains open | Testing readiness | Fix and retest | Development / QA Leads |
| Risk | Remaining UAT resources may not be confirmed | UAT start could be affected | Confirm two additional testers | Business Owner |
| Dependency | Security evidence incomplete | Approval readiness uncertain | Complete required documentation | Security Lead |

Action owners require confirmation.

#### 4. Next Week's Priorities

| Priority | Expected Outcome | Proposed Owner | Target Date |
|---|---|---|---|
| High | Complete identity certification | Vendor Lead | 18 June |
| High | Resolve and retest critical defect | Development / QA Leads | TBD |
| High | Confirm all UAT testers | Business Owner | TBD |
| High | Complete security evidence package | Security Lead | TBD |

The revised identity certification date is a target, not evidence that the milestone will be achieved.

#### 5. Decisions and Actions Required

| Type | Decision / Action | Required From | Deadline | Impact if Delayed |
|---|---|---|---|---|
| Decision | Assess additional vendor developer capacity | Project Sponsor | 18 June | Recovery options may narrow |
| Action | Confirm vendor certification forecast | Vendor Lead | 18 June | UAT planning uncertainty |
| Action | Confirm remaining UAT testers | Business Owner | TBD | Business testing readiness |
| Action | Validate critical defect closure forecast | Development Lead | TBD | Test schedule exposure |

**Management recommendation:** Confirm the vendor recovery forecast and remaining technical effort before approving additional capacity.

### Management Decisions

1. **Vendor recovery:** Validate the 18 June certification target against an actionable supplier plan.
2. **Quality:** Resolve the remaining critical integration defect before confirming UAT readiness.
3. **Business readiness:** Secure the two outstanding UAT testers.
4. **Resource decision:** Determine whether additional vendor developers would materially improve recovery feasibility.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The report clearly communicates Amber status, material progress, open issues, and management requirements. However, several proposed owners and deadlines are unconfirmed, and the recovery forecast lacks supporting evidence.

**Required corrections:**
- Validate vendor certification commitments.
- Confirm ownership and resolution dates for the critical defect.
- Obtain the remaining UAT resource commitments.
- Verify the reported budget position.
- Confirm sponsor decision authority and capacity assumptions.

**Approval blockers:** Unverified vendor recovery, incomplete action ownership, and missing milestone evidence.

**Governance:** This template supports PMI-aligned project monitoring, stakeholder communication, risk and issue management, and decision support.

The accountable Project Manager must validate project status, critical commitments, and management recommendations before formal distribution. Protect confidential customer, security, financial, vendor, and commercially sensitive information.
