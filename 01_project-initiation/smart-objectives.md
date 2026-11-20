# SMART Project Objectives

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** INIT-005 | **Category:** Project Initiation

---


## 1. Ready-to-Use Prompt

**Purpose:** Translate strategic project goals into measurable, accountable objectives that align delivery performance with business value.

**Use case:** Define or revise success measures, KPI targets, and accountable ownership when initiating a project, establishing a delivery baseline, or reviewing major scope changes.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in software delivery,
business analysis, performance measurement, benefits realization,
and project governance.

CONTEXT

Project: [PROJECT NAME]
Business problem: [PROBLEM]
Strategic purpose: [BUSINESS OBJECTIVE]
Expected benefits: [BENEFITS]
Target completion: [DATE]
Budget: [BUDGET OR RANGE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Stakeholders: [ROLES]
Expected outcomes: [LIST]
Known success criteria and KPIs: [LIST]
Current performance baselines: [METRICS, IF AVAILABLE]
Dependencies: [LIST]
Constraints: [LIST]

TASK

Define five SMART project objectives aligned with business value.

1. Make each objective Specific, Measurable, Achievable,
   Relevant, and Time-bound.
2. Distinguish project outputs from business, operational,
   quality, and flow/delivery outcomes.
3. Link each objective to an expected business benefit.
4. Define measurable indicators, baselines, targets, and deadlines.
5. Assess target feasibility against budget, capacity, and constraints.
6. Identify accountable owners and unresolved ownership.
7. Highlight objectives dependent on unapproved scope or requirements.
8. Identify critical vendor, technical, and stakeholder dependencies.
9. Assess risks that could prevent objective achievement.
10. Flag conflicting objectives, unsupported targets, and missing data.
11. Replace vague goals with measurable statements where evidence allows.
12. Identify objectives requiring stakeholder approval.

Do not invent targets, baselines, dates, or ownership.
Use "Target to be confirmed" where evidence is insufficient.
Clearly distinguish proposed measures from approved commitments.

OUTPUT FORMAT

TABLE 1 — SMART OBJECTIVES

ID | Objective | Specific Outcome | KPI / Measurement |
Baseline | Target | Target Date | Accountable Owner |
Business Benefit | Primary Dependency | Key Risk | Objective Type

Classify each objective as:
- Project Output
- Business Outcome
- Operational Outcome
- Quality Outcome
- Flow / Delivery Outcome

TABLE 2 — SMART ASSESSMENT

Objective ID | Specific | Measurable | Achievable |
Relevant | Time-bound | Overall Rating |
Required Improvement

Ratings:
Strong / Acceptable / Needs Clarification / Not SMART

TABLE 3 — DEPENDENCY REVIEW

Objective ID | Primary Dependency | Dependency Owner |
Risk if Dependency Fails | Recommended Action

MANAGEMENT SUMMARY

1. Objectives requiring clarification or approval
2. Missing baselines, targets, or ownership
3. Critical dependencies and achievement risks
4. Potential conflicts with project constraints
5. Recommended management decisions

Use concise Markdown tables.
Mark missing information explicitly.
Do not present proposed targets as approved commitments.
```

---

## 2. Quality Check

Apply this quality control after generating the SMART objectives.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the SMART objectives.

Verify:

1. Completeness: Five objectives and all required analyses are present.
2. SMART Compliance: Each objective has a specific outcome,
   measurable indicator, feasible target, business relevance,
   and defined timeframe, or is flagged for clarification.
3. Evidence: Baselines, targets, deadlines, and ownership are supported
   by available information or clearly marked as unconfirmed.
4. Alignment: Objectives support business value and distinguish
   project outputs from business outcomes.
5. Dependencies: Critical risks, constraints, and external
   dependencies are identified.
6. Governance: Accountability, required approvals, and unresolved
   decisions are visible.
7. Actionability: Recommended improvements are specific and feasible.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]

Do not invent missing targets, metrics, owners, or approvals.
Flag objectives requiring stakeholder validation.
```

---

## 3. Practical IT Use Case

### Data Warehouse and BI Reporting Implementation

**Scenario:** A company is implementing a centralized data warehouse and Power BI reporting solution to replace fragmented departmental reports. The Project Manager must translate broad goals such as improving data quality and accelerating reporting into measurable objectives before the delivery plan is approved.

### Project Context

| Attribute | Details |
|---|---|
| Project | Enterprise Data Warehouse & BI Reporting |
| Phase | Initiation / Planning |
| Delivery approach | Hybrid |
| Target completion | 30 September 2027 |
| Budget | €400,000 (planning estimate) |
| Data sources | CRM, ERP, financial reporting systems |
| Key stakeholders | Finance, Sales, IT, Data Engineering, BI Team |
| Dependencies | Data access, ETL pipelines, data quality, business validation |
| Management decision | Agree measurable delivery objectives, reporting KPIs, and accountable owners |

### Example Input

```text
Project: Enterprise Data Warehouse & BI Reporting

Business problem:
Finance and Sales rely on manual Excel reporting.
Data is fragmented across CRM, ERP, and financial systems.
Reports contain inconsistencies and require repeated reconciliation.

Strategic purpose:
Establish a centralized, reliable reporting environment.

Expected business value:
- Reduce manual reporting effort.
- Improve data consistency.
- Accelerate management reporting.
- Increase access to standardized KPIs.

Target completion: 30 September 2027
Budget: €400,000 (planning estimate)
Delivery approach: Hybrid

Known information:
- Current monthly reporting takes approximately 5 working days.
- Target reporting time: 2 working days.
- CRM and ERP integrations are required.
- Power BI dashboards are planned.
- Data quality baseline has not been established.
- Business KPI definitions require stakeholder approval.
- Data Engineering resources are shared with other projects.
- Project ownership and success criteria require confirmation.
```

### Example Output — SMART Objectives

The following table is a concise illustration of the required output. Missing targets and owners are explicitly identified rather than invented.

| ID | Objective | KPI / Measurement | Target | Date | Proposed Owner | Type |
|---|---|---|---|---|---|---|
| O-01 | Implement the centralized reporting platform | Approved production deployment | Successful release | 30 Sep 2027 | IT Project Manager | Project Output |
| O-02 | Reduce monthly reporting time | Working days per reporting cycle | 5 → 2 days | TBD | Finance Lead | Business Outcome |
| O-03 | Improve data quality | Percentage of records meeting approved quality rules | Target to be confirmed | TBD | Data Lead | Quality Outcome |
| O-04 | Standardize management reporting | Percentage of priority KPIs with approved definitions | Target to be confirmed | TBD | Business Owner | Operational Outcome |
| O-05 | Reduce manual reporting activities | Manual reporting hours per month | Target to be confirmed | TBD | Finance Lead | Business Outcome |

*Proposed owners require confirmation. The completion date does not automatically establish deadlines for post-implementation business benefits.*

### SMART Assessment

| Objective | Rating | Weakness | Required Improvement |
|---|---|---|---|
| O-01 | Acceptable | Scope and acceptance criteria not finalized | Confirm release acceptance criteria |
| O-02 | Needs Clarification | Deadline and feasibility not established | Confirm measurement period and delivery feasibility |
| O-03 | Not SMART | Baseline, target, and deadline missing | Perform data profiling and agree target |
| O-04 | Not SMART | Priority KPI list and target undefined | Approve KPI definitions and coverage target |
| O-05 | Not SMART | Baseline, target, and deadline missing | Measure current effort and agree reduction |

### Dependency Review

| Objective | Primary Dependency | Proposed Dependency Owner | Risk if Dependency Fails |
|---|---|---|---|
| O-01 | CRM/ERP integration readiness | Data Engineering Lead | Deployment delay |
| O-02 | Automated reporting availability | BI Lead | Reporting-time target not achieved |
| O-03 | Source data quality | Data Lead | Unreliable analytical outputs |
| O-04 | Business KPI approval | Business Owner | Inconsistent management reporting |
| O-05 | Manual process assessment | Finance Lead | Benefits cannot be measured |

### Management Decisions

1. **Reporting performance:** Confirm whether reducing reporting time from five to two working days is feasible and agree on the measurement period.
2. **Data quality:** Establish a baseline and approve measurable quality thresholds before committing to improvement targets.
3. **Business alignment:** Approve KPI definitions, reporting scope, and the criteria for successful adoption.
4. **Accountability:** Confirm objective owners, dependency owners, and benefit measurement responsibilities.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The project has a defined business purpose and a measurable reporting-time target. However, several objectives lack validated baselines, target values, deadlines, and confirmed ownership.

**Required corrections:**
- Confirm the reporting-time target and measurement period.
- Establish data quality and manual-effort baselines.
- Approve KPI coverage and data quality targets.
- Confirm accountable owners and validate delivery feasibility.

**Governance:** This prompt supports relevant PMI-aligned practices in value delivery, objectives management, benefits realization, performance measurement, stakeholder accountability, and project governance.

SMART objectives require validation by the Project Sponsor, Business Owner, and relevant delivery stakeholders before becoming approved project commitments. Protect confidential financial, operational, personal, and commercially sensitive information.
