# Monthly Project Progress Report

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** REPORT-002 | **Category:** Reporting & Communication

---


## 1. Ready-to-Use Prompt

**Purpose:** Convert project performance data into a concise, evidence-based monthly report that supports executive oversight, delivery forecasting, and timely management decisions.

**Use case:** Prepare monthly reports for IT project sponsors, PMOs, and steering committees when management needs visibility into milestones, costs, quality, risks, dependencies, and upcoming decisions.

Copy the prompt and replace the placeholders with your project information.

```text id="monthlyreport02"
ROLE

You are a Senior IT Project Manager specializing in software
delivery, executive reporting, financial oversight, risk
management, delivery forecasting, and project governance.

CONTEXT

Project: [PROJECT NAME]
Reporting period: [MONTH / DATE RANGE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target completion: [DATE]
Approved baseline: [IF AVAILABLE]
Previous monthly report: [PASTE / NOT AVAILABLE]
Reported overall RAG: [GREEN / AMBER / RED / UNKNOWN]

PROJECT PERFORMANCE DATA

Achievements and progress: [DETAILS]
Milestones and forecasts: [DETAILS]
Schedule variances: [DETAILS]
Scope and approved changes: [DETAILS]
Approved budget: [AMOUNT]
Actual and committed costs: [AMOUNTS]
Forecast at completion: [AMOUNT]
Contingency and pending changes: [DETAILS]
Quality and testing: [METRICS / FINDINGS]
Security and compliance: [STATUS]
Business and operational readiness: [STATUS]
Resources: [STATUS]
Vendors and external dependencies: [DETAILS]
Risks and issues: [REGISTER EXCERPTS]
Decisions and actions: [LIST]
Next-period priorities: [LIST]
Delivery forecast: [DETAILS]

TASK

Create a professional Monthly Project Progress Report.

1. Summarize overall delivery health, key achievements,
   material concerns, financial position, and decisions required.
2. Assess overall and individual RAG status using
   available evidence and approved thresholds.
3. Compare baseline milestones with current forecasts;
   explain variances, causes, impacts, and recovery actions.
4. Summarize meaningful workstream achievements,
   blockers, and next priorities without listing every task.
5. Analyze budget, actual spend, commitments, forecast
   at completion, contingency, and approved changes.
6. Evaluate quality, testing, security, and business
   or operational readiness using relevant evidence.
7. Highlight material risks and issues, their trends,
   ownership, mitigation, and resolution actions.
8. Assess vendor commitments and critical dependencies.
9. Identify decisions, actions, escalations, responsible
   authorities, deadlines, and consequences of delay.
10. Forecast next-period milestones, priorities, risks,
    and management requirements.
11. Compare current and previous reporting periods
    where historical data is available.
12. Identify contradictory data, missing evidence,
    and assumptions requiring validation.

Adapt reporting to the delivery approach:
- Agile / Scrum: Release goals, increments, backlog readiness,
  delivery trends, quality, and cross-team dependencies.
- Kanban: Throughput, cycle time, WIP, ageing work,
  blocked items, and service expectations.
- Predictive: Baseline variance, critical path,
  milestone forecasts, and approved changes.
- Hybrid: Combine delivery metrics with governance commitments.

Do not use velocity or similar metrics without context.
Translate metrics into business and delivery implications.

Do not invent progress percentages, financial values,
milestone dates, recovery actions, or approvals.
Do not automatically repeat last month's RAG status.
Flag inconsistencies between reported status and evidence.

OUTPUT FORMAT

1. EXECUTIVE SUMMARY

Write 3–5 sentences covering:
- Overall project health
- Major achievement
- Principal risk or issue
- Schedule and financial outlook
- Management decision required

2. OVERALL PROJECT HEALTH

Area | RAG Status | Current Position |
Trend | Management Concern

Include relevant areas:
Overall, Schedule, Budget, Scope, Quality,
Risk, Resources, Vendor, Security, Business Readiness.

Trend: Improving / Stable / Deteriorating / Unknown.

3. MILESTONE PERFORMANCE

Milestone | Baseline Date | Current Forecast |
Variance | Status | Recovery / Commentary

4. DELIVERY / WORKSTREAM PROGRESS

Workstream | Status | Key Achievement |
Current Blocker | Next Priority

5. FINANCIAL SUMMARY

Financial Measure | Budget / Baseline |
Actual / Forecast | Variance | Commentary

6. QUALITY AND READINESS

Area | Status | Supporting Evidence |
Concern | Required Action

7. KEY RISKS AND ISSUES

Type | Description | Impact | Rating / Priority |
Trend | Action | Owner

8. VENDOR AND EXTERNAL DEPENDENCIES

Vendor / Dependency | Commitment | Current Status |
Delivery Impact | Required Action

9. DECISIONS AND ACTIONS REQUIRED

Type | Decision / Action | Recommended Response |
Decision Owner | Deadline | Impact if Delayed

Type: Decision / Action / Escalation.

10. NEXT-PERIOD FORECAST

Expected Milestone / Priority | Forecast |
Critical Dependency | Confidence |
Management Attention Required

11. MONTH-ON-MONTH CHANGES
    (ONLY IF PREVIOUS REPORT PROVIDED)

Area | Previous Position | Current Position |
Trend | Management Significance

MANAGEMENT SUMMARY

- Current project health and supporting evidence
- Major deviations from plan
- Financial and delivery exposure
- Critical decisions and escalation
- Next-month management priorities

Use concise Markdown tables.
Mark unavailable information as "Not provided".
Distinguish approved commitments from forecasts.
```

---

## 2. Quality Check

Apply this independent review before issuing the monthly report.

```text id="monthlyqa02"
QUALITY CHECK

Act as a Senior PMO Director reviewing an executive
Monthly Project Progress Report.

Verify:

1. Accuracy: All facts, dates, calculations, and
   performance metrics match the supplied project data.
2. RAG Assessment: Status is supported by evidence
   and consistent with the organization's thresholds.
3. Milestones: Variances, recovery plans, and forecast
   changes are explained.
4. Financials: Budget, actuals, commitments, forecasts,
   and variances reconcile where sufficient data exists.
5. Delivery: Progress is outcome-focused rather
   than an excessive task-level summary.
6. Risks and Issues: Material concerns have clear
   owners, impact, trend, and response actions.
7. Decisions: Management requests, authority,
   deadlines, and consequences are explicit.
8. Forecast: Next-period outlook is realistic,
   forward-looking, and supported by evidence.
9. Consistency: No contradictions, unsupported assumptions,
   or unexplained month-on-month changes.
10. Executive Readability: The report is concise,
    actionable, and suitable for governance review.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Identify unsupported conclusions, weak forecasts,
missing decisions, and unreconciled financial values.

Do not invent project evidence or authorize management decisions.
```

---

## 3. Practical IT Use Case

### E-commerce System Enhancement — Monthly Delivery Review

**Scenario:** An IT team is enhancing an e-commerce order management system. Development is progressing, but integration defects and a delayed payment gateway dependency are creating pressure on testing and release readiness.

The Project Manager must prepare a monthly report for the Project Sponsor, explaining current performance, emerging delivery risks, and required management actions.

### Project Context

| Attribute | Details |
|---|---|
| Project | E-commerce Order Management Enhancement |
| Reporting period | August 2027 |
| Project phase | Integration / Testing |
| Delivery approach | Hybrid |
| Target release | 30 September 2027 |
| Approved budget | €450,000 |
| Current overall status | Amber |
| Key concern | Integration defects and payment gateway readiness |
| Audience | Project Sponsor / Steering Committee |
| Management decision | Validate recovery options and protect the release timeline |

### Example Input

```text id="monthlyexample02"
Project: E-commerce Order Management Enhancement

Reporting period: August 2027
Delivery approach: Hybrid
Target release: 30 September 2027

Reported overall status: Amber

Delivery progress:
- Order workflow development completed.
- Payment gateway integration 80% complete.
- System Integration Testing 70% complete.
- Two critical defects remain open.

Milestones:
- Development completion: 31 July — completed.
- SIT completion: 31 August — forecast 7 September.
- UAT completion: 17 September — forecast TBD.
- Production release: 30 September — unchanged target.

Budget:
- Approved budget: €450,000
- Actual spend: €310,000
- Committed additional cost: €80,000
- Forecast at completion: €445,000

Quality:
- SIT execution: 70%
- Critical defects: 2 open

External dependency:
- Payment provider integration support delayed.
- Revised supplier delivery date not confirmed.

Main risk:
Integration defects may delay UAT and release readiness.

Decision required:
Confirm whether additional technical support
should be requested from the payment provider.

Next-month priorities:
- Complete SIT
- Resolve critical defects
- Conduct UAT
- Confirm release readiness

Previous monthly report:
Not available.
```

### Example Output — Monthly Project Progress Report

#### 1. Executive Summary

The E-commerce Order Management Enhancement project is **Amber** for August 2027 due to integration defects and unresolved payment-provider dependencies. Core order workflow development is complete, but SIT completion is forecast seven calendar days later than the original milestone. The forecast project cost of €445,000 remains €5,000 below the approved €450,000 budget, although the underlying cost assumptions require confirmation. Management attention is required to obtain a reliable supplier recovery date and assess whether additional technical support is needed to protect the September release.

#### 2. Overall Project Health

| Area | RAG | Current Position | Trend |
|---|---|---|---|
| Overall | Amber | Integration and testing delays | Not assessed |
| Schedule | Amber | SIT forecast seven days late | Not assessed |
| Budget | Green (provisional) | Forecast €5,000 below budget | Not assessed |
| Scope | Green (provisional) | No scope changes reported | Not assessed |
| Quality | Amber | Two critical defects remain | Not assessed |
| Risk | Amber | Payment dependency threatens UAT | Not assessed |
| Vendor | Amber | Revised supplier commitment missing | Not assessed |
| Business Readiness | Not assessed | UAT forecast unavailable | Unknown |

RAG classifications are illustrative and require validation against approved thresholds. Trends cannot be established without previous-period data.

#### 3. Milestone Performance

| Milestone | Baseline | Forecast / Actual | Variance | Status |
|---|---|---|---|---|
| Development completion | 31 Jul | Completed | Not reported | Complete |
| SIT completion | 31 Aug | 7 Sep | +7 calendar days | Delayed forecast |
| UAT completion | 17 Sep | TBD | Not assessable | At risk |
| Production release | 30 Sep | No revised forecast | Not assessable | At risk |

**Schedule concern:** The SIT delay reduces the available time for UAT, defect resolution, and release preparation.

#### 4. Delivery / Workstream Progress

| Workstream | Status | Key Achievement | Current Blocker | Next Priority |
|---|---|---|---|---|
| Order workflow | Complete | Development finished | None reported | Support testing |
| Payment integration | At risk | 80% reported complete | Vendor dependency | Complete integration |
| QA / SIT | At risk | 70% of tests executed | Two critical defects | Resolve and retest |
| UAT | At risk | Planned milestone established | SIT dependency | Confirm readiness |

#### 5. Financial Summary

| Measure | Budget / Baseline | Actual / Forecast | Variance |
|---|---:|---:|---:|
| Approved project budget | €450,000 | — | — |
| Actual spend | — | €310,000 | — |
| Additional committed cost | — | €80,000 | — |
| Forecast at completion | €450,000 | €445,000 | €5,000 below budget |

Actual spend and additional commitments total €390,000, leaving €55,000 between that amount and the stated forecast at completion.

**Financial review required:** Confirm whether the forecast includes all remaining committed and expected costs, especially any additional payment-provider support.

#### 6. Quality and Readiness

| Area | Status | Evidence | Required Action |
|---|---|---|---|
| SIT execution | In progress | 70% completed | Finish remaining tests |
| Critical defects | At risk | Two open | Resolve and retest |
| UAT readiness | Not confirmed | SIT incomplete | Validate entry criteria |
| Release readiness | At risk | Downstream milestones exposed | Confirm go/no-go evidence |
| Security | Not provided | No assessment supplied | Confirm required clearance |

#### 7. Key Risks and Issues

| Type | Description | Impact | Action | Proposed Owner |
|---|---|---|---|---|
| Issue | Two critical integration defects remain open | SIT completion affected | Correct and retest | Development / QA Leads |
| Issue | Payment-provider support is delayed | Integration coordination affected | Obtain recovery commitment | Vendor Lead |
| Risk | UAT may be delayed | Release schedule exposure | Reassess test sequence | Project Manager |
| Risk | September release may become unachievable | Business milestone at risk | Validate recovery forecast | Project Manager |

Existing delays are issues; uncertain downstream consequences are risks.

#### 8. Vendor and External Dependencies

| Dependency | Commitment | Current Status | Delivery Impact | Required Action |
|---|---|---|---|---|
| Payment gateway support | Support for integration completion | Delayed; revised date unknown | SIT and release exposure | Obtain dated recovery plan |
| Payment integration completion | Complete integration | 80% reported | Remaining test dependency | Validate outstanding work |

#### 9. Decisions and Actions Required

| Type | Decision / Action | Proposed Owner | Deadline | Impact if Delayed |
|---|---|---|---|---|
| Decision | Determine need for additional vendor support | Authorized Sponsor / PM | TBD | Recovery may be constrained |
| Action | Obtain confirmed supplier recovery date | Vendor Lead | TBD | Forecast remains unreliable |
| Action | Confirm critical defect resolution plan | Development Lead | TBD | SIT completion at risk |
| Decision | Revalidate UAT and release forecasts | Project Governance | Before release readiness | Late commitment change |

#### 10. Next-Period Forecast

| Priority | Forecast | Dependency | Confidence |
|---|---|---|---|
| SIT completion | 7 September | Defect resolution, provider support | Low |
| UAT completion | TBD | Successful SIT and business availability | Low |
| Release readiness | TBD | Quality and UAT evidence | Low |
| Production release | 30 September remains target | Recovery feasibility | Low |

The immediate management priority is to confirm whether the current recovery options can protect UAT and the planned production release.

#### 11. Month-on-Month Changes

**Not assessed.** The previous monthly report was not provided, so improvements, deterioration, and month-on-month financial changes cannot be verified.

### Management Decisions

1. **Vendor recovery:** Obtain a committed payment-provider recovery plan with named owners and dates.
2. **Testing:** Confirm critical defect resolution and reassess the SIT and UAT sequence.
3. **Financial control:** Validate the forecast at completion and the cost of any additional technical support.
4. **Release governance:** Decide whether the September release remains feasible using evidence from testing and supplier readiness.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The report identifies schedule exposure, quality concerns, key dependencies, and financial position. However, the UAT forecast, revised supplier commitment, financial forecast assumptions, and RAG thresholds require validation.

**Required corrections:**
- Confirm SIT recovery feasibility and the updated UAT forecast.
- Obtain dated vendor recovery commitments.
- Reconcile remaining costs with forecast at completion.
- Validate RAG classifications against approved thresholds.
- Confirm the release decision owner and deadlines.

**Approval blockers:** Unconfirmed downstream milestone forecasts, incomplete vendor recovery commitments, and unvalidated financial assumptions.

**Governance:** This framework supports PMI-aligned project performance reporting, financial oversight, forecasting, risk and issue management, stakeholder communication, and project governance.

The monthly report is a management decision-support artifact. All material performance figures, forecasts, status assessments, and recommendations require verification by the accountable Project Manager and relevant stakeholders. Protect confidential financial, contractual, security, customer, and vendor information.
