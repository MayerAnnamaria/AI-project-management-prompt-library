# Project Issues Log

**Prompt ID:** RISK-005 | **Category:** Risk & Issue Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Document, assess, resolve, and monitor active project issues to minimize delivery impact and support timely management decisions.

**Use case:** Record and manage critical defects, missed milestones, failed integrations, vendor delays, or materialized risks during software development, testing, deployment, and operational transition.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
issue and risk management, root cause analysis, stakeholder coordination,
recovery planning, and project governance.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target milestone: [MILESTONE / DATE]
Reporting date: [DATE]

Issue ID: [ID / NEW]
Related risk ID: [ID / NONE]
Original risk: [DESCRIPTION, IF APPLICABLE]
Risk rating: [RATING, IF APPLICABLE]
Issue description: [WHAT HAS OCCURRED]
Date raised: [DATE]
Known root cause: [DETAILS / UNKNOWN]
Current impact: [DETAILS]
Schedule impact: [DETAILS]
Cost impact: [DETAILS]
Scope impact: [DETAILS]
Quality / technical impact: [DETAILS]
Security / compliance impact: [DETAILS]
Operational / stakeholder impact: [DETAILS]

Current containment: [ACTIONS]
Existing resolution actions: [LIST]
Known dependencies: [LIST]
Issue owner: [ROLE / UNKNOWN]
Action owners: [ROLES / UNKNOWN]
Target resolution date: [DATE / UNKNOWN]
Current status: [OPEN / IN PROGRESS / BLOCKED / RESOLVED]
Decisions or escalations: [DETAILS]

TASK

Create a formal issue record, resolution plan, and management update.

STEP 1 — ISSUE IDENTIFICATION AND ASSESSMENT

1. Confirm that the problem has occurred; distinguish issues
   from uncertain future risks.
2. Link the issue to a materialized risk where applicable,
   and recommend updating the risk register.
3. Write a factual issue statement describing the event,
   its significance, and current project impact.
4. Classify the issue by category and priority using the
   available organizational criteria.
5. Assess actual and potential impacts on schedule, cost,
   scope, quality, security, compliance, operations,
   stakeholders, and business value.
6. Distinguish symptoms, immediate causes, underlying causes,
   and systemic causes where supported by evidence.

STEP 2 — RESOLUTION AND ESCALATION

7. Separate immediate containment from permanent resolution.
8. Define specific actions, expected results, accountable owners,
   target dates, and progress status.
9. Identify dependencies and constraints affecting resolution.
10. Assess whether the issue threatens critical milestones,
    exceeds project tolerances, or requires external authority.
11. Identify escalation triggers, recipients, required decisions,
    decision owners, and deadlines.
12. Define measurable closure criteria and required evidence.

STEP 3 — MONITORING AND MANAGEMENT REPORTING

13. Track issue age, overdue actions, and target resolution dates.
14. Review changes in impact, recovery feasibility, and new risks.
15. Identify technical debt or residual impacts created by workarounds.
16. Prepare a concise 3–4 sentence management status update.
17. Define the next review and conditions for formal closure.
18. Recommend corrective and preventive actions where appropriate.

Do not invent causes, impacts, owners, dates, or approvals.
Distinguish confirmed facts from hypotheses and forecasts.
Keep unresolved issues visible until formally closed or transferred.
Adapt issue handling to the delivery approach without duplicating
team-level defect or incident management unnecessarily.

OUTPUT FORMAT

1. FORMAL ISSUE RECORD

Field | Value

Include:
Issue ID
Related Risk ID
Date Raised
Issue Category
Issue Description
Root Cause / Investigation Status
Current Impact
Schedule Impact
Cost Impact
Scope Impact
Quality / Technical Impact
Security / Compliance / Operational Impact
Priority
Immediate Containment
Permanent Resolution
Issue Owner
Action Owners
Target Resolution Date
Escalation Required
Decision Required
Decision Owner
Current Status
Issue Age / Days Overdue
Closure Criteria

2. ISSUE RESOLUTION PLAN

Action | Type (Containment / Resolution / Prevention) |
Purpose | Owner | Due Date | Status | Dependency

3. ESCALATION AND DECISION REVIEW

Trigger | Business / Delivery Impact | Escalation Recipient |
Decision Required | Decision Owner | Deadline

4. ISSUE MONITORING

Metric / Indicator | Current Status | Trend |
Required Action | Next Review

5. MANAGEMENT STATUS UPDATE

Write 3–4 sentences covering:
- What occurred
- Current delivery impact
- Resolution progress
- Escalation or decision required
- Next update or milestone

6. CLOSURE CRITERIA

Criterion | Required Evidence | Validation Owner | Status

7. MANAGEMENT SUMMARY

- Priority and current issue health
- Most significant project impacts
- Critical actions and overdue dependencies
- Decisions and escalations required
- Recommended next steps

Use concise Markdown tables.
Mark missing information as "Not yet defined".
Label proposed actions, ownership, and dates as unconfirmed.
```

---

## 2. Quality Check

Apply this control after generating the issue record and resolution analysis.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Project Issue Log.

Verify:

1. Validity: The issue describes an actual event, not merely
   a potential future risk.
2. Completeness: Required issue fields, resolution actions,
   monitoring, escalation, and closure criteria are addressed.
3. Accuracy: Confirmed facts, root cause hypotheses, impacts,
   and forecasts are clearly distinguished.
4. Priority: Issue severity and urgency reflect supported
   project impacts and organizational criteria.
5. Actionability: Containment and permanent resolution are
   separate, specific, and assigned to appropriate owners.
6. Governance: Escalation triggers, decisions, authority,
   and related risk updates are addressed.
7. Closure: Measurable completion criteria and evidence
   requirements prevent premature issue closure.
8. Reporting: Management updates are factual, concise,
   decision-oriented, and consistent with the issue record.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Escalation / Closure Blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent root causes, deadlines, ownership, or approvals.
Flag items requiring technical or stakeholder validation.
```

---

## 3. Practical IT Use Case

### Software Development — Critical Defect During Release Testing

**Scenario:** During regression testing, QA identifies a critical defect in a web application's reporting functionality. Users cannot export reports to Excel, a capability required for the upcoming release.

The Project Manager must document the issue, coordinate resolution, assess its impact on the release date, and communicate the required management decisions.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Testing / Release Preparation |
| Delivery approach | Scrum |
| Target release | 30 June 2027 |
| Reporting date | 22 June 2027 |
| Related risk | R-07 — Critical defects may delay release readiness |
| Current issue | Excel export fails during regression testing |
| Team | Project Manager, Product Owner, Developers, QA Lead |
| Management decision | Confirm defect resolution and release readiness before go-live |

### Example Input

```text
Project: Web Application Reporting Enhancement

Project phase: Regression Testing
Delivery approach: Scrum
Reporting date: 22 June 2027
Target release: 30 June 2027

Related risk:
R-07 — Critical defects may delay release readiness.

What has occurred:
On 21 June, QA identified that the Excel export function
fails when generating reports containing more than 5,000 rows.

Known impact:
- Excel export is a required release capability.
- Business users cannot export larger reports.
- Regression testing cannot be completed for this function.
- Release readiness approval requires resolution
  or an authorized exception.

Known technical information:
- The export function fails during file generation.
- The underlying technical cause is not yet confirmed.
- Other reporting functions are operating as expected.

Current containment:
- QA has documented reproduction steps.
- Developers are investigating the defect.
- Other eligible regression tests continue.

Current status: Open
Issue owner: Project Manager
Action owners: Development Lead / QA Lead
Target resolution date: Not yet defined

Escalation:
Required if the defect cannot be resolved and retested
before the release readiness decision.
```

### Example Output — Project Issue Log

#### 1. Formal Issue Record

| Field | Value |
|---|---|
| Issue ID | I-01 (illustrative) |
| Related Risk ID | R-07 |
| Date Raised | 21 June 2027 |
| Category | Quality / Technical / Testing |
| Issue Description | Excel export fails for reports exceeding 5,000 rows |
| Root Cause | Under investigation |
| Current Impact | Required reporting capability unavailable for affected reports |
| Schedule Impact | Release readiness potentially delayed |
| Cost Impact | Not yet assessed |
| Scope Impact | No confirmed scope change |
| Quality / Technical Impact | Regression acceptance cannot complete |
| Security / Compliance Impact | No impact identified; assessment incomplete |
| Priority | High (proposed; release-blocking) |
| Immediate Containment | Continue unaffected testing and preserve defect evidence |
| Permanent Resolution | Correct defect and complete regression verification |
| Issue Owner | Project Manager |
| Action Owners | Development Lead / QA Lead |
| Target Resolution | Not yet defined |
| Escalation Required | Conditional — if release readiness is threatened |
| Decision Required | Determine release readiness or formally approve a revised plan |
| Decision Owner | Authorized release approver — TBD |
| Status | Open |
| Issue Age | 1 calendar day as of 22 June |
| Days Overdue | Not assessable; no resolution deadline established |
| Closure Criteria | Fix verified, acceptance criteria met, evidence recorded |

The original risk should be reviewed and linked to the materialized issue according to the organization's risk-management process.

#### 2. Issue Resolution Plan

| Action | Type | Purpose | Proposed Owner | Due Date | Status |
|---|---|---|---|---|---|
| Investigate export failure | Resolution | Identify technical cause | Development Lead | TBD | In progress |
| Preserve reproduction evidence | Containment | Support diagnosis and retesting | QA Lead | TBD | In progress |
| Continue unaffected regression tests | Containment | Minimize testing delays | QA Lead | Ongoing | In progress |
| Implement approved defect correction | Resolution | Restore required functionality | Development Lead | TBD | Pending |
| Retest export scenarios | Resolution | Confirm fix and prevent regression | QA Lead | TBD | Pending |
| Review regression coverage | Prevention | Assess need for additional large-dataset tests | QA Lead | TBD | Proposed |

#### 3. Escalation and Decision Review

| Trigger | Delivery Impact | Escalation Recipient | Decision Required | Decision Owner | Deadline |
|---|---|---|---|---|---|
| Fix unavailable before readiness review | Release may be blocked | Project Manager / Product Owner | Confirm recovery approach | Authorized release approver | TBD |
| Critical defect remains unresolved | Quality acceptance not met | Release governance authority | Approve delay or evaluate permitted alternatives | TBD | Before release decision |
| Additional capacity required | Cost or resource impact | Project Sponsor | Approve resource change | TBD | As required |

**Escalation recommendation:** Confirm the release readiness decision date and defect-resolution forecast immediately. Any exception must follow authorized risk acceptance and release governance procedures.

#### 4. Issue Monitoring

| Indicator | Current Status | Trend | Required Action | Next Review |
|---|---|---|---|---|
| Issue priority | High (proposed) | Newly identified | Confirm classification | Next defect triage |
| Root cause | Unknown | Investigation ongoing | Complete diagnosis | Next technical update |
| Resolution forecast | Not established | Unknown | Agree target date | Next project review |
| Testing impact | Export testing blocked | Open | Validate fix and retest | After correction |
| Release impact | At risk | Uncertain | Assess readiness | Before release approval |

#### 5. Management Status Update

A critical defect was identified during regression testing on 21 June, preventing Excel exports for reports exceeding 5,000 rows. The defect affects a required release capability and may threaten the planned 30 June production deployment. Development is investigating the cause while QA continues unaffected regression testing; a confirmed resolution forecast remains outstanding. Release readiness will be reassessed once the fix and test evidence are available, with escalation required if the issue remains unresolved before the approval decision.

#### 6. Closure Criteria

| Criterion | Required Evidence | Proposed Validation Owner | Status |
|---|---|---|---|
| Root cause understood | Technical investigation record | Development Lead | Pending |
| Export defect resolved | Successful execution of agreed test cases | QA Lead | Pending |
| Regression impact assessed | Completed relevant regression tests | QA Lead | Pending |
| Release impact addressed | Documented readiness decision | Authorized approver | Pending |
| Related risk updated | Linked risk / issue register records | Project Manager | Pending |
| Issue closure approved | Verified resolution evidence | Issue Owner / designated approver | Pending |

The issue must remain open until the defined closure criteria are met and authorized stakeholders accept the resolution.

### Management Decisions

1. **Technical resolution:** Confirm the root cause, corrective approach, and realistic resolution date.
2. **Testing priorities:** Ensure the defect is fixed and retested without compromising mandatory regression coverage.
3. **Release readiness:** Determine whether the planned release remains feasible based on verified quality evidence.
4. **Governance:** Confirm escalation thresholds, approval authority, and whether a revised release plan is necessary.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The issue is documented with a clear impact, initial containment, and proposed resolution actions. However, its underlying cause, resolution forecast, escalation deadline, and release decision authority remain unconfirmed.

**Required corrections:**
- Complete root cause investigation.
- Confirm accountable action owners and resolution dates.
- Establish the release readiness decision deadline.
- Validate defect priority and escalation requirements.
- Obtain test evidence and formal closure authorization.

**Escalation / Closure Blockers:** Unresolved release-critical defect, missing resolution forecast, and unconfirmed release approval authority.

**Governance:** This prompt supports PMI-aligned practices in issue management, risk monitoring, problem resolution, stakeholder communication, escalation, and project governance.

A project issue is an active problem, not a future uncertainty. AI-generated issue records support analysis and reporting but do not replace technical investigation, authorized risk acceptance, or formal issue closure. Protect confidential customer, employee, vendor, financial, and security-sensitive information.
