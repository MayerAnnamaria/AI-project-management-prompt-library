# Qualitative Risk Analysis

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** RISK-003 | **Category:** Risk & Issue Management

---


## 1. Ready-to-Use Prompt

**Purpose:** Assess and prioritize project risks using consistent qualitative scoring to support mitigation, monitoring, escalation, and informed management decisions.

**Use case:** Evaluate technical, delivery, vendor, security, and resource risks during project planning, milestone reviews, or release preparation when management must prioritize limited mitigation resources.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager and Risk Management Specialist
experienced in software delivery, qualitative risk assessment,
dependency management, mitigation planning, and project governance.

CONTEXT

Project: [PROJECT NAME]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Target milestone: [DATE / MILESTONE]
Assessment date: [DATE]
Risk tolerance: [APPROVED THRESHOLDS / NOT DEFINED]
Risk owners: [ROLES]
Known dependencies: [LIST]
Available risk evidence: [DATA / STATUS / HISTORICAL INFORMATION]
Existing mitigation actions: [LIST / NONE]
Risk register: [PASTE IDENTIFIED RISKS]

SCORING MODEL

Likelihood:
1 = Rare
2 = Unlikely
3 = Possible
4 = Likely
5 = Very Likely

Impact:
1 = Minimal
2 = Minor
3 = Moderate
4 = Major
5 = Severe

Risk Score = Likelihood × Impact

Risk Rating:
1–4 = Low
5–9 = Medium
10–16 = High
17–25 = Critical

Risk Proximity:
Immediate = Less than 2 weeks
Near-term = 2–6 weeks
Medium-term = 6–12 weeks
Long-term = More than 12 weeks

Scoring Confidence:
High / Medium / Low

Use this scoring model unless an approved organizational
risk methodology is provided.

TASK

Perform qualitative risk analysis and recommend management priorities.

STEP 1 — INITIAL RISK ASSESSMENT

1. Confirm each risk describes an uncertain future event,
   not an issue that has already occurred.
2. Assess likelihood using available evidence and project indicators.
3. Assess impact against schedule, cost, scope, quality,
   security, compliance, operations, and business value.
4. Calculate risk scores and apply the defined rating thresholds.
5. Assess proximity to the potential risk event.
6. Document scoring rationale, evidence, and confidence levels.
7. Identify missing information affecting assessment reliability.

STEP 2 — PRIORITIZATION AND RESPONSE

8. Rank risks using score, proximity, dependency impact,
   recovery difficulty, business exposure, and decision urgency.
9. Identify concentrations of High and Critical risks,
   shared dependencies, and potential cascading impacts.
10. Recommend proportionate mitigation, monitoring,
    or escalation actions with proposed owners.
11. Identify risks exceeding organizational tolerance,
    threatening milestones, or requiring management authority.

STEP 3 — RESIDUAL RISK REVIEW

12. Distinguish initial exposure from residual exposure.
13. Assess whether mitigation actions are planned,
    implemented, and demonstrated effective.
14. Re-score residual likelihood and impact only when
    supported by evidence of mitigation effectiveness.
15. Where mitigation is not implemented, distinguish
    forecast residual exposure from verified residual exposure.
16. Assess residual acceptability against approved risk tolerance.
17. Identify further actions, monitoring needs,
    and formal risk acceptance decisions.

Do not invent probabilities, scoring evidence, or risk tolerance.
Do not reduce scores simply because mitigation is planned.
Flag unsupported assessments for expert validation.
Do not classify a risk as accepted without authorized approval.

OUTPUT FORMAT

1. QUALITATIVE RISK REGISTER

Risk ID | Risk Description | Likelihood | Impact |
Score | Rating | Proximity | Primary Impact Area |
Priority Rank | Confidence | Scoring Rationale |
Recommended Management Focus

2. RISK PROFILE SUMMARY

Rating | Number of Risks | Management Approach

Provide commentary on:
- High and Critical risk concentrations
- Shared dependencies and cascading exposure
- Most urgent management priorities

3. MITIGATION AND ESCALATION

Risk ID | Recommended Response | Proposed Owner |
Required By | Escalation Trigger | Decision Required

4. RESIDUAL RISK ASSESSMENT

Risk ID | Initial Score / Rating | Mitigation Status |
Mitigation Evidence | Residual Likelihood | Residual Impact |
Residual Score / Rating | Exposure Acceptable? |
Further Action

Clearly distinguish forecast residual risk from
verified post-mitigation residual risk.

5. SCORING CONFIDENCE

Risk ID | Confidence | Missing Evidence |
Required Validation | Proposed Owner

6. MANAGEMENT SUMMARY

- Five highest-priority risks
- Overall risk exposure
- Immediate mitigation and escalation requirements
- Residual risks requiring management attention
- Recommended decisions and next review actions

Use concise Markdown tables.
Mark unsupported scores as "Not assessed".
Label proposed actions and ownership as unconfirmed.
```

---

## 2. Quality Check

Apply this quality control after generating the Qualitative Risk Analysis.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the risk analysis.

Verify:

1. Validity: Each risk describes an uncertain event,
   not an issue that has already occurred.
2. Accuracy: Likelihood, impact, scores, and ratings
   follow the defined scoring model.
3. Evidence: Scoring rationale, confidence,
   assumptions, and information gaps are explicit.
4. Prioritization: Rankings consider proximity,
   dependencies, recovery difficulty, and business impact.
5. Completeness: Major project risk categories
   and shared dependencies are assessed.
6. Mitigation: Recommended actions address risk causes
   or consequences and have proposed owners.
7. Residual Risk: Forecast exposure is distinguished
   from verified mitigation effectiveness.
8. Governance: Escalation, risk tolerance, and
   acceptance authority are correctly addressed.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Escalation / Acceptance Blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent scoring evidence, risk thresholds,
mitigation effectiveness, or approvals.
Flag assessments requiring expert validation.
```

---

## 3. Practical IT Use Case

### Software Development — Release Risk Assessment

**Scenario:** A software development team is preparing for integration testing and a planned production release. Several technical and operational uncertainties could affect the schedule, including API readiness, defects, business-user availability, and security approval.

The Project Manager must prioritize mitigation actions and determine which risks require management intervention.

### Project Context

| Attribute | Details |
|---|---|
| Project | Web Application Reporting Enhancement |
| Phase | Development / Integration |
| Delivery approach | Scrum |
| Assessment date | 17 May 2027 |
| Target release | 30 June 2027 |
| Team | Developers, QA, Product Owner, Project Manager |
| Critical milestones | SIT, UAT, Security Approval, Production Release |
| Risk tolerance | Not formally defined |
| Management decision | Prioritize mitigation and identify release risks requiring escalation |

### Example Input

```text
Project: Web Application Reporting Enhancement

Business objective:
Deliver enhanced reporting functionality by 30 June 2027.

Current phase: Development / Integration
Delivery approach: Scrum
Assessment date: 17 May 2027

Upcoming milestones:
- SIT completion: 5 June
- UAT completion: 19 June
- Release readiness: 25 June
- Production release: 30 June

Known information:

R-01 — API Integration
The reporting API is not yet integration-ready.
The integration team forecasts completion on 29 May,
leaving limited time before SIT completion.

R-02 — UAT Availability
Business users have not confirmed their availability
for the planned UAT window.

R-03 — Critical Defects
Two major reporting defects remain open.
The team has not confirmed whether additional
release-blocking defects will be identified.

R-04 — Security Approval
The application security review is scheduled,
but approval has not yet been received.

R-05 — QA Capacity
The QA team is also supporting another release.
Available capacity for regression testing is uncertain.

Existing mitigation:
- Developers are prioritizing API endpoints.
- QA is preparing integration test cases.
- The Product Owner has requested UAT availability confirmation.

Risk tolerance:
Not formally defined.

Assessment requirement:
Use the supplied 5×5 qualitative scoring model.
Identify scoring uncertainty and proposed escalation actions.
```

### Example Output — Qualitative Risk Analysis

The scores below are **illustrative expert judgments**, not measured probabilities. They require validation by the relevant risk owners.

#### 1. Qualitative Risk Register

| Risk ID | Risk Description | L | I | Score | Rating | Proximity | Priority |
|---|---|---:|---:|---:|---|---|---:|
| R-01 | API may not be ready for SIT completion | 4 | 4 | 16 | High | Immediate | 1 |
| R-02 | Business users may be unavailable for UAT | 4 | 4 | 16 | High | Near-term | 2 |
| R-03 | Critical defects may remain at release readiness | 3 | 5 | 15 | High | Near-term | 3 |
| R-04 | Security approval may be delayed | 3 | 5 | 15 | High | Medium-term | 4 |
| R-05 | Limited QA capacity may delay regression testing | 3 | 4 | 12 | High | Immediate | 5 |

**Primary impact areas and scoring rationale**

| Risk | Primary Impact | Confidence | Scoring Rationale |
|---|---|---|---|
| R-01 | Schedule / Integration | Medium | API forecast leaves limited SIT time |
| R-02 | Schedule / Business Acceptance | Low | UAT resource commitments are unconfirmed |
| R-03 | Quality / Release | Low | Open defects exist; future defect exposure is uncertain |
| R-04 | Security / Release | Low | Approval is pending; completion probability is unknown |
| R-05 | Capacity / Testing | Low | QA resources are shared and availability is unvalidated |

The current API readiness problem should also be checked for an existing issue record. The risk assessment addresses the uncertain downstream consequence; confirmed delays or blockers must be managed as issues.

#### 2. Risk Profile Summary

| Rating | Number of Risks | Management Approach |
|---|---:|---|
| Critical | 0 | Immediate escalation if identified |
| High | 5 | Active mitigation and frequent review |
| Medium | 0 | Monitor and manage |
| Low | 0 | Periodic review |

**Management interpretation:** The illustrative profile is concentrated in integration, testing, and release-readiness exposure. API readiness and QA capacity require immediate attention because they may affect SIT, while unresolved business availability threatens UAT.

A potential cascading dependency is:

`API Readiness → SIT Completion → UAT Readiness → Release Approval`

The ranking considers event proximity and downstream impact, not numerical scores alone.

#### 3. Mitigation and Escalation

| Risk | Recommended Response | Proposed Owner | Required By | Escalation Trigger |
|---|---|---|---|---|
| R-01 | Confirm endpoint readiness and integration recovery plan | Development Lead | Before SIT decision | API delivery threatens SIT |
| R-02 | Secure UAT resource commitments | Product Owner | Before UAT | Required users remain unavailable |
| R-03 | Prioritize release-critical defect resolution | QA / Development Leads | Before readiness review | Mandatory release criteria at risk |
| R-04 | Confirm security review dependencies and approval forecast | Security Lead | Before release approval | Security clearance threatens release |
| R-05 | Assess QA capacity and reallocate work if approved | Project Manager / QA Lead | Before regression execution | Testing cannot meet required coverage |

**Escalation authority:** Not yet defined. Any decision to change scope, increase capacity, accept residual exposure, or revise the release date requires appropriate authorization.

#### 4. Residual Risk Assessment

Mitigation activities are either planned or in progress. No verified mitigation effectiveness has been provided, so lower residual scores cannot yet be justified.

| Risk | Initial Rating | Mitigation Status | Verified Residual Rating | Further Action |
|---|---|---|---|---|
| R-01 | High (16) | Prioritization in progress | Not assessed | Verify API readiness and test results |
| R-02 | High (16) | Availability requested | Not assessed | Obtain confirmed UAT allocation |
| R-03 | High (15) | Resolution planning required | Not assessed | Verify fixes and test evidence |
| R-04 | High (15) | Security review scheduled | Not assessed | Obtain security decision |
| R-05 | High (12) | Capacity assessment required | Not assessed | Validate available QA capacity |

**Residual exposure acceptability:** Not determined. Risk tolerance has not been approved, and mitigation effectiveness has not been demonstrated.

#### 5. Scoring Confidence

| Risk | Confidence | Missing Evidence | Proposed Validation Owner |
|---|---|---|---|
| R-01 | Medium | API completion evidence and SIT impact | Development Lead |
| R-02 | Low | Confirmed business-user allocation | Product Owner |
| R-03 | Low | Defect trends, severity, and resolution forecast | QA Lead |
| R-04 | Low | Security review outcome and remaining actions | Security Lead |
| R-05 | Low | QA capacity and regression effort forecast | QA Lead |

Risk ratings should be reviewed when these data become available.

### Management Decisions

1. **Integration:** Confirm whether the API forecast supports the planned SIT completion milestone and approve any necessary recovery actions.
2. **Testing capacity:** Validate QA and business-user availability before committing to SIT and UAT completion dates.
3. **Release readiness:** Agree on critical defect and security approval requirements for the go/no-go decision.
4. **Risk governance:** Define risk tolerance, escalation authority, and conditions for accepting residual exposure.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The analysis provides consistent scoring calculations, identifies shared schedule dependencies, and prioritizes management action. However, most scores rely on limited evidence, mitigation effectiveness is unverified, and organizational risk tolerance is undefined.

**Required corrections:**
- Validate likelihood and impact assessments with risk owners.
- Confirm API, QA, UAT, and security readiness evidence.
- Establish documented escalation and risk acceptance authority.
- Reassess risk ratings when material new evidence is available.
- Evaluate residual exposure only after mitigation effectiveness is verified.

**Escalation / Acceptance Blockers:** Undefined risk tolerance, insufficient evidence for several scores, and unverified mitigation effectiveness.

**Governance:** This prompt supports PMI-aligned practices in qualitative risk assessment, prioritization, uncertainty management, response planning, monitoring, and escalation.

The analysis is a management decision-support artifact. Risk scores and residual exposure require validation by accountable risk owners, technical experts, and authorized governance stakeholders. Protect confidential project, security, customer, vendor, and commercially sensitive information.
