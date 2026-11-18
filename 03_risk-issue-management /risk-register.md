# Project Risk Register

**Prompt ID:** RISK-001 | **Category:** Risk & Issue Management | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Identify, assess, prioritize, and monitor project risks to support proactive mitigation, accountability, and management decisions.

**Use case:** Create or update a risk register during software implementation, integration testing, release preparation, or milestone reviews when delivery uncertainty threatens project commitments.

Copy the prompt and replace the placeholders.

```text
ROLE

You are a Senior IT Project Manager specializing in software
delivery, risk assessment, dependency management, and governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target completion: [DATE]
Budget: [AMOUNT / RANGE]
Team and stakeholders: [ROLES]
Vendors: [IF RELEVANT]
Systems and integrations: [LIST]
Dependencies: [LIST]
Constraints: [LIST]
Assumptions: [LIST]
Known risks: [LIST]
Known issues: [LIST]
Risk tolerance: [APPROVED THRESHOLDS / UNKNOWN]
Existing register: [PASTE IF AVAILABLE]
Assessment date: [DATE]

SCORING MODEL

Likelihood: 1 Rare | 2 Unlikely | 3 Possible |
            4 Likely | 5 Very Likely

Impact: 1 Minimal | 2 Minor | 3 Moderate |
        4 Major | 5 Severe

Risk Score = Likelihood × Impact

Rating:
1–4 Low | 5–9 Medium | 10–16 High | 17–25 Critical

Proximity:
Immediate <2 weeks | Near-term 2–6 weeks |
Medium-term 6–12 weeks | Long-term >12 weeks

Use approved organizational scoring rules where available.
Otherwise, treat this model as provisional.

TASK

Create or update a Project Risk Register and prioritize
the risks requiring management attention.

STEP 1 — IDENTIFICATION

1. Identify material uncertainty affecting schedule, cost,
   scope, resources, technology, data, security, quality,
   operations, and business outcomes.
2. Write risks using cause–event–impact:
   "Because of [CAUSE], [EVENT] may occur,
   resulting in [IMPACT]."
3. Separate future risks from existing issues.
4. Identify related assumptions, constraints, dependencies,
   and duplicate or unsupported statements.

STEP 2 — ASSESSMENT

5. Assess likelihood and impact using available evidence.
6. Calculate scores and assign ratings consistently.
7. Identify proximity, early warning indicators,
   and scoring confidence.
8. Prioritize using score, urgency, dependency impact,
   recovery difficulty, and business exposure.
9. Identify shared causes and cascading risks.

STEP 3 — RESPONSE

10. Recommend Avoid / Mitigate / Transfer or Share /
    Accept / Escalate, as appropriate.
11. Separate preventive mitigation from contingency actions.
12. For High/Critical risks, specify actions, Risk Owner,
    Action Owner, due date, and escalation trigger.
13. Flag decisions exceeding project-level authority.

STEP 4 — MONITORING

14. Define review dates, status, and progress indicators.
15. Monitor changes in exposure, proximity, and mitigation.
16. Distinguish planned mitigation from verified residual risk.
17. Convert materialized risks into linked issues.
18. Identify the five highest-priority risks and recommend
    management actions.

Do not invent evidence, scores, owners, dates, or approvals.
Mark unsupported assessments as provisional or "Not assessed".

OUTPUT FORMAT

1. PROJECT RISK REGISTER

Risk ID | Category | Risk Statement | Cause |
Potential Event | Potential Impact | Likelihood |
Impact | Score | Rating | Proximity |
Early Warning Indicator | Mitigation | Contingency |
Risk Owner | Action Owner | Review Date | Status

2. RISK PRIORITIZATION

Priority | Risk ID | Current Exposure |
Management Concern | Immediate Action |
Decision Required | Decision Owner | Deadline

3. RISK INTERDEPENDENCIES

Related Risks | Common Cause | Dependency Chain |
Cascading Impact | Recommended Action

4. RISK RESPONSE AND ESCALATION

Risk ID | Strategy | Preventive Action |
Contingency Trigger / Action | Proposed Owner |
Due Date | Escalation Trigger

5. RISK MONITORING

Risk ID | Rating | Proximity | Warning Status |
Mitigation Progress | Residual Exposure | Next Review

6. MANAGEMENT SUMMARY

- Five highest-priority risks
- Risk concentrations and dependencies
- Immediate mitigation and escalation
- Evidence and ownership gaps
- Required management decisions

Use concise Markdown tables.
Clearly label unconfirmed assignments and assessments.
```

---

## 2. Quality Check

Apply this control after generating the register.

```text
QUALITY CHECK

Act as a Senior QA Manager and validate the Project Risk Register.

Verify:

1. Validity: Risks are uncertain future events, not existing issues.
2. Completeness: Material risks, dependencies, indicators,
   responses, and ownership are covered.
3. Accuracy: Cause–event–impact statements and calculations
   follow the scoring model.
4. Evidence: Scores, proximity, and priority are justified
   or marked provisional.
5. Prioritization: Business impact, urgency, dependencies,
   and recovery difficulty are considered.
6. Response: Mitigation and contingency are distinct,
   actionable, and proportionate.
7. Governance: Ownership, review dates, escalation,
   and acceptance authority are clear or flagged.
8. Monitoring: Risk trends and residual exposure are tracked
   without assuming mitigation effectiveness.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent evidence, ownership, or approvals.
```

---

## 3. Practical IT Use Case

### SaaS Implementation — Integration and Release Risks

**Scenario:** An IT team is replacing a legacy ticketing application with a SaaS platform. The project requires identity integration, historical-data migration, workflow configuration, and UAT. The Project Manager must prioritize risks before production deployment.

### Project Context

| Attribute | Details |
|---|---|
| Project | IT Service Desk SaaS Implementation |
| Phase | Configuration / Integration |
| Delivery approach | Hybrid |
| Go-live target | 30 September 2027 |
| Systems | Legacy Ticketing, SaaS Platform, Identity Provider |
| Vendor | SaaS Implementation Partner |
| Key dependencies | Integration, migration, UAT, release readiness |
| Management decision | Confirm risk priorities, mitigation ownership, and escalation |

### Example Input

```text
Project: IT Service Desk SaaS Implementation

Business objective:
Replace the legacy ticketing system and improve
support-request management.

Phase: Configuration / Integration
Delivery approach: Hybrid
Go-live: 30 September 2027

Known information:
- Identity integration testing has not started.
- Historical tickets contain duplicate records.
- UAT availability is not confirmed.
- Vendor workflow configuration is incomplete.
- Training materials are awaiting approval.

Existing issue:
Duplicate records identified during data profiling.

Constraints:
- Fixed go-live target
- Limited IT support capacity
- External vendor dependency

Risk tolerance: Not defined.

Task:
Use the provisional 5×5 model and identify risks
requiring immediate management attention.
```

### Example Output — Project Risk Register

All scores are **illustrative and require validation** by the relevant risk owners.

#### 1. Project Risk Register

| ID | Category | Risk Statement | L | I | Score | Rating |
|---|---|---|---:|---:|---:|---|
| R-01 | Integration | Untested identity integration may delay UAT if defects emerge. | 4 | 4 | 16 | High |
| R-02 | Data | Inadequate duplicate remediation may cause migration acceptance failure. | 4 | 4 | 16 | High |
| R-03 | Resources | Unavailable business testers may delay UAT. | 3 | 4 | 12 | High |
| R-04 | Vendor | Late workflow configuration may delay testing and training. | 3 | 4 | 12 | High |
| R-05 | Operations | Unapproved training materials may affect go-live readiness. | 3 | 3 | 9 | Medium |

**Response and ownership details**

| Risk | Early Warning | Mitigation | Contingency | Proposed Risk Owner |
|---|---|---|---|---|
| R-01 | Integration start slips | Validate API and test readiness | Re-sequence approved testing | IT Lead |
| R-02 | Reconciliation failures | Cleanse and validate source data | Approved remediation plan | Data Lead |
| R-03 | UAT slots unconfirmed | Secure user commitments | Escalate resource shortage | Business Owner |
| R-04 | Vendor checkpoints slip | Monitor configuration delivery | Vendor recovery plan | Project Manager |
| R-05 | Training remains unapproved | Confirm review schedule | Additional approved training | Service Desk Manager |

Action owners, dates, risk proximity, and review status require confirmation.

The duplicate-record problem is already an **issue**. R-02 represents its uncertain future impact on migration acceptance.

#### 2. Risk Prioritization

| Priority | Risk | Management Concern | Immediate Action |
|---|---|---|---|
| 1 | R-01 | Integration could block UAT | Confirm API readiness |
| 2 | R-02 | Migration may fail acceptance | Assess data remediation |
| 3 | R-03 | UAT capacity uncertain | Confirm business availability |
| 4 | R-04 | Vendor delay affects downstream work | Obtain updated forecast |
| 5 | R-05 | Training readiness incomplete | Confirm approval plan |

Ranking is illustrative; final priority requires proximity, dependency, and recovery evidence.

#### 3. Risk Interdependencies

| Related Risks | Dependency Chain | Cascading Impact |
|---|---|---|
| R-01 / R-03 | Identity Integration → UAT | Delayed acceptance |
| R-02 / R-03 | Data Remediation → Migration Validation → UAT | Testing delays |
| R-04 / R-05 | Workflow Configuration → Training → Go-Live | Reduced readiness |

Multiple risks converge on UAT and go-live, increasing the importance of coordinated mitigation.

#### 4. Risk Response and Escalation

| Risk | Strategy | Preventive Action | Escalation Trigger |
|---|---|---|---|
| R-01 | Mitigate | Confirm integration readiness | UAT milestone threatened |
| R-02 | Mitigate | Define cleansing and reconciliation criteria | Migration acceptance at risk |
| R-03 | Mitigate | Confirm business-user allocation | Insufficient UAT capacity |
| R-04 | Mitigate | Establish vendor checkpoints | Configuration milestone missed |
| R-05 | Mitigate | Approve training plan | Operational readiness threatened |

Contingency actions, decision owners, and deadlines must be validated before formal adoption.

#### 5. Risk Monitoring

| Risk | Rating | Warning Status | Residual Exposure | Next Review |
|---|---|---|---|---|
| R-01 | High | Testing not started | Not assessed | Integration review |
| R-02 | High | Duplicates identified | Not assessed | Migration review |
| R-03 | High | Availability unconfirmed | Not assessed | UAT planning |
| R-04 | High | Configuration incomplete | Not assessed | Vendor review |
| R-05 | Medium | Training approval pending | Not assessed | Readiness review |

No risk reduction is assumed without evidence of mitigation effectiveness.

### Management Decisions

1. **Integration:** Confirm API readiness and recovery options before UAT.
2. **Data quality:** Approve migration acceptance criteria and remediation ownership.
3. **Business readiness:** Secure UAT resources and training approvals.
4. **Governance:** Validate scores, owners, escalation thresholds, and review dates.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** Key risks and dependencies are identified, but scores, proximity, ownership, and mitigation effectiveness remain unverified.

**Required corrections:** Validate assessments with risk owners; confirm action owners, deadlines, warning thresholds, and escalation authority; track the existing data-quality issue separately.

**Approval blockers:** Unconfirmed ownership, limited scoring evidence, and undefined risk tolerance.

**Governance:** Supports PMI-aligned risk identification, assessment, response planning, monitoring, and escalation. Human validation and authorized risk acceptance remain mandatory. Protect confidential project, customer, vendor, and security information.
