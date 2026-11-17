# Project Performance Dashboard Commentary

## Purpose

Use this prompt to convert project KPI data into concise, management-level dashboard commentary.

The objective is not to repeat the numbers.

The objective is to explain:

- what the metrics mean,
- why performance changed,
- what the project impact is,
- whether management action is required,
- and what the team will focus on next.

A useful dashboard should answer:

> What is the data telling us about project health?

---

## Best Used For

**Project phase:**  
Delivery / Testing / Deployment / Hypercare

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Programme Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Weekly / Monthly / Governance reporting cycle

---

# Prompt

```text id="dashboard-01"
ROLE

You are a senior IT Project Manager experienced in performance
management, executive reporting, financial analysis, delivery metrics,
risk management, and project governance.

TASK

Write professional dashboard commentary from the KPI data below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Reporting period:
[DATE / MONTH]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Overall RAG:
[IF KNOWN]

KPI DATA

Schedule:
[DATA]

Cost / Budget:
[DATA]

Delivery Progress:
[DATA]

Quality / Testing:
[DATA]

Risks:
[DATA]

Issues:
[DATA]

Vendors:
[DATA]

Security / Compliance:
[DATA]

Business / Operational Readiness:
[DATA]

Flow Metrics:
[IF RELEVANT]

OUTPUT FORMAT

Write concise management commentary covering:

1. Schedule / Delivery Performance
2. Cost / Budget Performance
3. Quality / Risk / Issue Position
4. Overall Project Health
5. Recommended Management Focus for the Next Period
```

---

# Commentary Principle

Do not write:

```text id="dashboard-weak"
Schedule performance is 82%.
Budget performance is 96%.
There are 5 risks.
```

Write:

```text id="dashboard-better"
Delivery remains behind the planned baseline, driven primarily by
late completion of the identity-integration dependency.

Cost performance remains broadly within forecast, but contingency
exposure is increasing because additional vendor capacity may be
required.

The primary management focus for the next period should therefore
be schedule recovery and closure of the remaining integration
dependency.
```

Numbers should lead to interpretation.

---

# 1. Schedule / Delivery Performance

Explain:

```text id="dashboard-schedule"
Current position
Variance from plan
Cause
Impact
Recovery action
Forecast
```

Example:

> Integration testing is approximately two weeks behind the original plan because identity-provider certification was received later than forecast. The current recovery plan protects the UAT start only if the remaining critical defects close within the next reporting period.

---

# Earned Value Metrics

Where EVM is actually used, explain the metrics in plain language.

Possible measures include:

```text id="evm-metrics"
Planned Value (PV)
Earned Value (EV)
Actual Cost (AC)
Schedule Performance Index (SPI)
Cost Performance Index (CPI)
Schedule Variance (SV)
Cost Variance (CV)
Estimate at Completion (EAC)
```

Do not assume EVM is appropriate for every IT project.

---

# EVM Interpretation

## Schedule Performance Index

```text id="spi"
SPI = EV / PV
```

General interpretation:

```text id="spi-interpretation"
SPI = 1.0
Progress is aligned with the planned value.

SPI < 1.0
Earned progress is behind planned progress.

SPI > 1.0
Earned progress is ahead of planned progress.
```

Example:

> An SPI of 0.88 indicates that earned progress is below the planned position for the reporting period. The variance is currently concentrated in the integration workstream.

Do not interpret SPI without explaining the underlying cause.

---

# Cost Performance Index

```text id="cpi"
CPI = EV / AC
```

General interpretation:

```text id="cpi-interpretation"
CPI = 1.0
Cost efficiency is aligned with earned value.

CPI < 1.0
Cost performance is less efficient than planned.

CPI > 1.0
Cost performance is more efficient than planned.
```

Example:

> A CPI of 0.96 indicates moderate cost inefficiency relative to earned progress. Current forecast pressure is driven by additional vendor effort rather than broad cost growth across the programme.

---

# Estimate at Completion

If EAC is available, explain:

- forecast versus approved budget,
- main driver,
- whether the forecast is stable,
- whether management intervention is required.

Example:

> Forecast at completion is currently €1.86M against an approved budget of €1.80M. The €60k pressure is mainly associated with additional migration support and remains under review.

---

# Do Not Overstate EVM

EVM outputs should not be interpreted mechanically.

Check:

```text id="evm-quality"
Is progress measurement reliable?

Is the baseline current?

Is earned value calculated consistently?

Are major scope changes reflected?

Does the metric accurately represent software delivery?
```

A precise index does not guarantee precise management insight.

---

# 2. Cost / Budget Performance

Where full EVM is not used, analyse:

```text id="dashboard-finance"
Approved Budget
Actual Spend
Committed Cost
Forecast at Completion
Variance
Contingency
Change Requests
```

Example:

> Actual expenditure remains within the approved monthly profile, although the forecast has increased because of the proposed six-week extension of vendor migration support.

---

# 3. Delivery / Progress Metrics

Possible metrics include:

```text id="dashboard-delivery"
Milestone completion
Release progress
Requirements completion
Configuration progress
Migration progress
Integration status
Deployment readiness
```

Always translate progress into project meaning.

### Weak

> Configuration is 90%.

### Better

> Core configuration is approximately 90% complete, with the remaining work concentrated in two high-complexity business processes required before UAT.

---

# 4. Quality / Testing Commentary

Possible indicators:

```text id="dashboard-quality"
Test execution
Pass rate
Defect count
Critical defects
Defect ageing
Defect escape rate
UAT readiness
Regression status
```

Example:

> SIT execution reached 82%, with a 93% pass rate. Two Severity 1 defects remain open; both must close before the planned UAT entry decision.

---

# Quality Trend

Do not look only at absolute defect counts.

Consider:

```text id="quality-trend"
New defects
Closed defects
Defect ageing
Severity trend
Reopen rate
Test coverage
```

Example:

> Total open defects declined this month, but ageing of the remaining critical defects increased, so the overall quality position remains Amber.

---

# 5. Risk and Issue Commentary

Summarise:

```text id="dashboard-risk"
Total active risks
High / Critical risks
New risks
Materialised risks
Open issues
Escalated issues
Overdue mitigation
```

Do not list every risk.

Explain where risk concentration exists.

Example:

> The risk profile remains concentrated in vendor integration and release readiness. Three High risks remain open, but exposure has reduced following confirmation of UAT resources.

---

# 6. Vendor Performance

Possible indicators:

```text id="dashboard-vendor"
Milestone adherence
Defect performance
Resource capacity
SLA performance
Response time
Forecast reliability
Commercial change
```

Example:

> Vendor milestone performance deteriorated during the reporting period, with two integration commitments delivered late. A formal recovery plan is now in place and will be reviewed weekly.

---

# 7. Security / Compliance

Possible measures:

```text id="dashboard-security"
Open findings
Critical vulnerabilities
Approval status
Evidence completion
Penetration-test status
Compliance actions
```

Example:

> Security readiness remains Amber. No Critical findings are open, but final production approval depends on closure of three Medium findings before 15 September.

---

# 8. Agile / Scrum Metrics

Potential evidence includes:

```text id="dashboard-agile"
Release progress
Sprint Goal achievement
Backlog health
Defect trends
Cross-team dependencies
Team capacity
```

Avoid using velocity as a simple productivity ranking.

Interpret the metric in delivery context.

---

# 9. Kanban / Flow Metrics

Where Kanban is used, consider:

```text id="dashboard-kanban"
Throughput
Cycle Time
Lead Time
WIP
Work Item Age
Blocked Time
SLE Performance
```

Example:

> Median cycle time increased from 8 to 11 days because work is accumulating in integration review. WIP in that stage is above the agreed limit, indicating a bottleneck that may affect release predictability.

---

# Flow Metrics Should Drive Questions

Ask:

```text id="flow-questions"
Where is work ageing?

Where is WIP accumulating?

Which workflow stage is limiting throughput?

Are blocked items increasing?

Is delivery predictability improving or deteriorating?
```

Do not report flow metrics without explaining what management should do with them.

---

# 10. Overall Project Health

Bring the metrics together.

Do not produce separate comments that contradict one another.

Use:

```text id="dashboard-health"
Overall status
Primary driver
Trend
Key exposure
Recovery confidence
Management focus
```

Example:

> Overall project health remains Amber. Financial performance is stable and quality is improving, but the schedule remains exposed to external identity certification and one unresolved critical integration defect. Management focus next month should remain on closing the dependency and protecting UAT readiness.

---

# Metric-to-Management Logic

Use this sequence:

```text id="metric-management"
Metric
↓
Trend
↓
Cause
↓
Project Impact
↓
Management Action
```

Example:

```text id="metric-example"
Metric:
Cycle time increased 35%.

Cause:
Integration-review queue increased.

Impact:
Release predictability deteriorating.

Action:
Reduce WIP and allocate additional review capacity.
```

---

# Example Input

```text id="dashboard-example-input"
Project:
CRM Replacement

Reporting Period:
August

Overall:
Amber

Schedule:
Implementation milestone 2 weeks behind baseline.

Budget:
Approved €1.8M.
Actual €1.1M.
Forecast €1.78M.

Testing:
SIT 78% complete.
Pass rate 92%.
2 Critical defects open.

Risks:
9 active.
3 High.
5 Medium.
1 Low.

Issues:
2 open.
One vendor integration issue requires escalation.

Vendor:
Migration vendor added one additional specialist.

Security:
Final assessment planned for 5 September.

Flow:
Integration-review cycle time increased from 7 to 10 days.
```

---

# Example Output

## Schedule / Delivery Performance

Delivery remains behind the baseline by approximately two weeks, driven primarily by the integration and migration workstreams. Integration-review cycle time has increased from seven to ten days, indicating a growing constraint in the current workflow. Recovery remains possible, but the available schedule margin is limited ahead of UAT.

## Cost Performance

Financial performance remains stable. Actual spend is €1.1M against the €1.8M approved budget, and the current forecast of €1.78M remains within the authorised envelope. Additional migration support is currently absorbed within the forecast.

## Quality and Risk

SIT is 78% complete with a 92% pass rate. Two Critical defects remain open and represent the main quality constraint before UAT. Three High risks remain active, with the largest exposure related to vendor integration and release readiness.

## Overall Health

Overall project status remains Amber. Budget performance is stable, but schedule and integration risks require continued management attention. The priority for the next reporting period should be closure of the Critical defects, reduction of the integration-review bottleneck, and confirmation of security readiness.

---

# Prompt 2 — Dashboard Commentary Quality Review

```text id="dashboard-review"
ROLE

You are a PMO Director reviewing project dashboard commentary.

TASK

Review the commentary below.

[PASTE COMMENTARY]

Check whether:

- metrics are interpreted correctly,
- causes are explained,
- trends are visible,
- management impact is clear,
- recommendations follow logically from the data,
- unsupported conclusions are present,
- contradictory statements exist,
- numbers are simply repeated without interpretation.

OUTPUT FORMAT

Finding
Evidence
Why It Matters
Recommended Improvement
Priority
```

---

# Prompt 3 — Metric Anomaly Review

```text id="dashboard-anomaly"
ROLE

You are a project performance analyst.

TASK

Review the KPI dataset below and identify metrics that appear
inconsistent, unusual, or potentially misleading.

[PASTE KPI DATA]

Do not assume an anomaly is an error.

OUTPUT FORMAT

Metric
Observed Issue
Possible Explanation
Validation Required
Management Relevance
```

This is useful before dashboard commentary is distributed.

---

# Senior-Level Commentary Rules

A strong commentary should answer:

```text id="dashboard-rules"
What changed?

Why did it change?

Why does it matter?

Is it improving or deteriorating?

What are we doing about it?

What should management focus on next?
```

---

# Avoid

```text id="dashboard-avoid"
Metric dumping

Unsupported optimism

Unsupported pessimism

False precision

Explaining every KPI

Reporting numbers without trends

Reporting trends without causes

Reporting problems without actions
```

---

# Quality Checklist

Before publishing dashboard commentary, confirm:

- [ ] Metrics are factually correct
- [ ] Trends are explained
- [ ] Causes are identified where evidence exists
- [ ] Project impact is clear
- [ ] RAG status aligns with evidence
- [ ] Financial commentary reconciles
- [ ] Quality trends are interpreted
- [ ] Risks and issues are not simply counted
- [ ] Vendor performance is interpreted where relevant
- [ ] Flow metrics are translated into management meaning
- [ ] Recommendations are explicit
- [ ] Unsupported conclusions are removed

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- performance measurement,
- forecasting,
- schedule and cost management,
- quality,
- risk,
- governance,
- stakeholder communication.

## PMBOK Relevance

This prompt supports:

- measurement,
- delivery,
- finance,
- risk,
- governance,
- stakeholders.

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

Validate:

- KPI calculations,
- financial values,
- schedule data,
- defect information,
- risk ratings,
- vendor metrics,
- management conclusions.

AI can explain data.

It cannot compensate for inaccurate or poorly defined project metrics.

---

# Confidentiality

Dashboard data may contain sensitive information.

Protect:

- financial data,
- security findings,
- customer information,
- vendor performance,
- contract information,
- personal performance data.

Use anonymised information where required.

---

# Prompt Metadata

```text id="dashboard-metadata"
Prompt ID: REPORT-004
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Finance / Delivery Lead / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT performance dashboard commentary framework |
