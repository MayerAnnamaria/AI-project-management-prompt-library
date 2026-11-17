# Monthly Project Progress Report

## Purpose

Use this prompt to create a structured monthly project report for management, sponsors, PMO, steering committees, or other governance stakeholders.

The monthly report should provide a more complete view than a weekly update.

It should explain:

- overall project health,
- progress against commitments,
- financial position,
- major risks and issues,
- quality and readiness,
- vendor performance,
- key decisions,
- and the forward outlook.

The objective is to support **governance and informed decision-making**, not simply document activity.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment / Hypercare

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / PMO / Programme Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Monthly

---

# Prompt

```text id="monthly-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, executive reporting, project governance,
financial management, risk management, quality assurance,
and stakeholder communication.

TASK

Create a professional monthly project progress report from the
project information below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Reporting period:
[MONTH / DATE RANGE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target completion / release:
[DATE]

Overall RAG status:
[IF KNOWN]

PROJECT DATA

Progress:
[DETAILS]

Milestones:
[DETAILS]

Schedule:
[DETAILS]

Budget:
[DETAILS]

Scope:
[DETAILS]

Quality / Testing:
[DETAILS]

Security / Compliance:
[DETAILS]

Operations / Business Readiness:
[DETAILS]

Vendors:
[DETAILS]

Risks:
[DETAILS]

Issues:
[DETAILS]

Decisions:
[DETAILS]

Key achievements:
[DETAILS]

Next-period priorities:
[DETAILS]

Forecast:
[DETAILS]

OUTPUT FORMAT

Create the report with:

1. Executive Summary
2. Overall Project Health
3. Progress Against Milestones
4. Delivery / Workstream Progress
5. Financial Summary
6. Quality, Testing and Readiness
7. Key Risks and Issues
8. Vendor / External Dependency Status
9. Decisions and Actions Required
10. Forecast for Next Period
```

---

# 1. Executive Summary

Write 3–5 concise sentences covering:

```text id="monthly-exec"
Overall position
Major achievement
Main risk or issue
Financial / schedule position
Decision or management action required
```

The executive summary should be understandable without reading the rest of the report.

---

# Example Executive Summary

```text id="monthly-exec-example"
The CRM replacement remains Amber due to a two-week delay in
data-migration preparation and unresolved vendor integration
dependencies.

Core configuration is substantially complete and system integration
testing has started as planned.

Budget remains within the approved forecast, although contingency
exposure has increased because of migration uncertainty.

Management attention is required on vendor recovery actions and
business-resource confirmation for UAT.
```

---

# 2. Overall Project Health

Provide a project-health summary.

| Area | Status | Current Position | Trend |
|---|---|---|---|
| Overall | Green / Amber / Red | | |
| Schedule | | | |
| Budget | | | |
| Scope | | | |
| Quality | | | |
| Risk | | | |
| Resources | | | |
| Vendor | | | |
| Security / Compliance | | | |
| Business Readiness | | | |

Trend:

```text id="monthly-trend"
Improving
Stable
Deteriorating
```

---

# RAG Assessment

RAG should be based on evidence.

Do not automatically copy the previous month's status.

Review:

```text id="monthly-rag"
Schedule performance
Budget performance
Scope stability
Quality
Risk exposure
Issue severity
Critical dependencies
Vendor performance
Release readiness
Business readiness
```

If reported RAG and available evidence conflict, flag the inconsistency.

---

# 3. Progress Against Milestones

Provide:

| Milestone | Baseline / Target | Current Forecast | Status | Commentary |
|---|---|---|---|---|

Use:

```text id="monthly-milestone-status"
Complete
On Track
At Risk
Delayed
Not Started
```

Where a milestone is delayed, explain:

- cause,
- impact,
- recovery action,
- revised forecast.

---

# 4. Delivery / Workstream Progress

Report by meaningful workstream.

Possible workstreams:

```text id="monthly-workstreams"
Requirements
Architecture
Development / Configuration
Integration
Data Migration
Testing
Security
Change Management
Training
Deployment
Operations
Vendor Delivery
```

Provide:

| Workstream | Current Status | Progress | Key Achievement | Next Priority |
|---|---|---|---|---|

Do not report every task.

Focus on material delivery information.

---

# Agile / Scrum Reporting

Where relevant, monthly reporting may include:

- release progress,
- major product increments,
- Sprint trends,
- backlog health,
- cross-team dependencies,
- major blockers.

Do not use velocity as an executive performance target without context.

Explain what the metric means for delivery.

---

# Kanban Reporting

Relevant indicators may include:

```text id="monthly-kanban"
Throughput trend
Cycle-time trend
Work item age
WIP
Blocked work
SLE performance
```

Example:

> Average cycle time increased from 8 to 12 days because integration review became a bottleneck. Three ageing items are now directly linked to the planned release scope.

Translate metrics into management impact.

---

# Predictive Reporting

May include:

- baseline milestone variance,
- critical-path impact,
- schedule forecast,
- approved change impact.

---

# Hybrid Reporting

Combine formal project commitments with delivery-level evidence.

Example:

```text id="monthly-hybrid"
Roadmap / delivery metrics
↓
Milestone forecast
↓
Risk / dependency assessment
↓
Governance impact
```

---

# 5. Financial Summary

Provide:

| Financial Measure | Baseline / Budget | Actual / Forecast | Variance | Status |
|---|---:|---:|---:|---|

Possible measures:

```text id="monthly-financial"
Approved budget
Actual spend
Committed cost
Forecast at completion
Contingency
Approved changes
Pending changes
```

If values are missing, state this rather than inventing them.

---

# Financial Commentary

Explain:

```text id="monthly-financial-commentary"
What changed this month?

What is driving variance?

Is contingency changing?

Are vendor costs changing?

Are scope decisions affecting forecast?

Does management action need to be taken?
```

---

# 6. Quality, Testing and Readiness

Use only the areas relevant to the project.

Possible indicators:

```text id="monthly-quality"
Test execution
Pass rate
Critical defects
Defect ageing
UAT readiness
Security approvals
Data migration quality
Operational readiness
Training readiness
Deployment readiness
```

Provide:

| Area | Status | Evidence | Concern / Action |
|---|---|---|---|

---

# Example

```text id="monthly-quality-example"
System Integration Testing:
78% executed
92% pass rate
2 critical defects open

Status:
Amber

Action:
Resolve and retest critical defects before UAT entry decision.
```

---

# 7. Key Risks and Issues

Report only risks and issues requiring management visibility.

| Type | Description | Impact | Rating / Priority | Action | Owner |
|---|---|---|---|---|---|

For each major item explain:

```text id="monthly-risk-rule"
Current exposure
Change since previous month
Mitigation / resolution
Decision required
```

---

# Risk Trend

Where useful:

```text id="monthly-risk-trend"
New
Increasing
Stable
Reducing
Closed
Materialised into Issue
```

---

# 8. Vendor / External Dependency Status

Where external suppliers are important, provide:

| Vendor / Dependency | Commitment | Current Status | Risk | Required Action |
|---|---|---|---|---|

Consider:

- milestone performance,
- delivery quality,
- capacity,
- commercial changes,
- dependencies,
- escalations.

---

# 9. Decisions and Actions Required

Provide:

| Decision / Action | Owner | Recommendation | Deadline | Impact if Delayed |
|---|---|---|---|---|

Separate:

```text id="monthly-decision-types"
Decision Required
Action Required
Escalation Required
```

Do not hide decisions inside general commentary.

---

# Example

```text id="monthly-decision-example"
Decision:
Approve additional data-migration capacity.

Owner:
Project Sponsor.

Recommendation:
Approve two temporary specialists for six weeks.

Deadline:
15 August.

Impact if delayed:
Current migration recovery plan will not protect the UAT start.
```

---

# 10. Forecast for Next Period

Include:

```text id="monthly-forecast"
Expected milestones
Key priorities
Emerging risks
Expected decisions
Forecast status
```

A useful forecast should answer:

> What is most likely to change before the next report?

---

# Forecast Confidence

Optionally classify forecast confidence:

```text id="monthly-confidence"
High
Medium
Low
```

Explain low confidence where significant dependencies remain unresolved.

---

# Example Input

```text id="monthly-example-input"
Project:
CRM Replacement

Reporting Period:
August 2027

Delivery Approach:
Hybrid

Overall:
Amber

Progress:
Core configuration complete.
Integration testing 75% complete.
Data migration rehearsal delayed by two weeks.

Schedule:
Go-live still forecast for 1 October but recovery margin is limited.

Budget:
€1.1M spent of €1.8M approved.
Forecast currently €1.78M.

Quality:
2 critical defects open.
SIT pass rate 91%.

Security:
Final review scheduled for 5 September.

Business Readiness:
UAT testers confirmed.
Training material 60% complete.

Vendor:
Migration vendor has added one specialist.

Main Risk:
Migration delay may compress UAT.

Decision:
Sponsor may need to approve additional migration capacity.
```

---

# Example Executive Output

## Executive Summary

The CRM replacement remains **Amber** because the delayed data-migration rehearsal has reduced schedule contingency ahead of UAT. Core configuration is complete and integration testing is approximately 75% complete, with two critical defects still under resolution. The project remains within the approved financial forecast. Additional migration capacity may be required if the current recovery actions do not restore the planned UAT start.

---

# Prompt 2 — Month-on-Month Trend Analysis

```text id="monthly-trend-prompt"
ROLE

You are a senior PMO Lead reviewing monthly project performance.

TASK

Compare the current and previous monthly project reports.

PREVIOUS REPORT

[PASTE]

CURRENT REPORT

[PASTE]

Identify:

1. Areas improving
2. Areas deteriorating
3. New risks / issues
4. Risks closed
5. Milestones moved
6. Budget changes
7. New decisions
8. Forecast changes

OUTPUT FORMAT

Area
Previous Position
Current Position
Trend
Management Significance
```

This prevents monthly reporting from becoming a sequence of disconnected snapshots.

---

# Prompt 3 — Executive Quality Review

```text id="monthly-review"
ROLE

You are a PMO Director performing a quality review of a monthly
IT project report.

TASK

Review the report below.

[PASTE REPORT]

Check for:

- unsupported RAG status,
- inconsistent financial figures,
- unexplained milestone changes,
- missing decisions,
- weak forecasts,
- risks without owners,
- issues without resolution actions,
- excessive operational detail,
- contradictions,
- unsupported assumptions.

OUTPUT FORMAT

Finding
Evidence
Why It Matters
Recommended Correction
Priority
```

---

# Reporting Principles

The monthly report should be:

```text id="monthly-principles"
Evidence-based
Decision-oriented
Concise
Forward-looking
Consistent
Traceable
Audience-appropriate
```

A strong monthly report explains not only:

> What happened?

but also:

> What does it mean, what happens next, and what management action is required?

---

# Quality Checklist

Before issuing the report, confirm:

- [ ] Executive summary reflects actual project health
- [ ] RAG status is evidence-based
- [ ] Milestone movement is explained
- [ ] Financial figures reconcile
- [ ] Quality / readiness is visible
- [ ] Material risks and issues are included
- [ ] Vendor dependencies are visible
- [ ] Decisions are explicit
- [ ] Decision deadlines are included
- [ ] Forecast is forward-looking
- [ ] Trend from previous period is understood
- [ ] No unsupported information was invented

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- performance monitoring,
- forecasting,
- stakeholder communication,
- financial management,
- risk and issue management,
- governance,
- decision support.

## PMBOK Relevance

This prompt supports:

- measurement,
- finance,
- delivery,
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

Before formal distribution, validate:

- RAG status,
- financial values,
- milestone forecast,
- risks and issues,
- security or compliance statements,
- decisions and recommendations.

The accountable Project Manager remains responsible for the official report.

---

# Confidentiality

Monthly reports may contain commercially or operationally sensitive information.

Protect:

- budget details,
- vendor performance,
- security issues,
- customer information,
- contractual matters,
- personal performance information,
- strategic decisions.

Use anonymised data in public AI tools where required.

---

# Prompt Metadata

```text id="monthly-metadata"
Prompt ID: REPORT-002
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Sponsor
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
| 1.0 | YYYY-MM-DD | Initial IT monthly progress-report framework |
