# Project Performance Dashboard Commentary

**Prompt ID:** REPORT-004 | **Category:** Reporting & Communication | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Transform project KPIs into concise, evidence-based commentary explaining performance trends, delivery implications, and required management actions.

**Use case:** Prepare commentary for weekly project dashboards, monthly performance reviews, or steering committee reports when management needs to understand what project metrics mean and where intervention is required.

Copy the prompt and replace the placeholders with your project information.

```text id="dash04prompt"
ROLE

You are a Senior IT Project Manager specializing in project
performance analysis, executive reporting, delivery metrics,
financial oversight, risk management, and governance.

CONTEXT

Project: [PROJECT NAME]
Reporting period: [DATE / MONTH]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Overall RAG status: [GREEN / AMBER / RED / UNKNOWN]
Approved targets / baselines: [DETAILS]
Previous-period metrics: [IF AVAILABLE]

KPI DATA

Schedule and milestones: [DATA]
Budget / actual / committed cost / forecast: [DATA]
Delivery progress: [DATA]
Quality and testing: [DATA]
Risks and issues: [DATA]
Vendor performance: [DATA]
Security / compliance: [DATA]
Business / operational readiness: [DATA]
Agile or flow metrics: [IF RELEVANT]

EVM data, if used:
Planned Value (PV): [VALUE]
Earned Value (EV): [VALUE]
Actual Cost (AC): [VALUE]
Estimate at Completion (EAC): [VALUE]

Known constraints and dependencies: [LIST]
Existing recovery actions: [LIST]
Management decisions required: [LIST]

TASK

Create management-level dashboard commentary.

1. Validate reported KPI values, baselines, time periods,
   definitions, and relevant calculations.
2. Identify material variances and changes from prior periods.
3. Explain schedule and delivery performance, including
   milestone exposure and relevant dependencies.
4. Interpret budget, actual spend, committed costs,
   forecasts, and contingency where information exists.
5. If valid EVM data is provided, calculate and interpret:
   SPI = EV / PV
   CPI = EV / AC
   SV = EV - PV
   CV = EV - AC
   Explain EAC only if its value or estimation method is provided.
6. Assess quality using test execution, pass rates,
   critical defects, ageing, and readiness indicators.
7. Identify significant risk and issue concentrations,
   trends, overdue actions, and escalation needs.
8. Evaluate vendor, security, compliance, and operational
   readiness where relevant.
9. Interpret Agile delivery signals or Kanban flow metrics
   in terms of delivery predictability, not individual productivity.
10. Assess overall RAG health and identify conflicting indicators.
11. Recommend specific management actions, responsible roles,
    and decisions needed for the next reporting period.
12. Flag unusual, inconsistent, or potentially misleading data
    and identify the validation required.

For each material KPI, apply:

METRIC → TREND → CAUSE → PROJECT IMPACT → MANAGEMENT ACTION

Separate observed results from inferred causes.
Do not invent KPI values, trends, baselines, or recovery forecasts.
Do not assume EVM is appropriate unless the project uses it.
Avoid repeating numbers without explaining their significance.

OUTPUT FORMAT

1. EXECUTIVE DASHBOARD COMMENTARY

Write 3–5 sentences covering overall performance,
the most important changes, main exposure, and next actions.

2. KPI PERFORMANCE ANALYSIS

Area | KPI / Current Value | Previous / Target |
Trend or Variance | Interpretation | Management Impact

Include relevant:
Schedule, Cost, Delivery, Quality, Risk,
Vendor, Security, and Business Readiness.

3. EVM ANALYSIS (IF APPLICABLE)

Metric | Formula | Result | Interpretation |
Management Implication

4. ANOMALY AND DATA QUALITY REVIEW

Metric | Observed Inconsistency |
Possible Explanation | Validation Required |
Management Significance

5. OVERALL PROJECT HEALTH

Area | RAG | Evidence | Trend |
Primary Concern | Recovery Confidence

6. NEXT-PERIOD MANAGEMENT FOCUS

Priority | Required Action | Proposed Owner |
Deadline | Expected Outcome | Decision Required

MANAGEMENT SUMMARY

- Main performance drivers
- Significant negative and positive trends
- Material forecast or risk exposure
- Actions requiring governance attention

Use concise Markdown tables and professional management language.
Mark unavailable metrics as "Not provided".
Label hypotheses and proposed actions explicitly.
```

---

## 2. Quality Check

Apply this independent review before distributing dashboard commentary.

```text id="dash04qa"
QUALITY CHECK

Act as a Senior PMO Director and Project Performance Analyst.

Review the dashboard commentary and supporting KPI data.

Verify:

1. Accuracy: KPI values, formulas, percentages, and
   financial figures are calculated and interpreted correctly.
2. Trends: Changes are supported by comparable reporting periods.
3. Causality: Observed trends are separated from unverified causes.
4. Materiality: Commentary focuses on meaningful project impact,
   not simply repeating metric values.
5. Consistency: RAG status agrees with schedule, cost,
   quality, risks, and readiness evidence.
6. Anomalies: Unusual or contradictory KPIs are identified
   without automatically treating them as errors.
7. EVM: Metrics are calculated only from valid,
   consistently defined source data.
8. Decisions: Recommendations are specific, realistic,
   and supported by available evidence.
9. Executive Value: Commentary is concise, forward-looking,
   and appropriate for project governance.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Data Validation Required: [INCONSISTENT / MISSING METRICS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent causes, metric definitions, forecasts,
or management approvals.
```

---

## 3. Practical IT Use Case

### Software Development — Testing Performance and Release Readiness

**Scenario:** A software development team is delivering new reporting functionality for an internal business application. Although development is progressing, integration-review cycle time has increased and several critical defects remain unresolved.

The Project Manager must interpret Jira and QA dashboard data and recommend management action before the planned release.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Integration Testing |
| Delivery approach | Scrum |
| Reporting period | June 2027 |
| Target release | 30 June 2027 |
| Data sources | Jira, test results, project budget report |
| Key concern | Increasing cycle time and unresolved critical defects |
| Audience | Project Sponsor / Delivery Management |
| Management decision | Prioritize testing bottlenecks and determine release feasibility |

### Example Input

```text id="dash04example"
Project: Web Application Reporting Enhancement

Reporting period: June 2027
Delivery approach: Scrum
Target release: 30 June 2027

Reported overall status: Amber

Schedule:
- Development milestone completed on time.
- SIT completion planned for 20 June.
- SIT completion forecast for 25 June.

Budget:
- Approved budget: €200,000
- Actual spend: €145,000
- Forecast at completion: €195,000

Delivery:
- 85% of planned release scope completed.
- Three integration items remain blocked.

Quality:
- SIT test execution: 82%
- Test pass rate: 91%
- Two Severity 1 defects remain open.
- Critical defect closure dates not confirmed.

Flow metrics:
- Median integration-review cycle time:
  Previous period: 5 days
  Current period: 8 days
- Integration-review WIP above agreed limit.

Risk:
- Release readiness at risk due to testing dependencies.

Vendor:
No external delivery dependency identified.

Security:
Final approval status not provided.

Existing recovery actions:
Development and QA jointly reviewing open defects.

Previous-period financial data:
Not available.
```

### Example Output — Dashboard Commentary

#### 1. Executive Dashboard Commentary

Overall project health remains **Amber** due to delayed integration testing and two unresolved Severity 1 defects. SIT completion is forecast five calendar days later than planned, while median integration-review cycle time has increased from five to eight days. Forecast cost remains within the approved budget, but release readiness cannot be confirmed without defect resolution, completed testing, and outstanding approval evidence. Management focus should be on removing integration bottlenecks and validating the 30 June release forecast.

#### 2. KPI Performance Analysis

| Area | KPI / Current Value | Target / Previous | Trend / Variance | Management Interpretation |
|---|---|---|---|---|
| Schedule | SIT forecast 25 Jun | Planned 20 Jun | +5 calendar days | Reduced time for release readiness |
| Budget | EAC €195,000 | Budget €200,000 | €5,000 below budget | Forecast within allocation |
| Delivery | 85% scope complete | Target not provided | Not assessable | Remaining work requires review |
| Quality | 82% SIT executed | Target not provided | Not assessable | Testing incomplete |
| Defects | 2 Severity 1 open | Release criteria not provided | Open exposure | Critical quality concern |
| Flow | Median cycle time 8 days | Previous 5 days | +60% | Reduced integration throughput predictability |
| Blockers | 3 integration items | Previous not provided | Not assessable | Delivery dependencies remain |
| Security | Approval status unknown | Required status not provided | Unknown | Readiness information gap |

**Management interpretation:** Integration review is a significant constraint because work is accumulating above the agreed WIP limit while cycle time has increased.

The reported flow metrics establish a trend, but they do not independently establish its root cause.

#### 3. EVM Analysis

**Not applicable.** The project input does not provide Planned Value, Earned Value, Actual Cost on an EVM-consistent basis, or an approved earned-value measurement method.

The available financial position is:

| Measure | Value |
|---|---:|
| Approved budget | €200,000 |
| Actual spend | €145,000 |
| Forecast at completion | €195,000 |
| Forecast variance | €5,000 below budget |

The remaining forecast expenditure is €50,000, assuming actual spend and forecast at completion use the same cost basis.

Financial performance trends cannot be established without previous-period data.

#### 4. Anomaly and Data Quality Review

| Metric | Observed Concern | Possible Explanation | Validation Required |
|---|---|---|---|
| Scope progress | 85% reported complete | Completion definition unknown | Confirm measurement method |
| Cycle time | Increased 60% | Potential integration-review bottleneck | Review queue and blocked-item history |
| Critical defects | Two open, no closure dates | Resolution forecast unavailable | Confirm fix and retest estimates |
| Security approval | No status supplied | Data gap | Obtain readiness status |
| Budget | EAC below budget despite delay | Remaining effort may already be included | Validate forecast assumptions |

No inconsistency is automatically treated as an error.

#### 5. Overall Project Health

| Area | RAG | Supporting Evidence | Trend | Management Concern |
|---|---|---|---|---|
| Overall | Amber | SIT delay and open critical defects | Unknown | Release readiness |
| Schedule | Amber | Five-day SIT forecast delay | Deteriorating against plan | Testing compression |
| Budget | Green (provisional) | EAC below approved budget | Unknown | Forecast completeness |
| Quality | Amber | Two Severity 1 defects remain | Unknown | Acceptance risk |
| Integration | Amber | Cycle time increased; WIP above limit | Deteriorating | Bottleneck |
| Security | Not assessed | Approval evidence unavailable | Unknown | Release approval |

**Recovery confidence:** Low until defect closure forecasts, remaining SIT effort, and release-readiness evidence are confirmed.

#### 6. Next-Period Management Focus

| Priority | Required Action | Proposed Owner | Deadline | Expected Outcome |
|---|---|---|---|---|
| High | Confirm Severity 1 resolution dates | Development Lead | TBD | Reliable defect recovery forecast |
| High | Prioritize ageing integration items | Development / QA Leads | TBD | Reduced blocked work |
| High | Validate remaining SIT scope | QA Lead | Before release review | Evidence-based completion forecast |
| High | Confirm security approval status | Security Lead | Before release approval | Complete readiness evidence |
| High | Reassess production release feasibility | Project Manager | Before go/no-go decision | Informed management decision |

### Management Decisions

1. **Integration performance:** Review work-item ageing and WIP policy to reduce the testing bottleneck.
2. **Quality:** Confirm critical defect resolution and retesting before release approval.
3. **Schedule:** Reforecast remaining SIT and release-readiness activities based on verified capacity.
4. **Governance:** Determine whether the planned 30 June release remains feasible or requires a controlled schedule change.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** Commentary accurately translates the supplied schedule, budget, quality, and flow metrics into management implications. However, the root cause of increasing cycle time, defect closure forecasts, and security readiness remain unverified.

**Required corrections:**
- Validate integration-review bottleneck causes.
- Confirm critical defect resolution dates.
- Reassess release feasibility using remaining test effort.
- Validate the financial forecast assumptions.
- Obtain security approval status.

**Approval blockers:** Unconfirmed release-critical defect resolution, incomplete readiness evidence, and unavailable recovery forecasts.

**Governance:** Supports PMI-aligned performance measurement, forecasting, schedule and cost oversight, quality management, risk monitoring, and governance.

Dashboard commentary supports project decisions but does not replace validated KPI definitions, authoritative source data, or formal management approval. Protect confidential financial, commercial, customer, and security-sensitive information.
