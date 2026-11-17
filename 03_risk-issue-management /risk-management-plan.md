# Risk Management Plan

## Purpose

Use this prompt to create a structured Risk Management Plan for an IT, software, digital transformation, data, infrastructure, or technology-enabled project.

The plan should define:

- how risks will be identified,
- how risks will be assessed,
- who owns them,
- how responses will be planned,
- how risks will be monitored,
- when escalation is required,
- and how risk information will be reported.

The objective is to create a **repeatable project risk-management process**, not merely a one-time risk register.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Multi-vendor programme

**Primary user:**  
Project Manager / Delivery Manager / PMO / Risk Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
Create during project planning and review after material governance, scope, risk, or delivery changes

---

# Prompt

```text id="risk-plan-01"
ROLE

You are a senior IT Project Manager and risk-management specialist
experienced in international software delivery, digital transformation,
project governance, vendor management, technology risk, and
cross-functional delivery.

TASK

Create a professional Risk Management Plan for the project
described below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Project duration:
[DURATION]

Target completion:
[DATE]

Budget:
[BUDGET OR RANGE]

Project team:
[DETAILS]

External vendors:
[LIST]

Key systems:
[LIST]

Known dependencies:
[LIST]

Known constraints:
[LIST]

Governance structure:
[DETAILS]

Risk appetite / tolerance:
[IF KNOWN]

Reporting requirements:
[DETAILS]

OUTPUT FORMAT

Create a Risk Management Plan covering:

1. Purpose and Scope
2. Risk Management Approach
3. Roles and Responsibilities
4. Risk Appetite and Tolerance
5. Risk Identification Process
6. Qualitative Risk Analysis
7. Quantitative Risk Analysis Where Applicable
8. Risk Response Planning
9. Risk Ownership and Allocation
10. Risk Monitoring and Review
11. Risk Reporting
12. Risk Escalation
13. Risk Register Structure
14. Risk Review Cadence
15. Risk Closure
16. Continuous Improvement
```

---

# 1. Purpose and Scope

Define:

```text id="risk-plan-purpose"
Why risk management is required

Which project areas are included

Which stakeholders participate

How risk management supports project decisions

How risk management interacts with project governance
```

The plan should apply to material uncertainty affecting:

- delivery,
- cost,
- scope,
- quality,
- security,
- compliance,
- operations,
- customers,
- business outcomes.

---

# 2. Risk Management Approach

Describe the project's overall risk process.

Recommended flow:

```text id="risk-plan-process"
Identify
↓
Analyse
↓
Prioritise
↓
Plan Response
↓
Assign Ownership
↓
Monitor
↓
Escalate
↓
Close / Reassess
```

Risk management should remain continuous throughout the project.

---

# Risk Principles

The project should manage risks using the following principles:

```text id="risk-principles"
Evidence before assumption

Clear ownership

Early identification

Proportionate analysis

Specific response actions

Visible escalation thresholds

Regular review

Transparent reporting

Continuous reassessment
```

---

# 3. Roles and Responsibilities

Define responsibilities clearly.

Suggested structure:

| Role | Risk Responsibility |
|---|---|
| Project Sponsor | Owns escalated strategic risks and risk acceptance beyond project authority |
| Project Manager | Maintains overall risk process and governance |
| Risk Owner | Accountable for individual risk management |
| Action Owner | Completes specific mitigation actions |
| Technical Lead | Identifies and assesses technical risks |
| Security Lead | Manages security-related risk assessment |
| Business Owner | Assesses business impact and business-side risks |
| Vendor Lead | Manages supplier-related risk actions |
| PMO | Provides governance, standards, and reporting support |

Actual responsibilities should follow the organisation's governance model.

---

# 4. Risk Appetite and Tolerance

Define how much risk the project or organisation is prepared to accept.

Possible dimensions include:

```text id="risk-tolerance"
Schedule
Cost
Quality
Security
Compliance
Operations
Customer Impact
Reputation
Business Value
```

Example:

```text id="risk-tolerance-example"
Schedule tolerance:
Up to 5 working days at Project Manager level.

Beyond 5 working days:
Sponsor escalation required.

Security:
No unapproved Critical security exposure accepted for production.
```

Use actual organisational thresholds where available.

Do not invent risk tolerance.

---

# 5. Risk Identification Process

Define how risks will be identified.

Possible methods:

```text id="risk-identification-methods"
Risk workshops
Project team reviews
Dependency reviews
Architecture reviews
Vendor reviews
Testing findings
Assumption reviews
Lessons learned
Historical data
Stakeholder interviews
Delivery metrics
Audit findings
```

Risk identification should not depend solely on formal workshops.

---

# Risk Identification Sources

Consider risks arising from:

```text id="risk-sources"
Scope
Requirements
Architecture
Technology
Integration
Data
Security
Testing
Resources
Vendors
Schedule
Budget
Operations
Stakeholders
Governance
Compliance
External dependencies
```

---

# 6. Qualitative Risk Analysis

Define the project's scoring method.

Example:

```text id="risk-matrix"
Likelihood:
1–5

Impact:
1–5

Risk Score:
Likelihood × Impact
```

Suggested classification:

```text id="risk-rating-plan"
1–4 = Low
5–9 = Medium
10–16 = High
17–25 = Critical
```

Use organisational thresholds instead where defined.

---

# Qualitative Assessment Should Consider

Do not rely only on numerical score.

Also consider:

```text id="risk-analysis-factors"
Proximity
Dependency impact
Recovery difficulty
Business impact
Security / compliance impact
Decision urgency
Cross-workstream impact
Confidence in assessment
```

---

# 7. Quantitative Risk Analysis

Use quantitative analysis only where it adds management value.

Possible applications:

- schedule uncertainty,
- budget exposure,
- forecast ranges,
- contingency analysis,
- scenario analysis.

Do not create numerical precision where the available information does not support it.

Where quantitative analysis is not required, state:

> Not currently required for this project.

---

# 8. Risk Response Planning

For significant risks define:

```text id="risk-response-plan-fields"
Response Strategy
Preventive Actions
Trigger Point
Contingency
Risk Owner
Action Owner
Deadline
Residual Risk
```

Possible strategies:

```text id="risk-strategies-plan"
Avoid
Mitigate
Transfer / Share
Accept
Escalate
```

Avoid generic responses such as:

> Monitor closely.

Every significant response should explain what action changes the exposure.

---

# 9. Risk Ownership and Allocation

Each material risk should have one clear **Risk Owner**.

Ownership should follow:

- authority,
- ability to influence the risk,
- responsibility for the affected outcome.

Do not assign the Project Manager as owner of every risk by default.

Example:

```text id="risk-allocation-example"
Security approval risk
→ Security Lead

Business UAT availability risk
→ Business Owner

Vendor delivery risk
→ Vendor / Delivery Lead

Overall programme escalation
→ Project Manager / Sponsor
```

---

# 10. Risk Monitoring and Review

Define how risks will be monitored.

At each review ask:

```text id="risk-monitoring"
Has likelihood changed?

Has impact changed?

Has proximity changed?

Has mitigation progressed?

Has the trigger been reached?

Has the risk materialised?

Has the residual rating changed?

Does the risk require escalation?

Can the risk be closed?
```

---

# Risk Review Cadence

Possible cadences:

```text id="risk-cadence"
Weekly project risk review

Monthly steering committee risk review

Release-readiness risk review

Major milestone risk review

Ad hoc review after material change
```

Frequency should match project complexity.

---

# 11. Risk Reporting

Define what is reported to each audience.

## Delivery Team

Focus on:

- current actions,
- blockers,
- dependencies,
- trigger indicators.

## Project Governance

Focus on:

- High / Critical risks,
- exposure trends,
- overdue mitigation,
- decisions required.

## Executives / Sponsor

Focus on:

- material business exposure,
- strategic risks,
- required decisions,
- risk tolerance breaches.

---

# Risk Dashboard

Possible dashboard fields:

```text id="risk-dashboard"
Total Active Risks
Critical Risks
High Risks
New Risks
Closed Risks
Escalated Risks
Overdue Mitigation Actions
Top Risk Trend
```

Do not use dashboard metrics that do not support decisions.

---

# 12. Risk Escalation

Escalate when:

```text id="risk-plan-escalation"
Risk exceeds agreed tolerance.

Critical milestone is threatened.

Security or compliance exposure becomes material.

Required response exceeds Project Manager authority.

Additional budget is required.

Multiple workstreams are affected.

Vendor intervention requires senior authority.

Residual risk remains unacceptable.
```

For each escalation specify:

```text id="risk-escalation-fields"
Risk
Reason
Decision Required
Decision Owner
Decision Deadline
Impact if Delayed
```

---

# 13. Risk Register Structure

Recommended fields:

```text id="risk-register-fields"
Risk ID
Category
Risk Statement
Cause
Potential Impact
Likelihood
Impact
Score
Rating
Proximity
Early Warning Indicator
Response Strategy
Mitigation
Contingency
Risk Owner
Action Owner
Due Date
Review Date
Residual Rating
Status
```

---

# 14. Risk Review Schedule

Define when formal risk reviews occur.

Example:

| Review | Frequency | Participants | Output |
|---|---|---|---|
| Delivery Risk Review | Weekly | PM + Leads | Updated register |
| Vendor Risk Review | Biweekly | PM + Vendor | Vendor actions |
| Steering Risk Review | Monthly | Sponsor + PM | Decisions / escalation |
| Release Risk Review | Before release | Delivery + Security + Ops | Release risk decision |

---

# 15. Risk Closure

A risk may be closed when:

```text id="risk-closure"
Risk can no longer occur.

Risk period has passed.

Underlying dependency is resolved.

Exposure is formally accepted.

Risk has materialised and become an issue.
```

Closure should include:

- closure reason,
- date,
- evidence where relevant.

---

# 16. Continuous Improvement

After significant risks or project milestones, review:

```text id="risk-improvement"
Which risks were identified too late?

Which mitigations were effective?

Which triggers worked?

Which assumptions were wrong?

Which risks materialised unexpectedly?

What should future projects do differently?
```

This connects project risk management to lessons learned.

---

# Agile / Scrum Considerations

Risk management should complement Agile delivery.

Relevant signals may include:

- backlog volatility,
- team capacity,
- technical debt,
- cross-team dependencies,
- release uncertainty,
- defect trends.

Do not create unnecessary governance layers around risks that the delivery team can resolve directly.

---

# Kanban Considerations

Flow metrics may provide early-warning signals.

Examples:

```text id="risk-plan-kanban"
Increasing WIP

Ageing work

Blocked items

Cycle-time deterioration

Throughput decline

Repeated SLE breaches
```

Use these indicators to reassess emerging delivery risks where relevant.

---

# Predictive Considerations

Risk management may link closely to:

- schedule baseline,
- critical path,
- cost baseline,
- procurement,
- formal change control.

---

# Hybrid Considerations

Combine:

```text id="risk-plan-hybrid"
Formal project-level risk governance
+
Adaptive delivery signals
```

Example:

```text id="risk-hybrid-process"
Delivery signal
↓
Risk identified
↓
Project-level assessment
↓
Mitigation
↓
Escalation if tolerance exceeded
```

---

# Example Input

```text id="risk-plan-example"
Project:
CRM Replacement

Delivery Approach:
Hybrid

Duration:
10 months

Budget:
€1.8 million

Key Vendors:
CRM implementation partner
Data migration specialist

Known Risk Areas:
Data quality
Integration
Business-user availability
Security approval
Vendor capacity
Release readiness

Governance:
Weekly delivery review
Monthly steering committee
```

---

# Example Risk Governance Model

```text id="risk-plan-example-output"
Weekly:
Project team reviews active risks and mitigation actions.

Monthly:
Steering Committee reviews High and Critical risks.

Immediate:
Critical security, regulatory, or milestone risks are escalated
outside the normal reporting cycle.

Risk Owner:
Maintains individual risk response.

Project Manager:
Maintains overall register and escalation process.

Sponsor:
Approves risk acceptance beyond project tolerance.
```

---

# Quality Checklist

Before approving the Risk Management Plan, confirm:

- [ ] Risk process is defined
- [ ] Roles are clear
- [ ] Risk tolerance is explicit where known
- [ ] Identification methods are defined
- [ ] Scoring methodology is documented
- [ ] Response planning is defined
- [ ] Owners are required
- [ ] Escalation thresholds exist
- [ ] Reporting audiences are defined
- [ ] Review cadence is documented
- [ ] Risk closure rules exist
- [ ] Residual risk is considered
- [ ] Lessons learned are included

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- risk planning,
- uncertainty management,
- risk identification,
- qualitative analysis,
- quantitative analysis,
- response planning,
- monitoring,
- stakeholder communication,
- governance.

## ISO 31000 Relevance

The plan can support ISO 31000-style principles such as:

- structured risk management,
- integration with decision-making,
- continuous monitoring,
- stakeholder involvement,
- adaptation to context.

Use organisational risk standards where they differ.

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

Validate the Risk Management Plan with:

- Project Manager
- PMO / Risk function
- Project Sponsor
- Business Owner
- Technical Lead
- Security
- key vendors where relevant

AI can assist with drafting and consistency checks.

It cannot define the organisation's actual risk appetite, approve risk acceptance, or replace governance decisions.

---

# Confidentiality

Risk-management documents may contain sensitive information.

Protect:

- security vulnerabilities,
- commercial exposure,
- vendor concerns,
- customer information,
- regulatory matters,
- confidential financial impact,
- personal performance information.

Use anonymised information where required.

---

# Prompt Metadata

```text id="risk-plan-metadata"
Prompt ID: RISK-006
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager / Risk Manager
Reviewer: PMO / Sponsor
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: High
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT Risk Management Plan framework |
